# Comparing `tmp/jupyter_jobstorm-0.1.2-py3-none-any.whl.zip` & `tmp/jupyter_jobstorm-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 6741 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      123 b- defN 23-Jul-02 09:01 jobstorm/__init__.py
--rw-rw-r--  2.0 unx    13096 b- defN 23-Jul-04 15:35 jobstorm/jobcode.py
--rw-rw-r--  2.0 unx     1076 b- defN 23-Jul-04 15:44 jupyter_jobstorm-0.1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2335 b- defN 23-Jul-04 15:44 jupyter_jobstorm-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 15:44 jupyter_jobstorm-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-04 15:44 jupyter_jobstorm-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      583 b- defN 23-Jul-04 15:44 jupyter_jobstorm-0.1.2.dist-info/RECORD
-7 files, 17314 bytes uncompressed, 5701 bytes compressed:  67.1%
+Zip file size: 7267 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      143 b- defN 23-Jul-16 02:44 jobstorm/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-16 02:44 jobstorm/_version.py
+-rw-r--r--  2.0 unx    18845 b- defN 23-Jul-16 02:44 jobstorm/jobcode.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2653 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Jul-16 02:44 jupyter_jobstorm-0.2.0.dist-info/RECORD
+8 files, 23498 bytes uncompressed, 6111 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: jobstorm/__init__.py
 Comment: 
 
+Filename: jobstorm/_version.py
+Comment: 
+
 Filename: jobstorm/jobcode.py
 Comment: 
 
-Filename: jupyter_jobstorm-0.1.2.dist-info/LICENSE
+Filename: jupyter_jobstorm-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: jupyter_jobstorm-0.1.2.dist-info/METADATA
+Filename: jupyter_jobstorm-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: jupyter_jobstorm-0.1.2.dist-info/WHEEL
+Filename: jupyter_jobstorm-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: jupyter_jobstorm-0.1.2.dist-info/top_level.txt
+Filename: jupyter_jobstorm-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jupyter_jobstorm-0.1.2.dist-info/RECORD
+Filename: jupyter_jobstorm-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jobstorm/__init__.py

```diff
@@ -1,8 +1,8 @@
-# newsfeed.py
+from ._version import __version__
 from .jobcode import JobStorm
 from .jobcode import JobResult
 
 __all__ = [
     "JobStorm",
     "JobResult",
 ]
```

## jobstorm/jobcode.py

```diff
@@ -7,15 +7,17 @@
 import jenkins
 from tabulate import tabulate
 
 PROJECT = "jobstorm"
 SHRDIR = "/home/shared"
 IPYTMP = ["/ipykernel", "ipython-input"]
 SUFFIX = "tmp_"
+JOBCMD = "python3"
 PYTCMD = "python3"
+SAGCMD = "sage"
 PRMNAME = "server.param"
 MAXLINE = 100
 pattern = re.compile('"([^"]+)"')
 
 
 class JobResult:
     def __init__(self, output_paramfilepath, job_filename, jobstorm):
@@ -43,43 +45,43 @@
     def get_result(self):
         status = self.get_status()
         if status not in ["SUCCESS", "UNSTABLE"]:
             raise RuntimeError("job failure or job not finished.")
         return self.jobstorm.loadparam(self.output_paramfilepath)
 
 
-class JobStorm:
+class JobStormBase:
     """Job generator.
 
     Constructor options
     -------------------
     server_url : str
         URL of Jenkins.
     username : str
         Jenkins username.
     password : str
         Jenkins password.
     shared_dir : str
         root directory path of job workspace.
     project : str
         Jenkins project name.
-    python_cmd : str
-        Python command to run Python script.
+    job_cmd : str
+        command to run script.
     server_timeout : str
         timeout setting for Jenkins server.
     """
 
     def __init__(
         self,
         server_url=None,
         username=None,
         password=None,
         shared_dir=SHRDIR,
         project=PROJECT,
-        python_cmd=PYTCMD,
+        job_cmd=JOBCMD,
         server_timeout=60,
     ):
         if shared_dir is None:
             raise ValueError("shared_dir must be set.")
         if project is None:
             raise ValueError("project must be set.")
         if not pathlib.Path(shared_dir).is_absolute():
@@ -95,15 +97,15 @@
         else:
             os.makedirs(self.dirpath, exist_ok=True)
             os.chmod(self.dirpath, 0o0777)
 
         self.codes = []
         self.funcs = []
         self.srcfilepath = None
-        self.python_cmd = python_cmd
+        self.job_cmd = job_cmd
         self.server_timeout = server_timeout
 
         if server_url is not None:
             self.server = jenkins.Jenkins(
                 server_url,
                 username=username,
                 password=password,
@@ -184,32 +186,14 @@
             funcs.append(func)
 
         codes = ""
         for code in funcs:
             codes += code
         return codes
 
-    def savefunc(self):
-        self.setfunc(level=2)
-        src = self.getcode()
-        src += "\n"
-        src += "\n"
-        src += "from jobstorm import *\n"
-        src += f'jobstorm = JobStorm(shared_dir="{self.shared_dir}", project="{self.project}")\n'
-        src += "\n"
-        src += "\n"
-        src += self.getfunc()
-        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        filename = f"{SUFFIX}{tss}.py"
-        filepath = os.path.join(self.dirpath, filename)
-        with open(filepath, "w") as f:
-            f.write(src)
-        self.srcfilepath = filepath
-        return filepath
-
     def retrieve(self, name):
         for frame_tuple in inspect.stack():
             d = frame_tuple[0].f_globals
             k = d.keys()
             if not name in k:
                 continue
             v = d[name]
@@ -224,48 +208,16 @@
 
     def loadparam(self, filename):
         fin = open(filename, "rb")
         data = dill.load(fin)
         fin.close()
         return data
 
-    def makefuncjob(self, runfunc, *args, **kwargs):
-        if self.srcfilepath is None:
-            # error
-            return
-        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
-        paramfilename = f"{SUFFIX}{tss}.param"
-        paramfilepath = os.path.join(self.dirpath, paramfilename)
-        self.saveparam(paramfilepath, [args, kwargs])
-        output_paramfilepath = f"{paramfilepath}.output"
-
-        srcfile = os.path.basename(self.srcfilepath)
-
-        if inspect.isfunction(runfunc):
-            runfuncname = runfunc.__name__
-        else:
-            runfuncname = runfunc
-
-        src = f'exec(open("{srcfile}").read())\n'
-        src += "def run_jobcode():\n"
-        src += f'    params = jobstorm.loadparam("{paramfilepath}")\n'
-        src += f"    output = {runfuncname}(*params[0], **params[1])\n"
-        src += f'    jobstorm.saveparam("{output_paramfilepath}", output)\n'
-        src += "\n"
-        src += "run_jobcode()\n"
-        filename = f"{SUFFIX}{tss}_job.py"
-        filepath = os.path.join(self.dirpath, filename)
-        with open(filepath, "w") as f:
-            f.write(src)
-
-        self.server.build_job(self.project, {"job_filename": filename})
-        return JobResult(output_paramfilepath, filename, self)
-
     def create_project(self):
-        command = f"{self.python_cmd} $job_filename"
+        command = f"$job_cmd $job_filename"
         xmlstr = f"""<?xml version='1.1' encoding='UTF-8'?>
 <project>
   <actions/>
   <description></description>
   <keepDependencies>false</keepDependencies>
   <properties>
     <hudson.model.ParametersDefinitionProperty>
@@ -274,15 +226,21 @@
           <name>job_filename</name>
           <description>job filename</description>
           <trim>false</trim>
         </hudson.model.TextParameterDefinition>
         <hudson.model.TextParameterDefinition>
           <name>dirpath_of_workspace</name>
           <defaultValue>{self.dirpath}</defaultValue>
-          <description>job filename</description>
+          <description>job workspace</description>
+          <trim>false</trim>
+        </hudson.model.TextParameterDefinition>
+        <hudson.model.TextParameterDefinition>
+          <name>job_cmd</name>
+          <defaultValue>{self.job_cmd}</defaultValue>
+          <description>job command</description>
           <trim>false</trim>
         </hudson.model.TextParameterDefinition>
       </parameterDefinitions>
     </hudson.model.ParametersDefinitionProperty>
   </properties>
   <scm class="hudson.scm.NullSCM"/>
   <canRoam>true</canRoam>
@@ -298,14 +256,15 @@
       <configuredLocalRules/>
     </hudson.tasks.Shell>
   </builders>
   <publishers/>
   <buildWrappers/>
 </project>"""
         self.server.create_job(self.project, xmlstr)
+        print(f"project (name={self.project}) is created.")
 
     def delete_project(self):
         n_job = len(self.get_job_list())
         if n_job > 0:
             raise RuntimeError("all jobs must be deleted.")
         self.server.delete_job(self.project)
 
@@ -361,14 +320,88 @@
         filepath = os.path.join(self.dirpath, filename)
         try:
             os.remove(filepath)
             print(f"{filepath} is removed.")
         except:
             print(f"{filepath} is not found or some error occurs.")
 
+
+class JobStormPython(JobStormBase):
+    def __init__(
+        self,
+        server_url=None,
+        username=None,
+        password=None,
+        shared_dir=SHRDIR,
+        project=PROJECT,
+        job_cmd=PYTCMD,
+        server_timeout=60,
+    ):
+        super().__init__(
+            server_url,
+            username,
+            password,
+            shared_dir,
+            project,
+            job_cmd,
+            server_timeout,
+        )
+
+    def savefunc(self):
+        self.setfunc(level=2)
+        src = self.getcode()
+        src += "\n"
+        src += "\n"
+        src += "from jobstorm import *\n"
+        src += f'jobstorm = JobStorm(shared_dir="{self.shared_dir}", project="{self.project}")\n'
+        src += "\n"
+        src += "\n"
+        src += self.getfunc()
+        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
+        filename = f"{SUFFIX}{tss}.py"
+        filepath = os.path.join(self.dirpath, filename)
+        with open(filepath, "w") as f:
+            f.write(src)
+        self.srcfilepath = filepath
+        return filepath
+
+    def makefuncjob(self, runfunc, *args, **kwargs):
+        if self.srcfilepath is None:
+            # error
+            return
+        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
+        paramfilename = f"{SUFFIX}{tss}.param"
+        paramfilepath = os.path.join(self.dirpath, paramfilename)
+        self.saveparam(paramfilepath, [args, kwargs])
+        output_paramfilepath = f"{paramfilepath}.output"
+
+        srcfile = os.path.basename(self.srcfilepath)
+
+        if inspect.isfunction(runfunc):
+            runfuncname = runfunc.__name__
+        else:
+            runfuncname = runfunc
+
+        src = f'exec(open("{srcfile}").read())\n'
+        src += "def run_jobcode():\n"
+        src += f'    params = jobstorm.loadparam("{paramfilepath}")\n'
+        src += f"    output = {runfuncname}(*params[0], **params[1])\n"
+        src += f'    jobstorm.saveparam("{output_paramfilepath}", output)\n'
+        src += "\n"
+        src += "run_jobcode()\n"
+        filename = f"{SUFFIX}{tss}_job.py"
+        filepath = os.path.join(self.dirpath, filename)
+        with open(filepath, "w") as f:
+            f.write(src)
+
+        self.server.build_job(
+            self.project, {"job_filename": filename, "job_cmd": self.job_cmd}
+        )
+        return JobResult(output_paramfilepath, filename, self)
+
     def delete_job(self, job_number):
         def is_same_func_script_exists(job_number, func_script):
             for k, v in job_dict.items():
                 if k == job_number:
                     continue
                 if func_script == v[3]:
                     return True
@@ -387,7 +420,180 @@
         self.delete_file(f"{job_name}.param")
         self.delete_file(f"{job_name}.param.output")
         if not is_same_func_script_exists(job_number, func_script):
             self.delete_file(func_script)
         # self.server.delete_build(self.project, job_number)
         print("delete build job not implemented because of jenkins request error.")
         return
+
+
+class JobStormSage(JobStormBase):
+    def __init__(
+        self,
+        server_url=None,
+        username=None,
+        password=None,
+        shared_dir=SHRDIR,
+        project=PROJECT,
+        job_cmd=SAGCMD,
+        server_timeout=60,
+    ):
+        super().__init__(
+            server_url,
+            username,
+            password,
+            shared_dir,
+            project,
+            job_cmd,
+            server_timeout,
+        )
+
+    def savefunc(self):
+        self.setfunc(level=2)
+        src = self.getcode()
+        src += "\n"
+        src += "\n"
+        src += "from jobstorm import *\n"
+        src += f'jobstorm = JobStorm(shared_dir="{self.shared_dir}", project="{self.project}")\n'
+        src += "\n"
+        src += "\n"
+        src += "def Integer(x):\n"
+        src += "    return x\n"
+        src += "\n"
+        src += "\n"
+        src += "def RealNumber(x):\n"
+        src += "    return x\n"
+        src += "\n"
+        src += "\n"
+        src += self.getfunc()
+        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
+        filename = f"{SUFFIX}{tss}.sage"
+        filepath = os.path.join(self.dirpath, filename)
+        with open(filepath, "w") as f:
+            f.write(src)
+        self.srcfilepath = filepath
+        return filepath
+
+    def makefuncjob(self, runfunc, *args, **kwargs):
+        if self.srcfilepath is None:
+            # error
+            return
+        tss = datetime.now().strftime("%Y%m%d%H%M%S%f")
+        paramfilename = f"{SUFFIX}{tss}.param"
+        paramfilepath = os.path.join(self.dirpath, paramfilename)
+        self.saveparam(paramfilepath, [args, kwargs])
+        output_paramfilepath = f"{paramfilepath}.output"
+
+        srcfile = os.path.basename(self.srcfilepath)
+
+        if inspect.isfunction(runfunc):
+            runfuncname = runfunc.__name__
+        else:
+            runfuncname = runfunc
+
+        src = f'load("{srcfile}")\n'
+        src += "def run_jobcode():\n"
+        src += f'    params = jobstorm.loadparam("{paramfilepath}")\n'
+        src += f"    output = {runfuncname}(*params[0], **params[1])\n"
+        src += f'    jobstorm.saveparam("{output_paramfilepath}", output)\n'
+        src += "\n"
+        src += "run_jobcode()\n"
+        filename = f"{SUFFIX}{tss}_job.sage"
+        filepath = os.path.join(self.dirpath, filename)
+        with open(filepath, "w") as f:
+            f.write(src)
+
+        self.server.build_job(
+            self.project, {"job_filename": filename, "job_cmd": self.job_cmd}
+        )
+        return JobResult(output_paramfilepath, filename, self)
+
+    def delete_job(self, job_number):
+        def is_same_func_script_exists(job_number, func_script):
+            for k, v in job_dict.items():
+                if k == job_number:
+                    continue
+                if func_script == v[3]:
+                    return True
+            return False
+
+        job_list = self.get_job_list()
+        job_dict = {job[0]: job[1:] for job in job_list}
+        job = job_dict.get(job_number)
+        if job is None:
+            print(f"job ({job_number}) is not found.")
+            return
+        job_script = job[2]
+        func_script = job[3]
+        job_name = job_script[0:-7]
+        self.delete_file(f"{job_name}_job.sage")
+        self.delete_file(f"{job_name}.param")
+        self.delete_file(f"{job_name}.param.output")
+        if not is_same_func_script_exists(job_number, func_script):
+            self.delete_file(func_script)
+        # self.server.delete_build(self.project, job_number)
+        print("delete build job not implemented because of jenkins request error.")
+        return
+
+
+class JobStorm(JobStormPython):
+    def __init__(
+        self,
+        server_url=None,
+        username=None,
+        password=None,
+        shared_dir=SHRDIR,
+        project=PROJECT,
+        python_cmd=PYTCMD,
+        server_timeout=60,
+    ):
+        super().__init__(
+            server_url,
+            username,
+            password,
+            shared_dir,
+            project,
+            python_cmd,
+            server_timeout,
+        )
+
+    @classmethod
+    def python(
+        cls,
+        server_url=None,
+        username=None,
+        password=None,
+        shared_dir=SHRDIR,
+        project=PROJECT,
+        job_cmd=PYTCMD,
+        server_timeout=60,
+    ):
+        return JobStormPython(
+            server_url,
+            username,
+            password,
+            shared_dir,
+            project,
+            job_cmd,
+            server_timeout,
+        )
+
+    @classmethod
+    def sage(
+        cls,
+        server_url=None,
+        username=None,
+        password=None,
+        shared_dir=SHRDIR,
+        project=PROJECT,
+        job_cmd=SAGCMD,
+        server_timeout=60,
+    ):
+        return JobStormSage(
+            server_url,
+            username,
+            password,
+            shared_dir,
+            project,
+            job_cmd,
+            server_timeout,
+        )
```

## Comparing `jupyter_jobstorm-0.1.2.dist-info/LICENSE` & `jupyter_jobstorm-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupyter_jobstorm-0.1.2.dist-info/METADATA` & `jupyter_jobstorm-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: jupyter-jobstorm
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool to run a function written in Jupyter cell as a job
 Home-page: https://github.com/schrodingers-koala/jupyter-jobstorm
 Author: schrodingers-koala
 Author-email: schrodingers.koala@gmail.com
 License: MIT
-Keywords: jupyter-jobstorm jobstorm
-Platform: UNKNOWN
+Keywords: jupyter-jobstorm,jobstorm
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dill
 Requires-Dist: python-jenkins
 Requires-Dist: tabulate
 
@@ -33,15 +36,15 @@
 Please see examples for details.
 
 I believe that Jenkins will catch and execute jobs which are sent from you like the mighty storm on the planet Jupiter.
 
 ## Feature
 
 - Supporting Jenkins as job runner
-- Running a function (\*) of Python script as a job
+- Running a function (\*) of Python/SageMath script as a job
 - Retrieving the status and the result of the job
 
 (\*) Currently only variables of function arguments are passed to the function and variables outside of the function are not supported.
 
 ## Requirement
 
 - dill >= 0.3.5.1
@@ -57,14 +60,14 @@
 
 ```console
 $ pip install jupyter-jobstorm
 ```
 
 ## Usage
 
-- [Example 1: Job Test](https://github.com/schrodingers-koala/jupyter-jobstorm/blob/main/example/job_test.ipynb)
+- [Example 1: Python Job Test](https://github.com/schrodingers-koala/jupyter-jobstorm/blob/main/example/job_test.ipynb)
+
+- [Example 2: Sage Job Test](https://github.com/schrodingers-koala/jupyter-jobstorm/blob/main/example/sage_job_test.ipynb)
 
 ## License
 
 Jupyter-JobStorm is under MIT license.
-
-
```

