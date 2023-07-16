# Comparing `tmp/argtoolbox-1.1.4.tar.gz` & `tmp/argtoolbox-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/argtoolbox-1.1.4.tar", last modified: Sun Jun 13 19:45:47 2021, max compression
+gzip compressed data, was "argtoolbox-1.1.5.tar", last modified: Sun Jul 16 13:58:41 2023, max compression
```

## Comparing `argtoolbox-1.1.4.tar` & `argtoolbox-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-06-13 19:45:47.486963 argtoolbox-1.1.4/
--rw-rw-r--   0 fred      (1000) fred      (1000)    13386 2021-06-13 19:45:47.486963 argtoolbox-1.1.4/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)    10265 2019-10-13 12:16:20.000000 argtoolbox-1.1.4/README.rst
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-06-13 19:45:47.482963 argtoolbox-1.1.4/argtoolbox/
--rw-rw-r--   0 fred      (1000) fred      (1000)       49 2020-04-01 19:37:04.000000 argtoolbox-1.1.4/argtoolbox/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    51968 2021-06-04 21:22:13.000000 argtoolbox-1.1.4/argtoolbox/argtoolbox.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    13261 2020-02-15 15:44:55.000000 argtoolbox-1.1.4/argtoolbox/commands.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-06-13 19:45:47.486963 argtoolbox-1.1.4/argtoolbox/templates/
--rwxrwxr-x   0 fred      (1000) fred      (1000)     1800 2020-02-15 10:41:38.000000 argtoolbox-1.1.4/argtoolbox/templates/default.tml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-06-13 19:45:47.486963 argtoolbox-1.1.4/argtoolbox.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)    13386 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)      329 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 fred      (1000) fred      (1000)        1 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       61 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/entry_points.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       28 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/requires.txt
--rw-r--r--   0 fred      (1000) fred      (1000)       11 2021-06-13 19:45:47.000000 argtoolbox-1.1.4/argtoolbox.egg-info/top_level.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2021-06-13 19:45:47.486963 argtoolbox-1.1.4/setup.cfg
--rwxrwxr-x   0 fred      (1000) fred      (1000)     4946 2020-03-26 13:14:22.000000 argtoolbox-1.1.4/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-16 13:58:41.963613 argtoolbox-1.1.5/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35147 2022-04-30 15:14:59.000000 argtoolbox-1.1.5/LICENSE.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)    10925 2023-07-16 13:58:41.963613 argtoolbox-1.1.5/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)    10265 2022-04-30 15:14:59.000000 argtoolbox-1.1.5/README.rst
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-16 13:58:41.960280 argtoolbox-1.1.5/argtoolbox/
+-rw-r--r--   0 fred      (1000) fred      (1000)       49 2022-04-30 15:15:58.000000 argtoolbox-1.1.5/argtoolbox/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    51986 2023-07-16 13:54:25.000000 argtoolbox-1.1.5/argtoolbox/argtoolbox.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    13261 2022-04-30 15:14:59.000000 argtoolbox-1.1.5/argtoolbox/commands.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-16 13:58:41.963613 argtoolbox-1.1.5/argtoolbox/templates/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     1800 2022-01-15 02:09:18.000000 argtoolbox-1.1.5/argtoolbox/templates/default.tml
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-16 13:58:41.960280 argtoolbox-1.1.5/argtoolbox.egg-info/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)    10925 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/PKG-INFO
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      356 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/SOURCES.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/dependency_links.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       60 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/entry_points.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       28 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/requires.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       11 2023-07-16 13:58:41.000000 argtoolbox-1.1.5/argtoolbox.egg-info/top_level.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-07-16 13:58:41.963613 argtoolbox-1.1.5/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     4946 2022-01-15 02:09:18.000000 argtoolbox-1.1.5/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-16 13:58:41.963613 argtoolbox-1.1.5/tests/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     8019 2022-01-15 02:09:18.000000 argtoolbox-1.1.5/tests/tests.py
```

### Comparing `argtoolbox-1.1.4/PKG-INFO` & `argtoolbox-1.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: argtoolbox
-Version: 1.1.4
+Version: 1.1.5
 Summary: The easy way to create a short program with file options and command line options.
 Home-page: https://github.com/fred49/argtoolbox
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Description: Argtoolbox
-        ==========
-        
-        Description
-        -----------
-        
-        It helps to build a command line tool with argparse module.
-        It also use ConfigParser module to store default values into a
-        configuration file store in your profile.
-        
-        It checks the data type, if it is required, etc... without repeat your
-        constraint once for the config file, and another time for the cli parser.
-        Usefull trick, data store in the configuration file can be used as the
-        default value of the argparse argument.
-        
-        This lets you focus on the command you want to do, not the input processing
-        (cli or config file)
-        
-        Every program build with this tool have auto complete support on options and
-        arguments through argcomplete module.
-        
-        
-        Installation
-        ------------
-        
-        You can install this module using : ``pip install argtoolbox``.
-        
-        
-        QuickStart : Very Basic Usage
-        -----------------------------
-        
-        1. Imports :
-        ~~~~~~~~~~~~
-        
-        First of all, you just need the following classes to build your own script :
-        
-        * **DefaultCommand :** The default class to extend in order to create your own
-          command class.
-        
-        * **BasicProgram :** The most simple program to run your command classes.
-        
-        
-        2. Declaration :
-        ~~~~~~~~~~~~~~~~
-        
-        There is a script called sample-program.py which contains all the following
-        lines of code.
-        
-        1. First you have to create your command class TestCommand. (**Step 1**)
-        2. In the ``__call__`` method, you can do every thing you want. The first and only
-           arg of this method is the args object created by Argparse.parser. (**Step 2**)
-        3. You create an other class MyProgram (which extends the BasicProgram) (**Step 3**)
-        4. Now you create your  ``argparse.parser`` and your declare your argument, option and command. (**Step 4**)
-        5. Finally you just have to instanciate your class MyProgram and run it. (**Step 5**).
-        
-        
-        .. code-block:: python
-        
-            #! /usr/bin/env python2
-            # -*- coding: utf-8 -*-
-            # PYTHON_ARGCOMPLETE_OK
-        
-        
-            from argtoolbox import DefaultCommand
-            from argtoolbox import BasicProgram
-        
-            # Step 1
-            class TestCommand(DefaultCommand):
-                """Just a simple command, using the default command class.
-                It will print the inputs args to stdout"""
-        
-                def __call__(self, args):
-                    super(TestCommand, self).__call__(args)
-                    # Step 2
-                    print ""
-                    print "This is the beginning of the TestCommand class."
-                    print "The command line arguments (argv) :"
-                    print "-----------------------------------"
-                    print ""
-                    print "This is the end of the TestCommand class."
-                    print ""
-        
-            # Step 3
-            class MyProgram(BasicProgram):
-        
-                def add_commands(self):
-                    # Step 4
-                    subparsers = self.parser.add_subparsers()
-                    parser_tmp = subparsers.add_parser(
-                        'test',
-                        help="This command will print cli argv and configuration read \
-                        from the config file.")
-                    parser_tmp.add_argument('--host', required=True)
-                    parser_tmp.add_argument('--port', default=3000)
-                    parser_tmp.set_defaults(__func__=TestCommand(self.config))
-        
-        
-            # Step 5
-            if __name__ == "__main__":
-        
-                PROG = MyProgram("sample-program",
-                                    desc="""Just a description for a sample program.""")
-                PROG()
-        
-        
-        
-        3. Utilisation :
-        ~~~~~~~~~~~~~~~~
-        
-        Now you can show the help menu using the following command :
-        
-        ``$ ./sample-program.py test -h``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            usage: sample-program test [-h] --host HOST [--port PORT]
-        
-            optional arguments:
-              -h, --help   show this help message and exit
-              --host HOST
-              --port PORT
-        
-        Or run your command :
-        
-        ``$  ./sample-program.py test --host 127.0.0.1``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            This is the beginning of the TestCommand class.
-            The command line arguments (argv) :
-            -----------------------------------
-            Namespace(__func__=<__main__.TestCommand object at 0xb721a92c>,
-            config_file=None, host='127.0.0.1', port=3000, verbose=False)
-        
-            This is the end of the TestCommand class.
-        
-        You can see the variable ``host`` contains the input message ``127.0.0.1`` into the
-        args object.
-        The option ``port`` contains the default value ``3000``.
-        
-        
-        Advanced usage
-        --------------
-        
-        At this point, this program does not do much more than the argparse module can
-        do.
-        In the cas you have a lot of command and option, it could be usefull to store
-        default values in a configuration file like ``sample-program.cfg``
-        
-        
-        4. Imports :
-        ~~~~~~~~~~~~
-        
-        First of all, you just need the following classes to build your own script :
-        
-        * **TestCommand :** This command class will print to stdout the inputs args and
-          the configuration file content.
-        
-        * **BasicProgram :** The most simple program to run your command classes.
-        
-        * **SimpleSection :** This class is used to declare a Section in the config file
-          (ConfigFile)
-        
-        * **Element :** This class is used to declare an Option (a field) in the
-          previous section.
-        
-        * **Base64ElementHook :** This hook is used as a post reading processing in
-          order to convert base64 data stored into the config file into plain text data.
-        
-        
-        
-        5. Declaration :
-        ~~~~~~~~~~~~~~~~
-        
-        There is a script called sample-program2.py which contains all the following
-        lines of code.
-        
-        
-        #. Instead of creating a config file, we will use an in-memory config file
-           (**Step 1**)
-        #. You create an other class MyProgram (which extends the BasicProgram) (**Step
-           2**)
-        #. We override the default method called ``add_config_options``. (**Step 3**)
-        #. We declare the section named ``ldap`` that we are looking for.
-        #. We declare all the fields store into the previous section. For each fied, you can says if it is required, the default value, the type, an optional description. See the documentatino for more details. (**Step 5**).
-        #. The we declare all argparse arguments using the previous configuration declaration. This is very usefull because the data store into the configuration file are used as the default value for the argparse argument. The description, the type, required or not, ... declared in the ``add_config_options`` method are used to configure the parser argument. No need to repeat your self. (**Step 6**)
-        #. Declaration of the ``test`` argument using TestCommand class. (**Step 7**)
-        #. Finally you just have to instanciate your class MyProgram, the first argument is the program name. (**Step 8**)
-        #. We override the default config file name ``'.<program name>.cfg'``. (**Step 9**)
-        #. We launch the program. (**Step 10**)
-        
-        
-        .. code-block:: python
-        
-            #! /usr/bin/env python2
-            # -*- coding: utf-8 -*-
-            # PYTHON_ARGCOMPLETE_OK
-        
-            import io
-            from argtoolbox import TestCommand
-            from argtoolbox import BasicProgram
-            from argtoolbox import SimpleSection, Element, Base64ElementHook
-        
-            # Step 1
-            SAMPLE_CONFIG = """
-            [ldap]
-        
-            host=127.0.0.1
-            port=389
-            suffix=dc=nodomain
-            account=cn=admin,dc=nodomain
-            password=toto
-        
-            \n"""
-        
-            # Step 2
-            class MyProgram(BasicProgram):
-        
-                # Step 3
-                def add_config_options(self):
-                    # Step 4
-                    # section ldap
-                    section_ldap = self.config.add_section(SimpleSection("ldap"))
-                    # Step 5
-                    section_ldap.add_element(Element('debug',
-                                                     e_type=int,
-                                                     default=0,
-                                                     desc="""debug level : default : 0."""))
-                    section_ldap.add_element(Element('host',
-                                                     required=True,
-                                                     default="192.168.1.1"))
-                    section_ldap.add_element(Element('account', required=True))
-                    section_ldap.add_element(Element('port', e_type=int))
-                    section_ldap.add_element(Element('password',
-                                                     required=True,
-                                                     hidden=True,
-                                                     desc="account password to ldap",
-                                                     hooks=[Base64ElementHook(), ]))
-        
-               def add_commands(self):
-                    # Step 6
-                    self.parser.add_argument(
-                        '--host', **self.config.ldap.host.get_arg_parse_arguments())
-                    self.parser.add_argument(
-                        '--port', **self.config.ldap.port.get_arg_parse_arguments())
-                    self.parser.add_argument(
-                        '-d',
-                        action="count",
-                        **self.config.ldap.debug.get_arg_parse_arguments())
-        
-                    # Step 7
-                    subparsers = self.parser.add_subparsers()
-                    parser_tmp = subparsers.add_parser(
-                        'test',
-                        help="This simple command print cli argv and configuration read \
-                        form config file.")
-                    parser_tmp.set_defaults(__func__=TestCommand(self.config))
-        
-        
-            if __name__ ≡ "__main__":
-        
-                # Step 8
-                PROG = MyProgram("sample-program",
-                    # Step 9
-                                 config_file=io.BytesIO(SAMPLE_CONFIG),
-                                 desc="""Just a description for a sample program.""")
-                # Step 10
-                PROG()
-        
-        6. Utilisation :
-        ~~~~~~~~~~~~~~~~
-        
-        Now you can run your command :
-        
-        ``$ ./sample-program2.py --host an.other.host.com test``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            This is the beginning of the TestCommand class.
-        
-            The loaded configuration :
-            ---------------------------
-            Configuration of sample-program :
-        
-                    Section LDAP
-                     - debug : 0
-                     - host : 127.0.0.1
-                     - account : cn=admin,dc=nodomain
-                     - port : 389
-                     - password : xxxxxxxx
-        
-        
-            The command line arguments (argv) :
-            ------------------------------------
-            Namespace(__func__=<argtoolbox.argtoolbox.TestCommand object at 0xb7199f8c>, config_file=None, debug=0, host='an.other.host.com', port=389, verbose=False)
-        
-            This is the end of the TestCommand class.
-        
-        You can see the variable ``host`` contains the input message ``an.other.host.com`` into the
-        args object. The option ``port`` contains the default value ``389``.
-        You can also acces to the values store into the configuration file like ``account`` or ``password`` which can not be override by the CLI.
-        
 Keywords: argparse ConfigFile command line interface
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.txt
+
+Argtoolbox
+==========
+
+Description
+-----------
+
+It helps to build a command line tool with argparse module.
+It also use ConfigParser module to store default values into a
+configuration file store in your profile.
+
+It checks the data type, if it is required, etc... without repeat your
+constraint once for the config file, and another time for the cli parser.
+Usefull trick, data store in the configuration file can be used as the
+default value of the argparse argument.
+
+This lets you focus on the command you want to do, not the input processing
+(cli or config file)
+
+Every program build with this tool have auto complete support on options and
+arguments through argcomplete module.
+
+
+Installation
+------------
+
+You can install this module using : ``pip install argtoolbox``.
+
+
+QuickStart : Very Basic Usage
+-----------------------------
+
+1. Imports :
+~~~~~~~~~~~~
+
+First of all, you just need the following classes to build your own script :
+
+* **DefaultCommand :** The default class to extend in order to create your own
+  command class.
+
+* **BasicProgram :** The most simple program to run your command classes.
+
+
+2. Declaration :
+~~~~~~~~~~~~~~~~
+
+There is a script called sample-program.py which contains all the following
+lines of code.
+
+1. First you have to create your command class TestCommand. (**Step 1**)
+2. In the ``__call__`` method, you can do every thing you want. The first and only
+   arg of this method is the args object created by Argparse.parser. (**Step 2**)
+3. You create an other class MyProgram (which extends the BasicProgram) (**Step 3**)
+4. Now you create your  ``argparse.parser`` and your declare your argument, option and command. (**Step 4**)
+5. Finally you just have to instanciate your class MyProgram and run it. (**Step 5**).
+
+
+.. code-block:: python
+
+    #! /usr/bin/env python2
+    # -*- coding: utf-8 -*-
+    # PYTHON_ARGCOMPLETE_OK
+
+
+    from argtoolbox import DefaultCommand
+    from argtoolbox import BasicProgram
+
+    # Step 1
+    class TestCommand(DefaultCommand):
+        """Just a simple command, using the default command class.
+        It will print the inputs args to stdout"""
+
+        def __call__(self, args):
+            super(TestCommand, self).__call__(args)
+            # Step 2
+            print ""
+            print "This is the beginning of the TestCommand class."
+            print "The command line arguments (argv) :"
+            print "-----------------------------------"
+            print ""
+            print "This is the end of the TestCommand class."
+            print ""
+
+    # Step 3
+    class MyProgram(BasicProgram):
+
+        def add_commands(self):
+            # Step 4
+            subparsers = self.parser.add_subparsers()
+            parser_tmp = subparsers.add_parser(
+                'test',
+                help="This command will print cli argv and configuration read \
+                from the config file.")
+            parser_tmp.add_argument('--host', required=True)
+            parser_tmp.add_argument('--port', default=3000)
+            parser_tmp.set_defaults(__func__=TestCommand(self.config))
+
+
+    # Step 5
+    if __name__ == "__main__":
+
+        PROG = MyProgram("sample-program",
+                            desc="""Just a description for a sample program.""")
+        PROG()
+
+
+
+3. Utilisation :
+~~~~~~~~~~~~~~~~
+
+Now you can show the help menu using the following command :
+
+``$ ./sample-program.py test -h``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    usage: sample-program test [-h] --host HOST [--port PORT]
+
+    optional arguments:
+      -h, --help   show this help message and exit
+      --host HOST
+      --port PORT
+
+Or run your command :
+
+``$  ./sample-program.py test --host 127.0.0.1``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    This is the beginning of the TestCommand class.
+    The command line arguments (argv) :
+    -----------------------------------
+    Namespace(__func__=<__main__.TestCommand object at 0xb721a92c>,
+    config_file=None, host='127.0.0.1', port=3000, verbose=False)
+
+    This is the end of the TestCommand class.
+
+You can see the variable ``host`` contains the input message ``127.0.0.1`` into the
+args object.
+The option ``port`` contains the default value ``3000``.
+
+
+Advanced usage
+--------------
+
+At this point, this program does not do much more than the argparse module can
+do.
+In the cas you have a lot of command and option, it could be usefull to store
+default values in a configuration file like ``sample-program.cfg``
+
+
+4. Imports :
+~~~~~~~~~~~~
+
+First of all, you just need the following classes to build your own script :
+
+* **TestCommand :** This command class will print to stdout the inputs args and
+  the configuration file content.
+
+* **BasicProgram :** The most simple program to run your command classes.
+
+* **SimpleSection :** This class is used to declare a Section in the config file
+  (ConfigFile)
+
+* **Element :** This class is used to declare an Option (a field) in the
+  previous section.
+
+* **Base64ElementHook :** This hook is used as a post reading processing in
+  order to convert base64 data stored into the config file into plain text data.
+
+
+
+5. Declaration :
+~~~~~~~~~~~~~~~~
+
+There is a script called sample-program2.py which contains all the following
+lines of code.
+
+
+#. Instead of creating a config file, we will use an in-memory config file
+   (**Step 1**)
+#. You create an other class MyProgram (which extends the BasicProgram) (**Step
+   2**)
+#. We override the default method called ``add_config_options``. (**Step 3**)
+#. We declare the section named ``ldap`` that we are looking for.
+#. We declare all the fields store into the previous section. For each fied, you can says if it is required, the default value, the type, an optional description. See the documentatino for more details. (**Step 5**).
+#. The we declare all argparse arguments using the previous configuration declaration. This is very usefull because the data store into the configuration file are used as the default value for the argparse argument. The description, the type, required or not, ... declared in the ``add_config_options`` method are used to configure the parser argument. No need to repeat your self. (**Step 6**)
+#. Declaration of the ``test`` argument using TestCommand class. (**Step 7**)
+#. Finally you just have to instanciate your class MyProgram, the first argument is the program name. (**Step 8**)
+#. We override the default config file name ``'.<program name>.cfg'``. (**Step 9**)
+#. We launch the program. (**Step 10**)
+
+
+.. code-block:: python
+
+    #! /usr/bin/env python2
+    # -*- coding: utf-8 -*-
+    # PYTHON_ARGCOMPLETE_OK
+
+    import io
+    from argtoolbox import TestCommand
+    from argtoolbox import BasicProgram
+    from argtoolbox import SimpleSection, Element, Base64ElementHook
+
+    # Step 1
+    SAMPLE_CONFIG = """
+    [ldap]
+
+    host=127.0.0.1
+    port=389
+    suffix=dc=nodomain
+    account=cn=admin,dc=nodomain
+    password=toto
+
+    \n"""
+
+    # Step 2
+    class MyProgram(BasicProgram):
+
+        # Step 3
+        def add_config_options(self):
+            # Step 4
+            # section ldap
+            section_ldap = self.config.add_section(SimpleSection("ldap"))
+            # Step 5
+            section_ldap.add_element(Element('debug',
+                                             e_type=int,
+                                             default=0,
+                                             desc="""debug level : default : 0."""))
+            section_ldap.add_element(Element('host',
+                                             required=True,
+                                             default="192.168.1.1"))
+            section_ldap.add_element(Element('account', required=True))
+            section_ldap.add_element(Element('port', e_type=int))
+            section_ldap.add_element(Element('password',
+                                             required=True,
+                                             hidden=True,
+                                             desc="account password to ldap",
+                                             hooks=[Base64ElementHook(), ]))
+
+       def add_commands(self):
+            # Step 6
+            self.parser.add_argument(
+                '--host', **self.config.ldap.host.get_arg_parse_arguments())
+            self.parser.add_argument(
+                '--port', **self.config.ldap.port.get_arg_parse_arguments())
+            self.parser.add_argument(
+                '-d',
+                action="count",
+                **self.config.ldap.debug.get_arg_parse_arguments())
+
+            # Step 7
+            subparsers = self.parser.add_subparsers()
+            parser_tmp = subparsers.add_parser(
+                'test',
+                help="This simple command print cli argv and configuration read \
+                form config file.")
+            parser_tmp.set_defaults(__func__=TestCommand(self.config))
+
+
+    if __name__ ≡ "__main__":
+
+        # Step 8
+        PROG = MyProgram("sample-program",
+            # Step 9
+                         config_file=io.BytesIO(SAMPLE_CONFIG),
+                         desc="""Just a description for a sample program.""")
+        # Step 10
+        PROG()
+
+6. Utilisation :
+~~~~~~~~~~~~~~~~
+
+Now you can run your command :
+
+``$ ./sample-program2.py --host an.other.host.com test``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    This is the beginning of the TestCommand class.
+
+    The loaded configuration :
+    ---------------------------
+    Configuration of sample-program :
+
+            Section LDAP
+             - debug : 0
+             - host : 127.0.0.1
+             - account : cn=admin,dc=nodomain
+             - port : 389
+             - password : xxxxxxxx
+
+
+    The command line arguments (argv) :
+    ------------------------------------
+    Namespace(__func__=<argtoolbox.argtoolbox.TestCommand object at 0xb7199f8c>, config_file=None, debug=0, host='an.other.host.com', port=389, verbose=False)
+
+    This is the end of the TestCommand class.
+
+You can see the variable ``host`` contains the input message ``an.other.host.com`` into the
+args object. The option ``port`` contains the default value ``389``.
+You can also acces to the values store into the configuration file like ``account`` or ``password`` which can not be override by the CLI.
```

### Comparing `argtoolbox-1.1.4/README.rst` & `argtoolbox-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `argtoolbox-1.1.4/argtoolbox/argtoolbox.py` & `argtoolbox-1.1.5/argtoolbox/argtoolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,47 +22,45 @@
 #
 # Contributors list:
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
-
 import os
 import sys
 import logging
 import base64
 import copy
 import binascii
 from collections import OrderedDict
 import configparser
 import argparse
 from argparse import ArgumentError
 
 # global logger variable
-#log = logging.getLogger('argtoolbox')
-#log.setLevel(logging.INFO)
-#log.setLevel(logging.DEBUG)
+# log = logging.getLogger('argtoolbox')
+# log.setLevel(logging.INFO)
+# log.setLevel(logging.DEBUG)
 # logger formats
 DEFAULT_LOGGING_FORMAT = logging.Formatter(
     "%(asctime)s %(levelname)-8s: %(message)s", "%H:%M:%S")
 DEBUG_LOGGING_FORMAT = logging.Formatter(
-    "%(asctime)s %(levelname)-8s %(module)s:%(name)s:%(funcName)s:%(lineno)d:%(message)s",
-    "%H:%M:%S")
+    "%(asctime)s %(levelname)-8s %(module)s:%(name)s:%(funcName)s:%(lineno)d:%(message)s")
 # logger handlers
 # pylint: disable-msg=C0103
 streamHandler = logging.StreamHandler(sys.stdout)
 streamHandler.setFormatter(DEFAULT_LOGGING_FORMAT)
 
 # debug mode
 # if you need debug during class construction, file config loading, ...,
 # you need to modify the logger level here.
-#log.addHandler(streamHandler)
-#log.setLevel(logging.DEBUG)
-#streamHandler.setFormatter(DEBUG_LOGGING_FORMAT)
+# log.addHandler(streamHandler)
+# log.setLevel(logging.DEBUG)
+# streamHandler.setFormatter(DEBUG_LOGGING_FORMAT)
 
 
 class DefaultHook:
     """
     This class does nothing. This is the default class for creating your own
     hook. After reading an option from the config file, you can apply a
     postprocessing, like the base64 decoding or every thing you want.
@@ -254,15 +252,15 @@
         from the command line interface.
         1. pasing arguments
         2. applying hooks
         3. addding help argument
         4. reloading configuration using cli argument like a configuration
         file name.
         """
-        #from argcomplete import debug
+        # from argcomplete import debug
         # Parsing the command line looking for the previous options like
         # configuration file name or server section. Extra arguments
         # will be store into argv.
         args = None
 
         if os.environ.get('_ARGCOMPLETE'):
             # During argcomplete completion, parse_known_args will return an
@@ -360,14 +358,15 @@
         self._suffix = suffix
         self._required = required
 
     @property
     def name(self):
         """This method will return the name of the current element"""
         return self._name
+
     @name.setter
     def name(self, name):
         """TODO"""
         self._name = name
 
     def get_key_name(self):
         """This method return the name of the section, it Should be unique
@@ -707,15 +706,15 @@
 
     def __str__(self):
         return "".join(self.get_representation())
 
     def __copy__(self):
         newone = type(self)(self._name)
         newone.__dict__.update(self.__dict__)
-        #self.elements = OrderedDict()
+        # self.elements = OrderedDict()
         return newone
 
     def post_load(self):
         """Every element hooks are applied by this method, just after the
         loading process.
         """
         for h in self.hooks:
@@ -770,15 +769,15 @@
                     msg = "Data type not supported : %(type)s " % {
                         "type": self.e_type}
                     log.error(msg)
                     raise TypeError(msg)
 
             except ValueError as ex:
                 msg = "The current field '%(name)s' was present, but the \
-required type is : %(e_type)s." %  {
+required type is : %(e_type)s." % {
                 "name": self._name,
                 "e_type": self.e_type
                 }
                 log.error(msg)
                 log.error(str(ex))
                 raise ValueError(str(ex))
 
@@ -1075,15 +1074,15 @@
         self.protected_args = ['password']
 
     def __call__(self, args):
         self._log_namespace(args)
 
     def _log_namespace(self, args):
         dict_tmp = copy.copy(args)
-        #delattr(dict_tmp, "__func__")
+        # delattr(dict_tmp, "__func__")
         for field in getattr(self, 'protected_args', []):
             if hasattr(dict_tmp, field):
                 setattr(dict_tmp, field, "xxxxxxxx")
         self.log.debug("Namespace : begin :")
         for i in sorted(dict_tmp.__dict__):
             attribute = getattr(dict_tmp, i)
             self.log.debug("%s : %s : %s", i, attribute, type(attribute))
@@ -1135,16 +1134,16 @@
             debug("Kwargs content :")
             for i, j in list(kwargs.items()):
                 debug("key : " + str(i))
                 debug("\t - " + str(j))
 
             args = kwargs.get('parsed_args')
             # pylint: disable-msg=W0612
-            parser = kwargs.get('parser')
-            #a = parser.parse_known_args()
+            # parser = kwargs.get('parser')
+            # a = parser.parse_known_args()
 
             # getting form args the current Command and looking for a method
             # called by default 'complete'. See __init__ method. The method
             # name is store in the class member called self.func_name
             debug("-------")
             debug("__func__:" + str(args.__func__))
             debug("func_name:" + str(self.func_name))
@@ -1240,27 +1239,27 @@
             return args.__func__(args)
         else:
             # pylint: disable-msg=W0621
             log = logging.getLogger('argtoolbox')
             try:
                 # run command
                 if not hasattr(args, '__func__'):
-                    self.parser.error("You must provide a command. See --help.")
+                    self.parser.error(
+                            "You must provide a command. See --help.")
                 return args.__func__(args)
             except ValueError as a:
                 log.error("ValueError : " + str(a))
-            except KeyboardInterrupt as a:
+            except KeyboardInterrupt:
                 log.warn("Keyboard interruption detected.")
             except ArgumentError as a:
                 self.parser.error(a.message)
             except Exception as a:
                 log.error("unexcepted error : " + str(a))
             return False
 
-
     def parse_args(self):
         args = self.parser.parse_args()
         for attr in args.__dict__:
             data = getattr(args, attr)
             if isinstance(data, str):
                 setattr(args, attr, data)
```

### Comparing `argtoolbox-1.1.4/argtoolbox/commands.py` & `argtoolbox-1.1.5/argtoolbox/commands.py`

 * *Files identical despite different names*

### Comparing `argtoolbox-1.1.4/argtoolbox/templates/default.tml` & `argtoolbox-1.1.5/argtoolbox/templates/default.tml`

 * *Files identical despite different names*

### Comparing `argtoolbox-1.1.4/argtoolbox.egg-info/PKG-INFO` & `argtoolbox-1.1.5/argtoolbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: argtoolbox
-Version: 1.1.4
+Version: 1.1.5
 Summary: The easy way to create a short program with file options and command line options.
 Home-page: https://github.com/fred49/argtoolbox
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Description: Argtoolbox
-        ==========
-        
-        Description
-        -----------
-        
-        It helps to build a command line tool with argparse module.
-        It also use ConfigParser module to store default values into a
-        configuration file store in your profile.
-        
-        It checks the data type, if it is required, etc... without repeat your
-        constraint once for the config file, and another time for the cli parser.
-        Usefull trick, data store in the configuration file can be used as the
-        default value of the argparse argument.
-        
-        This lets you focus on the command you want to do, not the input processing
-        (cli or config file)
-        
-        Every program build with this tool have auto complete support on options and
-        arguments through argcomplete module.
-        
-        
-        Installation
-        ------------
-        
-        You can install this module using : ``pip install argtoolbox``.
-        
-        
-        QuickStart : Very Basic Usage
-        -----------------------------
-        
-        1. Imports :
-        ~~~~~~~~~~~~
-        
-        First of all, you just need the following classes to build your own script :
-        
-        * **DefaultCommand :** The default class to extend in order to create your own
-          command class.
-        
-        * **BasicProgram :** The most simple program to run your command classes.
-        
-        
-        2. Declaration :
-        ~~~~~~~~~~~~~~~~
-        
-        There is a script called sample-program.py which contains all the following
-        lines of code.
-        
-        1. First you have to create your command class TestCommand. (**Step 1**)
-        2. In the ``__call__`` method, you can do every thing you want. The first and only
-           arg of this method is the args object created by Argparse.parser. (**Step 2**)
-        3. You create an other class MyProgram (which extends the BasicProgram) (**Step 3**)
-        4. Now you create your  ``argparse.parser`` and your declare your argument, option and command. (**Step 4**)
-        5. Finally you just have to instanciate your class MyProgram and run it. (**Step 5**).
-        
-        
-        .. code-block:: python
-        
-            #! /usr/bin/env python2
-            # -*- coding: utf-8 -*-
-            # PYTHON_ARGCOMPLETE_OK
-        
-        
-            from argtoolbox import DefaultCommand
-            from argtoolbox import BasicProgram
-        
-            # Step 1
-            class TestCommand(DefaultCommand):
-                """Just a simple command, using the default command class.
-                It will print the inputs args to stdout"""
-        
-                def __call__(self, args):
-                    super(TestCommand, self).__call__(args)
-                    # Step 2
-                    print ""
-                    print "This is the beginning of the TestCommand class."
-                    print "The command line arguments (argv) :"
-                    print "-----------------------------------"
-                    print ""
-                    print "This is the end of the TestCommand class."
-                    print ""
-        
-            # Step 3
-            class MyProgram(BasicProgram):
-        
-                def add_commands(self):
-                    # Step 4
-                    subparsers = self.parser.add_subparsers()
-                    parser_tmp = subparsers.add_parser(
-                        'test',
-                        help="This command will print cli argv and configuration read \
-                        from the config file.")
-                    parser_tmp.add_argument('--host', required=True)
-                    parser_tmp.add_argument('--port', default=3000)
-                    parser_tmp.set_defaults(__func__=TestCommand(self.config))
-        
-        
-            # Step 5
-            if __name__ == "__main__":
-        
-                PROG = MyProgram("sample-program",
-                                    desc="""Just a description for a sample program.""")
-                PROG()
-        
-        
-        
-        3. Utilisation :
-        ~~~~~~~~~~~~~~~~
-        
-        Now you can show the help menu using the following command :
-        
-        ``$ ./sample-program.py test -h``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            usage: sample-program test [-h] --host HOST [--port PORT]
-        
-            optional arguments:
-              -h, --help   show this help message and exit
-              --host HOST
-              --port PORT
-        
-        Or run your command :
-        
-        ``$  ./sample-program.py test --host 127.0.0.1``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            This is the beginning of the TestCommand class.
-            The command line arguments (argv) :
-            -----------------------------------
-            Namespace(__func__=<__main__.TestCommand object at 0xb721a92c>,
-            config_file=None, host='127.0.0.1', port=3000, verbose=False)
-        
-            This is the end of the TestCommand class.
-        
-        You can see the variable ``host`` contains the input message ``127.0.0.1`` into the
-        args object.
-        The option ``port`` contains the default value ``3000``.
-        
-        
-        Advanced usage
-        --------------
-        
-        At this point, this program does not do much more than the argparse module can
-        do.
-        In the cas you have a lot of command and option, it could be usefull to store
-        default values in a configuration file like ``sample-program.cfg``
-        
-        
-        4. Imports :
-        ~~~~~~~~~~~~
-        
-        First of all, you just need the following classes to build your own script :
-        
-        * **TestCommand :** This command class will print to stdout the inputs args and
-          the configuration file content.
-        
-        * **BasicProgram :** The most simple program to run your command classes.
-        
-        * **SimpleSection :** This class is used to declare a Section in the config file
-          (ConfigFile)
-        
-        * **Element :** This class is used to declare an Option (a field) in the
-          previous section.
-        
-        * **Base64ElementHook :** This hook is used as a post reading processing in
-          order to convert base64 data stored into the config file into plain text data.
-        
-        
-        
-        5. Declaration :
-        ~~~~~~~~~~~~~~~~
-        
-        There is a script called sample-program2.py which contains all the following
-        lines of code.
-        
-        
-        #. Instead of creating a config file, we will use an in-memory config file
-           (**Step 1**)
-        #. You create an other class MyProgram (which extends the BasicProgram) (**Step
-           2**)
-        #. We override the default method called ``add_config_options``. (**Step 3**)
-        #. We declare the section named ``ldap`` that we are looking for.
-        #. We declare all the fields store into the previous section. For each fied, you can says if it is required, the default value, the type, an optional description. See the documentatino for more details. (**Step 5**).
-        #. The we declare all argparse arguments using the previous configuration declaration. This is very usefull because the data store into the configuration file are used as the default value for the argparse argument. The description, the type, required or not, ... declared in the ``add_config_options`` method are used to configure the parser argument. No need to repeat your self. (**Step 6**)
-        #. Declaration of the ``test`` argument using TestCommand class. (**Step 7**)
-        #. Finally you just have to instanciate your class MyProgram, the first argument is the program name. (**Step 8**)
-        #. We override the default config file name ``'.<program name>.cfg'``. (**Step 9**)
-        #. We launch the program. (**Step 10**)
-        
-        
-        .. code-block:: python
-        
-            #! /usr/bin/env python2
-            # -*- coding: utf-8 -*-
-            # PYTHON_ARGCOMPLETE_OK
-        
-            import io
-            from argtoolbox import TestCommand
-            from argtoolbox import BasicProgram
-            from argtoolbox import SimpleSection, Element, Base64ElementHook
-        
-            # Step 1
-            SAMPLE_CONFIG = """
-            [ldap]
-        
-            host=127.0.0.1
-            port=389
-            suffix=dc=nodomain
-            account=cn=admin,dc=nodomain
-            password=toto
-        
-            \n"""
-        
-            # Step 2
-            class MyProgram(BasicProgram):
-        
-                # Step 3
-                def add_config_options(self):
-                    # Step 4
-                    # section ldap
-                    section_ldap = self.config.add_section(SimpleSection("ldap"))
-                    # Step 5
-                    section_ldap.add_element(Element('debug',
-                                                     e_type=int,
-                                                     default=0,
-                                                     desc="""debug level : default : 0."""))
-                    section_ldap.add_element(Element('host',
-                                                     required=True,
-                                                     default="192.168.1.1"))
-                    section_ldap.add_element(Element('account', required=True))
-                    section_ldap.add_element(Element('port', e_type=int))
-                    section_ldap.add_element(Element('password',
-                                                     required=True,
-                                                     hidden=True,
-                                                     desc="account password to ldap",
-                                                     hooks=[Base64ElementHook(), ]))
-        
-               def add_commands(self):
-                    # Step 6
-                    self.parser.add_argument(
-                        '--host', **self.config.ldap.host.get_arg_parse_arguments())
-                    self.parser.add_argument(
-                        '--port', **self.config.ldap.port.get_arg_parse_arguments())
-                    self.parser.add_argument(
-                        '-d',
-                        action="count",
-                        **self.config.ldap.debug.get_arg_parse_arguments())
-        
-                    # Step 7
-                    subparsers = self.parser.add_subparsers()
-                    parser_tmp = subparsers.add_parser(
-                        'test',
-                        help="This simple command print cli argv and configuration read \
-                        form config file.")
-                    parser_tmp.set_defaults(__func__=TestCommand(self.config))
-        
-        
-            if __name__ ≡ "__main__":
-        
-                # Step 8
-                PROG = MyProgram("sample-program",
-                    # Step 9
-                                 config_file=io.BytesIO(SAMPLE_CONFIG),
-                                 desc="""Just a description for a sample program.""")
-                # Step 10
-                PROG()
-        
-        6. Utilisation :
-        ~~~~~~~~~~~~~~~~
-        
-        Now you can run your command :
-        
-        ``$ ./sample-program2.py --host an.other.host.com test``
-        
-        **Console ouput :**
-        
-        .. code-block:: python
-        
-            This is the beginning of the TestCommand class.
-        
-            The loaded configuration :
-            ---------------------------
-            Configuration of sample-program :
-        
-                    Section LDAP
-                     - debug : 0
-                     - host : 127.0.0.1
-                     - account : cn=admin,dc=nodomain
-                     - port : 389
-                     - password : xxxxxxxx
-        
-        
-            The command line arguments (argv) :
-            ------------------------------------
-            Namespace(__func__=<argtoolbox.argtoolbox.TestCommand object at 0xb7199f8c>, config_file=None, debug=0, host='an.other.host.com', port=389, verbose=False)
-        
-            This is the end of the TestCommand class.
-        
-        You can see the variable ``host`` contains the input message ``an.other.host.com`` into the
-        args object. The option ``port`` contains the default value ``389``.
-        You can also acces to the values store into the configuration file like ``account`` or ``password`` which can not be override by the CLI.
-        
 Keywords: argparse ConfigFile command line interface
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.txt
+
+Argtoolbox
+==========
+
+Description
+-----------
+
+It helps to build a command line tool with argparse module.
+It also use ConfigParser module to store default values into a
+configuration file store in your profile.
+
+It checks the data type, if it is required, etc... without repeat your
+constraint once for the config file, and another time for the cli parser.
+Usefull trick, data store in the configuration file can be used as the
+default value of the argparse argument.
+
+This lets you focus on the command you want to do, not the input processing
+(cli or config file)
+
+Every program build with this tool have auto complete support on options and
+arguments through argcomplete module.
+
+
+Installation
+------------
+
+You can install this module using : ``pip install argtoolbox``.
+
+
+QuickStart : Very Basic Usage
+-----------------------------
+
+1. Imports :
+~~~~~~~~~~~~
+
+First of all, you just need the following classes to build your own script :
+
+* **DefaultCommand :** The default class to extend in order to create your own
+  command class.
+
+* **BasicProgram :** The most simple program to run your command classes.
+
+
+2. Declaration :
+~~~~~~~~~~~~~~~~
+
+There is a script called sample-program.py which contains all the following
+lines of code.
+
+1. First you have to create your command class TestCommand. (**Step 1**)
+2. In the ``__call__`` method, you can do every thing you want. The first and only
+   arg of this method is the args object created by Argparse.parser. (**Step 2**)
+3. You create an other class MyProgram (which extends the BasicProgram) (**Step 3**)
+4. Now you create your  ``argparse.parser`` and your declare your argument, option and command. (**Step 4**)
+5. Finally you just have to instanciate your class MyProgram and run it. (**Step 5**).
+
+
+.. code-block:: python
+
+    #! /usr/bin/env python2
+    # -*- coding: utf-8 -*-
+    # PYTHON_ARGCOMPLETE_OK
+
+
+    from argtoolbox import DefaultCommand
+    from argtoolbox import BasicProgram
+
+    # Step 1
+    class TestCommand(DefaultCommand):
+        """Just a simple command, using the default command class.
+        It will print the inputs args to stdout"""
+
+        def __call__(self, args):
+            super(TestCommand, self).__call__(args)
+            # Step 2
+            print ""
+            print "This is the beginning of the TestCommand class."
+            print "The command line arguments (argv) :"
+            print "-----------------------------------"
+            print ""
+            print "This is the end of the TestCommand class."
+            print ""
+
+    # Step 3
+    class MyProgram(BasicProgram):
+
+        def add_commands(self):
+            # Step 4
+            subparsers = self.parser.add_subparsers()
+            parser_tmp = subparsers.add_parser(
+                'test',
+                help="This command will print cli argv and configuration read \
+                from the config file.")
+            parser_tmp.add_argument('--host', required=True)
+            parser_tmp.add_argument('--port', default=3000)
+            parser_tmp.set_defaults(__func__=TestCommand(self.config))
+
+
+    # Step 5
+    if __name__ == "__main__":
+
+        PROG = MyProgram("sample-program",
+                            desc="""Just a description for a sample program.""")
+        PROG()
+
+
+
+3. Utilisation :
+~~~~~~~~~~~~~~~~
+
+Now you can show the help menu using the following command :
+
+``$ ./sample-program.py test -h``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    usage: sample-program test [-h] --host HOST [--port PORT]
+
+    optional arguments:
+      -h, --help   show this help message and exit
+      --host HOST
+      --port PORT
+
+Or run your command :
+
+``$  ./sample-program.py test --host 127.0.0.1``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    This is the beginning of the TestCommand class.
+    The command line arguments (argv) :
+    -----------------------------------
+    Namespace(__func__=<__main__.TestCommand object at 0xb721a92c>,
+    config_file=None, host='127.0.0.1', port=3000, verbose=False)
+
+    This is the end of the TestCommand class.
+
+You can see the variable ``host`` contains the input message ``127.0.0.1`` into the
+args object.
+The option ``port`` contains the default value ``3000``.
+
+
+Advanced usage
+--------------
+
+At this point, this program does not do much more than the argparse module can
+do.
+In the cas you have a lot of command and option, it could be usefull to store
+default values in a configuration file like ``sample-program.cfg``
+
+
+4. Imports :
+~~~~~~~~~~~~
+
+First of all, you just need the following classes to build your own script :
+
+* **TestCommand :** This command class will print to stdout the inputs args and
+  the configuration file content.
+
+* **BasicProgram :** The most simple program to run your command classes.
+
+* **SimpleSection :** This class is used to declare a Section in the config file
+  (ConfigFile)
+
+* **Element :** This class is used to declare an Option (a field) in the
+  previous section.
+
+* **Base64ElementHook :** This hook is used as a post reading processing in
+  order to convert base64 data stored into the config file into plain text data.
+
+
+
+5. Declaration :
+~~~~~~~~~~~~~~~~
+
+There is a script called sample-program2.py which contains all the following
+lines of code.
+
+
+#. Instead of creating a config file, we will use an in-memory config file
+   (**Step 1**)
+#. You create an other class MyProgram (which extends the BasicProgram) (**Step
+   2**)
+#. We override the default method called ``add_config_options``. (**Step 3**)
+#. We declare the section named ``ldap`` that we are looking for.
+#. We declare all the fields store into the previous section. For each fied, you can says if it is required, the default value, the type, an optional description. See the documentatino for more details. (**Step 5**).
+#. The we declare all argparse arguments using the previous configuration declaration. This is very usefull because the data store into the configuration file are used as the default value for the argparse argument. The description, the type, required or not, ... declared in the ``add_config_options`` method are used to configure the parser argument. No need to repeat your self. (**Step 6**)
+#. Declaration of the ``test`` argument using TestCommand class. (**Step 7**)
+#. Finally you just have to instanciate your class MyProgram, the first argument is the program name. (**Step 8**)
+#. We override the default config file name ``'.<program name>.cfg'``. (**Step 9**)
+#. We launch the program. (**Step 10**)
+
+
+.. code-block:: python
+
+    #! /usr/bin/env python2
+    # -*- coding: utf-8 -*-
+    # PYTHON_ARGCOMPLETE_OK
+
+    import io
+    from argtoolbox import TestCommand
+    from argtoolbox import BasicProgram
+    from argtoolbox import SimpleSection, Element, Base64ElementHook
+
+    # Step 1
+    SAMPLE_CONFIG = """
+    [ldap]
+
+    host=127.0.0.1
+    port=389
+    suffix=dc=nodomain
+    account=cn=admin,dc=nodomain
+    password=toto
+
+    \n"""
+
+    # Step 2
+    class MyProgram(BasicProgram):
+
+        # Step 3
+        def add_config_options(self):
+            # Step 4
+            # section ldap
+            section_ldap = self.config.add_section(SimpleSection("ldap"))
+            # Step 5
+            section_ldap.add_element(Element('debug',
+                                             e_type=int,
+                                             default=0,
+                                             desc="""debug level : default : 0."""))
+            section_ldap.add_element(Element('host',
+                                             required=True,
+                                             default="192.168.1.1"))
+            section_ldap.add_element(Element('account', required=True))
+            section_ldap.add_element(Element('port', e_type=int))
+            section_ldap.add_element(Element('password',
+                                             required=True,
+                                             hidden=True,
+                                             desc="account password to ldap",
+                                             hooks=[Base64ElementHook(), ]))
+
+       def add_commands(self):
+            # Step 6
+            self.parser.add_argument(
+                '--host', **self.config.ldap.host.get_arg_parse_arguments())
+            self.parser.add_argument(
+                '--port', **self.config.ldap.port.get_arg_parse_arguments())
+            self.parser.add_argument(
+                '-d',
+                action="count",
+                **self.config.ldap.debug.get_arg_parse_arguments())
+
+            # Step 7
+            subparsers = self.parser.add_subparsers()
+            parser_tmp = subparsers.add_parser(
+                'test',
+                help="This simple command print cli argv and configuration read \
+                form config file.")
+            parser_tmp.set_defaults(__func__=TestCommand(self.config))
+
+
+    if __name__ ≡ "__main__":
+
+        # Step 8
+        PROG = MyProgram("sample-program",
+            # Step 9
+                         config_file=io.BytesIO(SAMPLE_CONFIG),
+                         desc="""Just a description for a sample program.""")
+        # Step 10
+        PROG()
+
+6. Utilisation :
+~~~~~~~~~~~~~~~~
+
+Now you can run your command :
+
+``$ ./sample-program2.py --host an.other.host.com test``
+
+**Console ouput :**
+
+.. code-block:: python
+
+    This is the beginning of the TestCommand class.
+
+    The loaded configuration :
+    ---------------------------
+    Configuration of sample-program :
+
+            Section LDAP
+             - debug : 0
+             - host : 127.0.0.1
+             - account : cn=admin,dc=nodomain
+             - port : 389
+             - password : xxxxxxxx
+
+
+    The command line arguments (argv) :
+    ------------------------------------
+    Namespace(__func__=<argtoolbox.argtoolbox.TestCommand object at 0xb7199f8c>, config_file=None, debug=0, host='an.other.host.com', port=389, verbose=False)
+
+    This is the end of the TestCommand class.
+
+You can see the variable ``host`` contains the input message ``an.other.host.com`` into the
+args object. The option ``port`` contains the default value ``389``.
+You can also acces to the values store into the configuration file like ``account`` or ``password`` which can not be override by the CLI.
```

### Comparing `argtoolbox-1.1.4/setup.py` & `argtoolbox-1.1.5/setup.py`

 * *Files identical despite different names*

