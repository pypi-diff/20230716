# Comparing `tmp/whisper_autosrt-0.1.8.tar.gz` & `tmp/whisper_autosrt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.8.tar", last modified: Thu Jul 13 01:25:53 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.9.tar", last modified: Sun Jul 16 11:58:02 2023, max compression
```

## Comparing `whisper_autosrt-0.1.8.tar` & `whisper_autosrt-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.615467 whisper_autosrt-0.1.8/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2056 2023-07-13 01:25:53.616216 whisper_autosrt-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.8/README.md
--rw-rw-rw-   0        0        0      147 2023-07-13 01:25:53.618463 whisper_autosrt-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-06-21 11:17:31.000000 whisper_autosrt-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.584000 whisper_autosrt-0.1.8/whisper_autosrt/
--rw-rw-rw-   0        0        0   169913 2023-07-13 01:25:07.000000 whisper_autosrt-0.1.8/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:25:53.613970 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     2056 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-13 01:25:53.000000 whisper_autosrt-0.1.8/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 11:58:02.820950 whisper_autosrt-0.1.9/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2056 2023-07-16 11:58:02.821700 whisper_autosrt-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.9/README.md
+-rw-rw-rw-   0        0        0      147 2023-07-16 11:58:02.824697 whisper_autosrt-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-06-21 11:17:31.000000 whisper_autosrt-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:58:02.778246 whisper_autosrt-0.1.9/whisper_autosrt/
+-rw-rw-rw-   0        0        0   178378 2023-07-16 11:54:06.000000 whisper_autosrt-0.1.9/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:58:02.818702 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 11:58:02.000000 whisper_autosrt-0.1.9/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.8/LICENSE` & `whisper_autosrt-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.8/PKG-INFO` & `whisper_autosrt-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.8
+Version: 0.1.9
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.8/README.md` & `whisper_autosrt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.8/setup.py` & `whisper_autosrt-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.8/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.9/whisper_autosrt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 #marker='█'
 
 
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
@@ -2214,14 +2214,88 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
+def has_subtitles(media_filepath, error_messages_callback=None):
+    def which(program):
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    def ffmpeg_check():
+        if which("ffmpeg"):
+            return "ffmpeg"
+        if which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
+    if "\\" in media_filepath:
+        media_filepath = media_filepath.replace("\\", "/")
+
+    if not os.path.isfile(media_filepath):
+        if error_messages_callback:
+           error_messages_callback(f"The given file does not exist: '{media_filepath}'")
+        else:
+            print(f"The given file does not exist: '{media_filepath}'")
+            raise Exception(f"Invalid file: '{media_filepath}'")
+    if not ffmpeg_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffmpeg executable")
+        else:
+            print("Cannot find ffmpeg executable")
+            raise Exception("Dependency not found: ffmpeg")
+
+    try:
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        ffmpeg_cmd = [
+                        'ffmpeg',
+                        '-hide_banner',
+                        '-v', 'error',
+                        '-loglevel', 'error',
+                        '-y',
+                        '-i', media_filepath,
+                        '-map', '0:s:0',
+                        '-f', 'srt',
+                        '-'
+                     ]
+
+        result = None
+        if sys.platform == "win32":
+            result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
+
+        if result.stdout:
+            return True  # Subtitles detected
+        else:
+            return False  # No subtitles detected
+
+    except Exception as e:
+        if self.error_messages_callback:
+            self.error_messages_callback(e)
+        else:
+            print(e)
+        return False
+
+
 def change_code_page(code_page):
     kernel32 = ctypes.windll.kernel32
     kernel32.SetConsoleOutputCP(code_page)
     kernel32.SetConsoleCP(code_page)
 
 
 def stop_ffmpeg_windows(error_messages_callback=None):
@@ -2556,15 +2630,15 @@
         if sys.platform == "win32":
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
         total_duration = float(ffprobe_process.strip())
 
-        widgets = [f"Rendering '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        widgets = [f"Rendering '{language_code}' subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
         process = None
         if sys.platform == "win32":
             process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
@@ -2584,15 +2658,14 @@
                 current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
                 if current_duration>0 and current_duration<=total_duration*1000:
                     percentage = int(current_duration*100/(int(float(total_duration))*1000))
                     if percentage <= 100:
                         pbar.update(percentage)
 
-
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
@@ -2691,15 +2764,15 @@
             if sys.platform == "win32":
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
             total_duration = float(ffprobe_process.strip())
 
-            widgets = [f"Embedding '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+            widgets = [f"Embedding '{language_code}' subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             percentage = 0
 
             process = None
             if sys.platform == "win32":
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
@@ -2810,15 +2883,15 @@
         if sys.platform == "win32":
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
         total_duration = float(ffprobe_process.strip())
 
-        widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        widgets = ["Removing subtitles streams from file : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
         process = None
         if sys.platform == "win32":
             process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
@@ -2999,14 +3072,15 @@
     completed_tasks = 0
     media_filepaths = []
     arg_filepaths = []
     invalid_media_filepaths = []
     not_exist_filepaths = []
     argpath = None
     media_type = None
+    media_format = None
 
     args_source_path = args.source_path
     subtitle_format = args.format
 
     if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
         for filepath in args_source_path:
             fpath = Path(filepath)
@@ -3028,25 +3102,20 @@
         arg_filepaths += glob(arg)
 
     if arg_filepaths:
         for argpath in arg_filepaths:
             if os.path.isfile(argpath):
                 if check_file_type(argpath, error_messages_callback=show_error_messages) == 'video':
                     media_filepaths.append(argpath)
-                    media_type = "video"
                 elif check_file_type(argpath, error_messages_callback=show_error_messages) == 'audio':
                     media_filepaths.append(argpath)
-                    media_type = "audio"
-
                 else:
                     invalid_media_filepaths.append(argpath)
-                    media_type = None
             else:
                 not_exist_filepaths.append(argpath)
-                media_type = None
 
         if invalid_media_filepaths:
             for invalid_media_filepath in invalid_media_filepaths:
                 msg = f"'{invalid_media_filepath}' is not valid video or audio files"
                 print(msg)
 
     if not_exist_filepaths:
@@ -3064,43 +3133,57 @@
 
     transcribe_end_time = None
     transcribe_elapsed_time = None
     transcribe_start_time = time.time()
     task = "transcribe"
     total_duration = 0
 
+    src_subtitle_filepath = None
+    dst_subtitle_filepath = None
+    ffmpeg_src_language_code = None
+    ffmpeg_dst_language_code = None
+    embedded_media_filepath = None
+
     if args.src_language in google_unsupported_languages and do_translate:
         task = "translate"
         src_language = "en"
 
     removed_media_filepaths = []
     dst_language = args.dst_language
 
+
+    # CHECK SUBTITLE STREAM PART
     if args.force_recognize == False:
 
         print("CHECKING EXISTING SUBTITLES STREAMS")
         print("===================================")
 
         # CHECKING ffmpeg_src_language_code SUBTITLES STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
         if do_translate == False:
 
             for media_filepath in media_filepaths:
+
                 print(f"Checking '{media_filepath}'")
 
+                media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+                if media_type == "audio":
+                    print("Audio file won't have subtitles streams, skip checking")
+                    continue
+
                 if args.src_language == "auto":
                     try:
-                        widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                        widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
                         wav_filepath, sample_rate = wav_converter(media_filepath)
                         pbar.finish()
 
                         segments, info = model.transcribe(wav_filepath)
                         src_language = info.language
-                        print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
+                        print(f"Detected language                       : {info.language} (probability = {info.language_probability})")
 
                     except KeyboardInterrupt:
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
                         print("Cancelling all tasks")
@@ -3130,88 +3213,96 @@
                             sys.exit(1)
 
                 else:
                     src_language = args.src_language
 
                 if src_language in google_unsupported_languages and args.force_recognize==False:
                     print("Language is not supported by Google Translate API")
+                    print(f"Removing '{media_filepath}' from speech recognition process list")
                     removed_media_filepaths.append(media_filepath)
 
                 else:
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                     subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                     subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
                     if subtitle_streams_data and subtitle_streams_data != []:
 
                         src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                         if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_src_language_code.center(3)))
+                            print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : Yes")
 
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in src_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
 
                             base, ext = os.path.splitext(media_filepath)
                             src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
-                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
+                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as    : '{src_subtitle_filepath}'")
 
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             writer.write(src_subtitle_filepath)
 
-                            if args.force_recognize == False:
-                                removed_media_filepaths.append(media_filepath)
-
                             # no translate process as instructed in command arguments
 
                             # if args.embed_src is True we can't embed it because dst subtitles stream already exist
                             if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                 print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
+                            if args.force_recognize == False:
+                                print(f"Removing '{media_filepath}' from speech recognition process list")
+                                removed_media_filepaths.append(media_filepath)
+
+                            if os.path.isfile(src_subtitle_filepath):
+                                completed_tasks += 1
+                                #print(f"args.force_recognize == False, do_translate == False, media_type == 'video', subtitle stream = exist : completed_tasks = {completed_tasks}")
+
                         else:
-                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_src_language_code.center(3)))
+                            print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : No")
 
                 print("")
 
-            if removed_media_filepaths:
-                for removed_media_filepath in removed_media_filepaths:
-                    media_filepaths.remove(removed_media_filepath)
-
             if not media_filepaths:
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
+                msg = "Total running time                       : %s:%s:%s" %(hour.zfill(2), minute, second)
                 print(msg)
                 sys.exit(0)
 
         # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLES STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
         # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT AND THEN EMBED IT
         elif do_translate == True:
             for media_filepath in media_filepaths:
+
                 print(f"Checking '{media_filepath}'")
 
+                media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+                if media_type == "audio":
+                    print("Audio file won't have subtitles streams, skip checking")
+                    continue
+
                 if args.src_language == "auto":
                     try:
-                        widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                        widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
                         wav_filepath, sample_rate = wav_converter(media_filepath)
                         pbar.finish()
 
                         segments, info = model.transcribe(wav_filepath)
                         src_language = info.language
-                        print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
+                        print(f"Detected language                       : {info.language} (probability = {info.language_probability})")
 
                     except KeyboardInterrupt:
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
                         print("Cancelling all tasks")
@@ -3241,14 +3332,15 @@
                             sys.exit(1)
 
                 else:
                     src_language = args.src_language
 
                 if src_language in google_unsupported_languages and args.force_recognize==False:
                     print(f"Language '{src_language}' is not supported by Google Translate API")
+                    print(f"Removing '{media_filepath}' from speech recognition process list")
                     removed_media_filepaths.append(media_filepath)
 
                 else:
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                     subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
@@ -3257,59 +3349,60 @@
                     if subtitle_streams_data and subtitle_streams_data != []:
 
                         src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
                         dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
                         # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
                         if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_src_language_code.center(3)))
+                            print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : Yes")
 
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in src_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
 
                             base, ext = os.path.splitext(media_filepath)
                             src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
-                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
+                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as    : '{src_subtitle_filepath}'")
 
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             writer.write(src_subtitle_filepath)
 
                         # ffmpeg_src_language_code subtitles stream not exist, just print it
                         else:
-                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_src_language_code.center(3)))
+                            print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : No")
 
                         # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
                         if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_dst_language_code.center(3)))
+                            print(f"Is '{ffmpeg_dst_language_code}' subtitles stream exist         : Yes")
+
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in dst_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
                             base, ext = os.path.splitext(media_filepath)
                             dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                            print(f"Extracting '{ffmpeg_dst_language_code}' subtitles stream as       : '{dst_subtitle_filepath}'")
+                            print(f"Extracting '{ffmpeg_dst_language_code}' subtitles stream as    : '{dst_subtitle_filepath}'")
                             writer.write(dst_subtitle_filepath)
 
                         # ffmpeg_dst_language_code subtitles stream not exist, just print it
                         else:
-                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_dst_language_code.center(3)))
+                            print(f"Is '{ffmpeg_dst_language_code}' subtitles stream exist         : No")
 
                         # ffmpeg_src_language_code subtitles stream = not exist,
                         # ffmpeg_dst_language_code subtitles stream = exist,
                         # so we translate it from 'dst_language' to 'src_language'
                         if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
 
                             if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
-                                prompt = "Translating from %s to %s      : " %(dst_language.center(8), src_language.center(8))
+                                prompt = "Translating from %s to %s   : " %(dst_language.center(8), src_language.center(8))
                                 widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                                 pbar = ProgressBar(widgets=widgets, maxval=len(dst_subtitle_stream_timed_subtitles)).start()
 
                                 transcript_translator = SentenceTranslator(src=dst_language, dst=src_language, error_messages_callback=show_error_messages)
 
                                 translated_subtitle_stream_transcripts = []
                                 for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
@@ -3319,17 +3412,18 @@
 
                                 base, ext = os.path.splitext(media_filepath)
                                 src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
                                 translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                                 translation_writer.write(src_subtitle_filepath)
 
-                                print(f"Translated subtitles file saved as         : '{src_subtitle_filepath}'")
+                                print(f"Translated subtitles file saved as      : '{src_subtitle_filepath}'")
 
                                 if args.force_recognize == False:
+                                    print(f"Removing '{media_filepath}' from speech recognition process list")
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_src and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                                     base, ext = os.path.splitext(media_filepath)
 
@@ -3337,38 +3431,38 @@
                                         media_format = "mp4"
                                     else:
                                         media_format = ext[1:]
 
                                     src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
                                     embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
-                                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     src_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
                                     if os.path.isfile(src_tmp_output):
                                         shutil.copy(src_tmp_output, embedded_media_filepath)
                                         os.remove(src_tmp_output)
 
                                     if os.path.isfile(embedded_media_filepath):
-                                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+                                        print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
 
                                 # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
                                 if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                     print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
 
                         # ffmpeg_src_language_code subtitles stream = exist,
                         # ffmpeg_dst_language_code subtitles stream = not exist,
                         # so we translate it from 'src_language' to 'dst_language'
                         if ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
                             if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
-                                prompt = "Translating from %s to %s      : " %(src_language.center(8), dst_language.center(8))
+                                prompt = "Translating from %s to %s   : " %(src_language.center(8), dst_language.center(8))
                                 widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
                                 pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
 
                                 transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
 
                                 translated_subtitle_stream_transcripts = []
                                 for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
@@ -3381,14 +3475,15 @@
 
                                 translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                                 translation_writer.write(dst_subtitle_filepath)
 
                                 print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
 
                                 if args.force_recognize == False:
+                                    print(f"Removing '{media_filepath}' from speech recognition process list")
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                                     base, ext = os.path.splitext(media_filepath)
 
@@ -3396,338 +3491,398 @@
                                         media_format = "mp4"
                                     else:
                                         media_format = ext[1:]
 
                                     dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
                                     embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
-                                    widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                    widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     dst_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
                                     if os.path.isfile(dst_tmp_output):
                                         shutil.copy(dst_tmp_output, embedded_media_filepath)
                                         os.remove(dst_tmp_output)
 
                                     if os.path.isfile(embedded_media_filepath):
-                                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+                                        print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
 
                                 # if args.embed_src is True then no need to embed it because src subtitles stream already exist
                                 if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                     print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
                         # ffmpeg_dst_language_code subtitles stream = exist,
                         # ffmpeg_src_language_code subtitles stream = exist,
-                        # so we remove media_filepath from the list of files to be proceed
+                        # so we remove media_filepath from the list of files to be processed
                         elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
+
+                            # remove media_filepath from transcribe processed_list because all needed srt files already saved
                             if args.force_recognize == False:
+                                print(f"Removing '{media_filepath}' from speech recognition process list")
                                 removed_media_filepaths.append(media_filepath)
 
                             # no need to translate becouse both languages subtitles files already saved
 
                             # if args.embed_src is True we can't embed it because dst subtitles stream already exist
                             if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                 print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
                             # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
                             if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                 print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
 
-                print("")
+                        if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
+                            if args.force_recognize == False:
+                                completed_tasks += 1
+                                #print(f"\nargs.force_recognize == False, do_translate == True, media_type == 'video', subtitle stream = exist : completed_tasks = {completed_tasks}\n")
 
-            if removed_media_filepaths:
-                for removed_media_filepath in removed_media_filepaths:
-                    if removed_media_filepath in media_filepaths:
-                        media_filepaths.remove(removed_media_filepath)
+                print("")
+            print("")
 
             if not media_filepaths:
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
+                msg = "Total running time                       : %s:%s:%s" %(hour.zfill(2), minute, second)
                 print(msg)
                 sys.exit(0)
 
 
-    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RE-RECOGNIZED")
-    print("=========================================================================================================")
+    # SUBTITLES STREAMS REMOVER PART (IF args.force_recognize == True)
+    print("FORCE RECOGNIZE FLAG CHECK")
+    print("==========================")
 
-    proceed_list = []
-    # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
-    if args.force_recognize == True:
-        for media_filepath in media_filepaths:
-            base, ext = os.path.splitext(media_filepath)
+    processed_list = []
+
+    # if args.force_recognize is true then we need to remove subtitle streams and save it as new media file to processed with transcribe
+    for media_filepath in media_filepaths:
+
+        print(f"Checking '{media_filepath}'")
+
+        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+        if media_type == "video" and args.force_recognize == True:
+
+            force_recognize_media_file_format = None
 
+            base, ext = os.path.splitext(media_filepath)
             if ext[1:] == "ts":
-                media_format = "mp4"
+                force_recognize_media_file_format = "mp4"
             else:
-                media_format = ext[1:]
+                force_recognize_media_file_format = ext[1:]
 
-            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{media_format}"
-            subtitle_removed_media_filepath = f"{base}.force.recognize.{media_format}"
+            #print(f"media_filepath = {media_filepath}")
+            subtitle_stream_parser = SubtitleStreamParser()
+            subtitle_streams_data = subtitle_stream_parser(media_filepath)
+            #print(f"subtitle_streams_data = {subtitle_streams_data}")
+            #print(f"subtitle_stream_parser.timed_subtitles_of_index(1) = {subtitle_stream_parser.timed_subtitles_of_index(1)}")
 
-            #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+            if subtitle_streams_data and subtitle_stream_parser.timed_subtitles_of_index(1) != []:
 
-            widgets = [f"Removing subtitles streams from {media_type} file : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-            subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-            tmp_output = subtitle_remover(media_filepath)
-            pbar.finish()
+                tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{force_recognize_media_file_format}"
+                subtitle_removed_media_filepath = f"{base}.force.recognize.{force_recognize_media_file_format}"
 
-            if os.path.isfile(tmp_output):
-                shutil.copy(tmp_output, subtitle_removed_media_filepath)
-                os.remove(tmp_output)
+                widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                tmp_output = subtitle_remover(media_filepath)
+                pbar.finish()
 
-                proceed_list.append(subtitle_removed_media_filepath)
+                if os.path.isfile(tmp_output):
+                    shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                    os.remove(tmp_output)
 
-            print(f"Subtitles removed {media_type} file saved as      : '{subtitle_removed_media_filepath}'")
-            print("")
+                    processed_list.append(subtitle_removed_media_filepath)
 
-    # if args.force_recognize is false then we just use modified media_filepaths list
-    else:
-        proceed_list = media_filepaths
+                print(f"Subtitles removed {media_type} file saved as   : '{subtitle_removed_media_filepath}'")
+
+            else:
+                print("Nothing to remove")
+                if media_filepath not in processed_list and media_filepath not in removed_media_filepaths:
+                    processed_list.append(media_filepath)
+
+        else:
+            if media_type == "video":
+                print("force_recognize is false")
+
+            if media_type == "audio":
+                print(f"'{media_filepath}' is audio file, nothing to remove")
+
+            if media_filepath not in processed_list and media_filepath not in removed_media_filepaths:
+                processed_list.append(media_filepath)
+
+        print("")
 
 
     # START THE TRANSCRIBE PROCESS
-    for media_filepath in proceed_list:
+    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RECOGNIZED")
+    print("=========================================================================================================")
+
+    for media_filepath in processed_list:
         print(f"Processing '{media_filepath}'")
 
+        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
         try:
-            widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
+            widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
             wav_filepath, sample_rate = wav_converter(media_filepath)
             pbar.finish()
 
             if args.src_language == "auto":
                 segments, info = model.transcribe(wav_filepath)
                 src_language = info.language
-                print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
+                print(f"Detected language                       : {info.language} (probability = {info.language_probability})")
                 total_duration = info.duration
                 ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                 if src_language in google_unsupported_languages and do_translate:
                     task = "translate"
                     src_language = "en"
 
             else:
                 segments, info = model.transcribe(wav_filepath, language=src_language, task=task)
                 total_duration = info.duration
 
-            widgets = ["Performing speech recognition              : ", Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
-            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-
-            timed_subtitles = []
-            regions = []
-            transcripts = []
-            for segment in segments:
-                progress = int(round(float(segment.end))*100/total_duration)
-                regions.append((segment.start, segment.end))
-                transcripts.append(segment.text)
-                pbar.update(progress)
-            pbar.finish()
-            timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
-
-            base, ext = os.path.splitext(media_filepath)
-            src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
-
-            writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
-            writer.write(src_subtitle_filepath)
-
-            if do_translate:
-                timed_subtitles = writer.timed_subtitles
-                created_regions = []
-                created_subtitles = []
-                for entry in timed_subtitles:
-                    created_regions.append(entry[0])
-                    created_subtitles.append(entry[1])
-
-                prompt = "Translating from %s to %s      : " %(src_language.center(8), dst_language.center(8))
-                widgets = [prompt, Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
-                pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-
-                transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
-
-                translated_subtitles = []
-                for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
-                    translated_subtitles.append(translated_subtitle)
-                    pbar.update(i)
+            if segments:
+                widgets = ["Performing speech recognition           : ", Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
+                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+
+                timed_subtitles = []
+                regions = []
+                transcripts = []
+                for segment in segments:
+                    progress = int(round(float(segment.end))*100/total_duration)
+                    regions.append((segment.start, segment.end))
+                    transcripts.append(segment.text)
+                    pbar.update(progress)
                 pbar.finish()
+                timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
 
                 base, ext = os.path.splitext(media_filepath)
-                dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
+                src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
-                translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
-                translation_writer.write(dst_subtitle_filepath)
+                writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                writer.write(src_subtitle_filepath)
 
-            if do_translate:
-                print(f"Original subtitles file saved as           : '{src_subtitle_filepath}'")
-                print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
-            else:
-                print(f"Subtitles file saved as                    : '{src_subtitle_filepath}'")
+                if do_translate == True:
+                    timed_subtitles = writer.timed_subtitles
+                    created_regions = []
+                    created_subtitles = []
+                    for entry in timed_subtitles:
+                        created_regions.append(entry[0])
+                        created_subtitles.append(entry[1])
+
+                    prompt = "Translating from %s to %s   : " %(src_language.center(8), dst_language.center(8))
+                    widgets = [prompt, Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
+
+                    transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
+
+                    translated_subtitles = []
+                    for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
+                        translated_subtitles.append(translated_subtitle)
+                        pbar.update(i)
+                    pbar.finish()
 
+                    base, ext = os.path.splitext(media_filepath)
+                    dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
+                    translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
+                    translation_writer.write(dst_subtitle_filepath)
 
-            # EMBEDDING SUBTITLES FILE
+                    print(f"Original subtitles file saved as        : '{src_subtitle_filepath}'")
+                    print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
 
-            embedded_media_filepath = None
+                    if media_type == "audio":
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
 
-            if do_translate == False:
+                    elif media_type == "video" and args.embed_src == False and args.embed_dst == False:
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
 
-                if args.embed_src == True:
+                elif do_translate == False:
+                    print(f"Subtitles file saved as                  : '{src_subtitle_filepath}'")
 
-                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+                    if media_type == "audio":
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
 
-                    base, ext = os.path.splitext(media_filepath)
+                    elif media_type == "video" and args.embed_src == False:
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'video', args.embed_src == False : completed_tasks = {completed_tasks}\n")
 
-                    if ext[1:] == "ts":
-                        media_format = "mp4"
-                    else:
-                        media_format = ext[1:]
 
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
+                # EMBEDDING SUBTITLES FILE
 
-                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    src_tmp_output = subtitle_embedder(media_filepath)
-                    pbar.finish()
+                embedded_media_filepath = None
 
-                    if os.path.isfile(src_tmp_output):
-                        shutil.copy(src_tmp_output, embedded_media_filepath)
-                        os.remove(src_tmp_output)
-                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+                if do_translate == False:
 
-            elif do_translate == True:
+                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-                if args.embed_src == True and args.embed_dst == True:
+                    if media_type == "audio" and args.embed_src == True:
+                        print("Subtitles can only be embedded into video file, not audio file")
 
-                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
-                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+                    if media_type == "video" and args.embed_src == True:
 
-                    base, ext = os.path.splitext(media_filepath)
+                        ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
-                    if ext[1:] == "ts":
-                        media_format = "mp4"
-                    else:
-                        media_format = ext[1:]
+                        base, ext = os.path.splitext(media_filepath)
 
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                    src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
-
-                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    src_tmp_output = subtitle_embedder(media_filepath)
-                    pbar.finish()
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
-                    if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
-                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        src_dst_tmp_output = subtitle_embedder(src_tmp_output)
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
-                    if os.path.isfile(src_dst_tmp_output):
-                        shutil.copy(src_dst_tmp_output, embedded_media_filepath)
-                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
-                    else:
-                        print("Unknown error!")
+                        if os.path.isfile(src_tmp_output):
+                            shutil.copy(src_tmp_output, embedded_media_filepath)
+                            os.remove(src_tmp_output)
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
 
-                    if os.path.isfile(src_dst_tmp_output):
-                        os.remove(src_dst_tmp_output)
+                    if media_type == "video" and args.embed_src == False:
+                        completed_tasks += 1
+                        #print(f"\ndo_translate == False, media_type == 'video' : completed_tasks = {completed_tasks}\n")
 
-                    if os.path.isfile(src_tmp_output):
-                        os.remove(src_tmp_output)
 
+                elif do_translate == True:
 
-                elif args.embed_src == True and args.embed_dst == False:
+                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+                    if media_type == "audio" and (args.embed_src == True or args.embed_src == True):
+                        print("Subtitles can only be embedded into video file, not audio file")
 
-                    base, ext = os.path.splitext(media_filepath)
+                    if media_type == "video" and args.embed_src == True and args.embed_dst == True:
 
-                    if ext[1:] == "ts":
-                        media_format = "mp4"
-                    else:
-                        media_format = ext[1:]
+                        ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+                        ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
-                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
+                        base, ext = os.path.splitext(media_filepath)
 
-                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    src_tmp_output = subtitle_embedder(media_filepath)
-                    pbar.finish()
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
 
-                    if os.path.isfile(src_tmp_output):
-                        shutil.copy(src_tmp_output, embedded_media_filepath)
-                        os.remove(src_tmp_embedded_media_filepath)
-                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
-                    else:
-                        print("Unknown error!")
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
-                elif args.embed_src == False and args.embed_dst == True:
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
+                        pbar.finish()
 
-                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+                        if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            src_dst_tmp_output = subtitle_embedder(src_tmp_output)
+                            pbar.finish()
 
-                    base, ext = os.path.splitext(media_filepath)
+                        if os.path.isfile(src_dst_tmp_output):
+                            shutil.copy(src_dst_tmp_output, embedded_media_filepath)
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
+                        else:
+                            print("Unknown error!")
 
-                    if ext[1:] == "ts":
-                        media_format = "mp4"
-                    else:
-                        media_format = ext[1:]
+                        if os.path.isfile(src_dst_tmp_output):
+                            os.remove(src_dst_tmp_output)
+                        if os.path.isfile(src_tmp_output):
+                            os.remove(src_tmp_output)
 
-                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
-                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
+                    elif media_type == "video" and args.embed_src == True and args.embed_dst == False:
 
-                    widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    dst_tmp_output = subtitle_embedder(media_filepath)
-                    pbar.finish()
+                        ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
-                    if os.path.isfile(dst_tmp_output):
-                        shutil.copy(dst_tmp_output, embedded_media_filepath)
-                        os.remove(dst_tmp_output)
-                        print(f"Subtitles embedded {media_type} file saved as     : {embedded_media_filepath}")
-                    else:
-                        print("Unknown error!")
+                        base, ext = os.path.splitext(media_filepath)
 
-            if do_translate == False:
-                if args.embed_src == True:
-                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                        completed_tasks += 1
-                else:
-                    completed_tasks += 1
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
 
-            elif do_translate == True:
-                if args.embed_src == True or args.embed_dst == True:
-                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                        completed_tasks += 1
-                else:
-                    completed_tasks += 1
+                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
+
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if os.path.isfile(src_tmp_output):
+                            shutil.copy(src_tmp_output, embedded_media_filepath)
+                            os.remove(src_tmp_embedded_media_filepath)
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
+                        else:
+                            print("Unknown error!")
+
+                    elif media_type == "video" and args.embed_src == False and args.embed_dst == True:
+
+                        ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                        base, ext = os.path.splitext(media_filepath)
+
+                        if ext[1:] == "ts":
+                            media_format = "mp4"
+                        else:
+                            media_format = ext[1:]
+
+                        dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                        embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
+
+                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        dst_tmp_output = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if os.path.isfile(dst_tmp_output):
+                            shutil.copy(dst_tmp_output, embedded_media_filepath)
+                            os.remove(dst_tmp_output)
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
+                        else:
+                            print("Unknown error!")
 
             print("")
+
+            #print(f"len(media_filepaths) = {len(media_filepaths)}")
+            #print(f"completed_tasks = {completed_tasks}")
+
             if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
+                msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
                 print(msg)
 
-
         except KeyboardInterrupt:
             pbar.finish()
             pool.terminate()
             pool.close()
             pool.join()
             print("Cancelling all tasks")
```

### Comparing `whisper_autosrt-0.1.8/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.9/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.8
+Version: 0.1.9
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

