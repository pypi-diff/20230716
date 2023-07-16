# Comparing `tmp/autosrt-1.4.6.tar.gz` & `tmp/autosrt-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.4.6.tar", last modified: Thu Jul 13 01:58:07 2023, max compression
+gzip compressed data, was "autosrt-1.4.7.tar", last modified: Sun Jul 16 11:56:02 2023, max compression
```

## Comparing `autosrt-1.4.6.tar` & `autosrt-1.4.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.786406 autosrt-1.4.6/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.6/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-07-13 01:58:07.787156 autosrt-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.643716 autosrt-1.4.6/autosrt/
--rw-rw-rw-   0        0        0   163312 2023-07-13 01:51:28.000000 autosrt-1.4.6/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.701405 autosrt-1.4.6/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 01:58:07.000000 autosrt-1.4.6/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-13 01:58:07.796146 autosrt-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:58:07.783431 autosrt-1.4.6/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.6/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.6/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.6/test/test3.py
--rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.6/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:56:02.061192 autosrt-1.4.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-07-16 11:56:02.061942 autosrt-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:56:01.958885 autosrt-1.4.7/autosrt/
+-rw-rw-rw-   0        0        0   168204 2023-07-16 11:52:40.000000 autosrt-1.4.7/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:56:01.992361 autosrt-1.4.7/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-16 11:56:02.064943 autosrt-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:56:02.058195 autosrt-1.4.7/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.7/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.7/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.7/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.7/test/test4.py
```

### Comparing `autosrt-1.4.6/LICENSE` & `autosrt-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/PKG-INFO` & `autosrt-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.6
+Version: 1.4.7
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.6/README.md` & `autosrt-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/autosrt/__init__.py` & `autosrt-1.4.7/autosrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
 
-VERSION = "1.4.6"
+VERSION = "1.4.7"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -1196,17 +1196,17 @@
                 return self.vtt_formatter(subtitles, padding_before, padding_after)
             elif self.format_type == 'json':
                 return self.json_formatter(subtitles)
             elif self.format_type == 'raw':
                 return self.raw_formatter(subtitles)
             else:
                 if error_messages_callback:
-                    error_messages_callback(f'Unsupported format type: {self.format_type}')
+                    error_messages_callback(f"Unsupported format type: '{self.format_type}'")
                 else:
-                    raise ValueError(f'Unsupported format type: {self.format_type}')
+                    raise ValueError(f"Unsupported format type: '{self.format_type}'")
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
             return
@@ -1277,15 +1277,15 @@
         try:
             formatter = SubtitleFormatter(self.format)
             formatted_subtitles = formatter(self.timed_subtitles)
             saved_subtitle_filepath = declared_subtitle_filepath
             if saved_subtitle_filepath:
                 subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
                 if not subtitle_file_ext:
-                    saved_subtitle_filepath = "{subtitle_file_base}.{self.format}"
+                    saved_subtitle_filepath = f"{subtitle_file_base}.{self.format}"
                 else:
                     saved_subtitle_filepath = declared_subtitle_filepath
             with open(saved_subtitle_filepath, 'wb') as f:
                 f.write(formatted_subtitles.encode("utf-8"))
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -1786,15 +1786,15 @@
                 print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
             if self.language in existing_languages:
                 # THIS 'print' THINGS WILL MAKE progresbar screwed up!
-                #msg = (f"'{self.language}' subtitle stream already existed in '{media_filepath}'")
+                #msg = (f"'{self.language}' subtitles stream already existed in '{media_filepath}'")
                 #if self.error_messages_callback:
                 #    self.error_messages_callback(msg)
                 #else:
                 #    print(msg)
                 return
 
             else:
@@ -2703,17 +2703,17 @@
 
 def stop_ffmpeg_linux(error_messages_callback=None):
     process_name = 'ffmpeg'
     try:
         output = subprocess.check_output(['ps', '-ef'])
         pid = [line.split()[1] for line in output.decode('utf-8').split('\n') if process_name in line][0]
         subprocess.call(['kill', '-9', str(pid)])
-        #print(f"{process_name} has been killed")
+        #print(f"'{process_name}' has been killed")
     except IndexError:
-        #print(f"{process_name} is not running")
+        #print(f"'{process_name}' is not running")
         pass
 
     except KeyboardInterrupt:
         if error_messages_callback:
             error_messages_callback("Cancelling all tasks")
         else:
             print("Cancelling all tasks")
@@ -2898,15 +2898,15 @@
             do_translate = True
         else:
             do_translate = False
     else:
         do_translate = False
 
     if args.list_formats:
-        print("List of supported subtitles formats:")
+        print("List of supported subtitle formats:")
         for subtitle_format in SubtitleFormatter.supported_formats:
             print(f"{subtitle_format}")
         return 0
 
     if args.format not in SubtitleFormatter.supported_formats:
         print("Subtitle format is not supported. Run with --list-formats to see all supported formats.")
         return 1
@@ -2957,36 +2957,32 @@
 
 
     if arg_filepaths:
         for argpath in arg_filepaths:
             if os.path.isfile(argpath):
                 if check_file_type(argpath, error_messages_callback=show_error_messages) == 'video':
                     media_filepaths.append(argpath)
-                    media_type = "video"
                 elif check_file_type(argpath, error_messages_callback=show_error_messages) == 'audio':
                     media_filepaths.append(argpath)
-                    media_type = "audio"
                 else:
                     invalid_media_filepaths.append(argpath)
-                    media_type = None
             else:
                 not_exist_filepaths.append(argpath)
-                media_type = None
 
         if invalid_media_filepaths:
             for invalid_media_filepath in invalid_media_filepaths:
-                msg = f"{invalid_media_filepath} is not valid media files"
+                msg = f"'{invalid_media_filepath}' is not valid media files"
                 print(msg)
 
     #print("not_exist_filepaths = %s" %(not_exist_filepaths))
 
     if not_exist_filepaths:
         if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
             for not_exist_filepath in not_exist_filepaths:
-                msg = f"{not_exist_filepath} is not exist"
+                msg = f"'{not_exist_filepath}' is not exist"
                 print(msg)
                 sys.exit(0)
 
     if not arg_filepaths and not not_exist_filepaths:
         print("No any files matching filenames you typed")
         sys.exit(0)
 
@@ -3000,76 +2996,82 @@
     dst_subtitle_filepath = None
     ffmpeg_src_language_code = None
     ffmpeg_dst_language_code = None
     embedded_media_filepath = None
 
     subtitle_format = args.format
 
-    #print(f"media_filepaths = {media_filepaths}")
-
     removed_media_filepaths = []
 
+    # CHECK SUBTITLE STREAM PART IF args.force_recognize == False
     if args.force_recognize == False:
 
         print("CHECKING EXISTING SUBTITLES STREAMS")
         print("===================================")
 
         # CHECKING ffmpeg_src_language_code SUBTITLES STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
         if do_translate == False:
 
             for media_filepath in media_filepaths:
 
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                 print(f"Checking '{media_filepath}'")
 
+                media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+                if media_type == "audio":
+                    print("Audio file won't have subtitles streams, skip checking")
+                    continue
+
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                 subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
                 if subtitle_streams_data and subtitle_streams_data != []:
 
                     src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                     if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_src_language_code.center(3)))
+                        print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : Yes")
 
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
                         src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
-                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
+                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : '{src_subtitle_filepath}'")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
 
                         # no translate process as instructed in command arguments
 
                         # if args.embed_src is True we can't embed it because dst subtitles stream already exist
                         if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                             print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
-                        # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                        # remove media_filepath from transcribe processed_list because all needed srt files already saved
                         if args.force_recognize == False:
                             if media_filepath not in removed_media_filepaths:
+                                print(f"Removing '{media_filepath}' from speech recognition process list")
                                 removed_media_filepaths.append(media_filepath)
 
+                        if os.path.isfile(src_subtitle_filepath):
+                            completed_tasks += 1
+                            #print(f"args.force_recognize == False, do_translate == False, media_type == 'video', subtitle stream = exist : completed_tasks = {completed_tasks}")
+
                     else:
-                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_src_language_code.center(3)))
+                        print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : No")
 
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
                 msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
@@ -3078,70 +3080,76 @@
 
         # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLES STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
         # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT AND THEN EMBED IT
         elif do_translate == True:
 
             for media_filepath in media_filepaths:
 
+                print(f"Checking '{media_filepath}'")
+
+                media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+                if media_type == "audio":
+                    print("Audio file won't have subtitles streams, skip checking")
+                    continue
+
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                 ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                 subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-                print(f"Checking '{media_filepath}'")
-
                 if subtitle_streams_data and subtitle_streams_data != []:
 
                     src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
                     dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
-                    # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
+                    # ffmpeg_src_language_code subtitles stream exists, we print it and extract it
                     if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_src_language_code.center(3)))
+                        print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : Yes")
 
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
                         src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
-                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
+                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : '{src_subtitle_filepath}'")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
 
-                    # ffmpeg_src_language_code subtitles stream not exist, just print it
+                    # ffmpeg_src_language_code subtitles stream is not exist, just print it
                     else:
-                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_src_language_code.center(3)))
+                        print(f"Is '{ffmpeg_src_language_code}' subtitles stream exist         : No")
 
-                    # ffmpeg_dst_language_code subtitles stream exist, so we print it and extract it
+                    # ffmpeg_dst_language_code subtitles stream exists, so we print it and extract it
                     if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_dst_language_code.center(3)))
+                        print(f"Is '{ffmpeg_dst_language_code}' subtitles stream exist         : Yes")
 
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in dst_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
                         dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
 
-                        print(f"Extracting '{ffmpeg_dst_language_code}'subtitles stream as     : {dst_subtitle_filepath}")
+                        print(f"Extracting '{ffmpeg_dst_language_code}'subtitles stream as     : '{dst_subtitle_filepath}'")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(dst_subtitle_filepath)
 
-                    # ffmpeg_dst_language_code subtitles stream not exist, just print it
+                    # ffmpeg_dst_language_code subtitles stream is not exist, just print it
                     else:
-                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_dst_language_code.center(3)))
+                        print(f"Is '{ffmpeg_dst_language_code}' subtitles stream exist         : No")
 
                     # ffmpeg_src_language_code subtitles stream = not exist,
                     # ffmpeg_dst_language_code subtitles stream = exist
                     # so we translate it from 'args.dst_language' to 'args.src_language'
                     if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
 
                         if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
@@ -3161,17 +3169,18 @@
                             src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(src_subtitle_filepath)
 
                             print(f"Translated subtitles file saved as      : '{src_subtitle_filepath}'")
 
-                            # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                            # remove media_filepath from transcribe processed_list because all needed srt files already saved
                             if args.force_recognize == False:
                                 if media_filepath not in removed_media_filepaths:
+                                    print(f"Removing '{media_filepath}' from speech recognition process list")
                                     removed_media_filepaths.append(media_filepath)
 
                             # if args.embed_src is True then we embed the translated srt into media_filepath
                             if args.embed_src == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
 
                                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
@@ -3224,17 +3233,18 @@
                             dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
 
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(dst_subtitle_filepath)
 
                             print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
 
-                            # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                            # remove media_filepath from transcribe processed_list because all needed srt files already saved
                             if args.force_recognize == False:
                                 if media_filepath not in removed_media_filepaths:
+                                    print(f"Removing '{media_filepath}' from speech recognition process list")
                                     removed_media_filepaths.append(media_filepath)
 
                             # if args.embed_src is True we can't embed it because dst subtitles stream already exist
                             if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                 print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
                             # if args.embed_dst is True then we embed that translated srt into media_filepath
@@ -3263,93 +3273,128 @@
                                     os.remove(dst_tmp_output)
 
                                 if os.path.isfile(embedded_media_filepath):
                                     print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
 
                     # ffmpeg_dst_language_code subtitles stream = exist
                     # ffmpeg_src_language_code subtitles stream = exist
-                    # remove media_filepath from proceed list
+                    # remove media_filepath from processed list
                     elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
-                        # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                        # remove media_filepath from transcribe processed_list because all needed srt files already saved
                         if args.force_recognize == False:
                             if media_filepath not in removed_media_filepaths:
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
+                    if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
+                        if args.force_recognize == False:
+                            completed_tasks += 1
+                            #print(f"\nargs.force_recognize == False, do_translate == True, media_type == 'video', subtitle stream = exist : completed_tasks = {completed_tasks}\n")
 
-            # modifying  media_filepaths list as transcribe proceed_list (if args.force_recognize is false)
-            if removed_media_filepaths:
-                for removed_media_filepath in removed_media_filepaths:
-                    if removed_media_filepath in media_filepaths:
-                        media_filepaths.remove(removed_media_filepath)
+                print("")
+            print("")
 
-            # nothing to process
+            # nothing to process with speech reconition
             if not media_filepaths:
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
                 msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
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
 
+    # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to processed with transcribe
+    for media_filepath in media_filepaths:
+
+        print(f"Checking '{media_filepath}'")
+
+        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+        if media_type == "video" and args.force_recognize == True:
+
+            force_recognize_media_file_format = None
+
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
 
-            widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-            subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-            tmp_output = subtitle_remover(media_filepath)
-            pbar.finish()
+            if subtitle_streams_data and subtitle_stream_parser.timed_subtitles_of_index(1) != []:
 
-            if os.path.isfile(tmp_output):
-                shutil.copy(tmp_output, subtitle_removed_media_filepath)
-                os.remove(tmp_output)
+                tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{force_recognize_media_file_format}"
+                subtitle_removed_media_filepath = f"{base}.force.recognize.{force_recognize_media_file_format}"
 
-                proceed_list.append(subtitle_removed_media_filepath)
+                widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                tmp_output = subtitle_remover(media_filepath)
+                pbar.finish()
 
-            print(f"Subtitle removed {media_type} file saved as    : '{subtitle_removed_media_filepath}'")
-            print("")
+                if os.path.isfile(tmp_output):
+                    shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                    os.remove(tmp_output)
 
-    # if args.force_recognize is false then we just use modified media_filepaths list
-    else:
-        proceed_list = media_filepaths
+                    processed_list.append(subtitle_removed_media_filepath)
+
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
             widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
             wav_filepath, sample_rate = wav_converter(media_filepath)
             pbar.finish()
 
@@ -3406,26 +3451,49 @@
                     pbar.finish()
 
                     base, ext = os.path.splitext(media_filepath)
                     dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
                     translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                     translation_writer.write(dst_subtitle_filepath)
 
-                if do_translate == True:
                     print(f"Original subtitles file saved as        : '{src_subtitle_filepath}'")
                     print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
-                else:
+
+                    if media_type == "audio":
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
+
+                    elif media_type == "video" and args.embed_src == False and args.embed_dst == False:
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
+
+                elif do_translate == False:
                     print(f"Subtitles file saved as                 : '{src_subtitle_filepath}'")
 
+                    if media_type == "audio":
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
+
+                    elif media_type == "video" and args.embed_src == False:
+                        completed_tasks += 1
+                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'video', args.embed_src == False : completed_tasks = {completed_tasks}\n")
+
 
                 # EMBEDDING SUBTITLES FILE
+
                 embedded_media_filepath = None
+
                 if do_translate == False:
 
-                    if args.embed_src == True:
+                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+                    if media_type == "audio" and args.embed_src == True:
+                        print("Subtitles can only be embedded into video file, not audio file")
+
+                    if media_type == "video" and args.embed_src == True:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                         base, ext = os.path.splitext(media_filepath)
 
                         if ext[1:] == "ts":
                             media_format = "mp4"
@@ -3440,19 +3508,29 @@
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(src_tmp_output):
                             shutil.copy(src_tmp_output, embedded_media_filepath)
                             os.remove(src_tmp_output)
-                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+
+                    if media_type == "video" and args.embed_src == False:
+                        completed_tasks += 1
+                        #print(f"\ndo_translate == False, media_type == 'video' : completed_tasks = {completed_tasks}\n")
+
 
                 elif do_translate == True:
 
-                    if args.embed_src == True and args.embed_dst == True:
+                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+                    if media_type == "audio" and (args.embed_src == True or args.embed_src == True):
+                        print("Subtitles can only be embedded into video file, not audio file")
+
+                    if media_type == "video" and args.embed_src == True and args.embed_dst == True:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                         base, ext = os.path.splitext(media_filepath)
 
                         if ext[1:] == "ts":
@@ -3467,42 +3545,42 @@
                         '''
                         # USING FUNCTION
                         src_tmp_output = embed_subtitle_into_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
                         if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                             src_dst_tmp_output = embed_subtitle_into_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
                         '''
 
-
                         # USING CLASS
                         widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                             widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=100).start()
                             subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             src_dst_tmp_output = subtitle_embedder(src_tmp_output)
                             pbar.finish()
 
-
                         if os.path.isfile(src_dst_tmp_output):
                             shutil.copy(src_dst_tmp_output, embedded_media_filepath)
-                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
                         else:
                             print("Unknown error!")
 
                         if os.path.isfile(src_dst_tmp_output):
                             os.remove(src_dst_tmp_output)
                         if os.path.isfile(src_tmp_output):
                             os.remove(src_tmp_output)
 
-                    elif args.embed_src == True and args.embed_dst == False:
+                    elif media_type == "video" and args.embed_src == True and args.embed_dst == False:
 
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                         base, ext = os.path.splitext(media_filepath)
 
                         if ext[1:] == "ts":
                             media_format = "mp4"
@@ -3517,19 +3595,21 @@
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(src_tmp_output):
                             shutil.copy(src_tmp_output, embedded_media_filepath)
                             os.remove(src_tmp_embedded_media_filepath)
-                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
                         else:
                             print("Unknown error!")
 
-                    elif args.embed_src == False and args.embed_dst == True:
+                    elif media_type == "video" and args.embed_src == False and args.embed_dst == True:
 
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                         base, ext = os.path.splitext(media_filepath)
 
                         if ext[1:] == "ts":
                             media_format = "mp4"
@@ -3544,41 +3624,33 @@
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                         dst_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
                         if os.path.isfile(dst_tmp_output):
                             shutil.copy(dst_tmp_output, embedded_media_filepath)
                             os.remove(dst_tmp_output)
-                            print(f"Subtitle embedded {media_type} file saved as   : '{embedded_media_filepath}'")
+                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                            completed_tasks += 1
+                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
                         else:
                             print("Unknown error!")
 
-                if do_translate == False:
-                    if args.embed_src == True:
-                        if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                            completed_tasks += 1
-                    else:
-                        completed_tasks += 1
+            print('')
 
-                elif do_translate == True:
-                    if args.embed_src == True or args.embed_dst == True:
-                        if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                            completed_tasks += 1
-                    else:
-                        completed_tasks += 1
+            #print(f"len(media_filepaths) = {len(media_filepaths)}")
+            #print(f"completed_tasks = {completed_tasks}\n")
 
-                print('')
-                if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
-                    transcribe_end_time = time.time()
-                    transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
-                    transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
-                    transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
-                    hour, minute, second = transcribe_elapsed_time_str.split(":")
-                    msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
-                    print(msg)
+            if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
+                transcribe_end_time = time.time()
+                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+                hour, minute, second = transcribe_elapsed_time_str.split(":")
+                msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
+                print(msg)
 
         except KeyboardInterrupt:
             pbar.finish()
             pool.terminate()
             pool.close()
             pool.join()
             print("Cancelling all tasks")
```

### Comparing `autosrt-1.4.6/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.7/autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.6
+Version: 1.4.7
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.6/setup.py` & `autosrt-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/test/test1.py` & `autosrt-1.4.7/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/test/test2.py` & `autosrt-1.4.7/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/test/test3.py` & `autosrt-1.4.7/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.6/test/test4.py` & `autosrt-1.4.7/test/test4.py`

 * *Files identical despite different names*

