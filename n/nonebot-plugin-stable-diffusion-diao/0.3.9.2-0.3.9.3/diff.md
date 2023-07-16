# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar", last modified: Sat Jul 15 02:49:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.3.tar", last modified: Sun Jul 16 04:28:55 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.2/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    26312 2023-07-15 02:38:33.308037 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15932 2023-07-15 02:22:12.577508 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    17940 2023-07-15 02:42:00.196730 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11298 2023-07-15 02:23:36.589787 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    38132 2023-07-15 02:28:37.087912 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4417 2023-07-15 02:39:45.240818 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      728 2023-07-15 02:49:05.693126 nonebot_plugin_stable_diffusion_diao-0.3.9.2/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.3/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    26573 2023-07-16 04:26:42.432587 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16093 2023-07-16 04:28:25.749676 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5993 2023-07-16 04:10:50.146982 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17941 2023-07-16 03:48:35.050825 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-16 04:01:07.429355 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11298 2023-07-15 02:23:36.589787 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    41763 2023-07-16 04:24:54.907060 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4670 2023-07-16 04:27:02.446129 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-07-16 04:28:55.835601 nonebot_plugin_stable_diffusion_diao-0.3.9.3/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.3/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                            type=str, help="使用的lora", dest="lora")
 aidraw_parser.add_argument("-hr",
                            type=float, help="高清修复倍率", dest="hiresfix_scale")
 aidraw_parser.add_argument("-m",
                            type=str, help="更换模型", dest="model")
 aidraw_parser.add_argument("-match_off","-match-off",
                            action="store_true", help="关闭自动匹配", dest="match")
-aidraw_parser.add_argument("-sr_on","-sr-on",
+aidraw_parser.add_argument("-sr_on", "-sr-on", "-sr",
                            action="store_true", help="图片生产后再次超分", dest="sr")
 
 
 async def get_message_at(data: str) -> int:
     '''
     获取at列表
     :param data: event.json()
@@ -243,14 +243,15 @@
                         new_tags_list = []
                         tags_list = org_tag_list
                         fifo.extra_info += "自动匹配到的模型过多\n已关闭自动匹配功能"
                         model_info = ""
                         raise RuntimeError("匹配到很多lora")
                     fifo.extra_info += f"{model_info}\n"
             except Exception as e:
+                logger.warning(str(traceback.print_exc()))
                 logger.warning(f"tag自动匹配失效,出现问题的: {tag}\n或者是prompt里自动匹配到的模型过多")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
             tags_list: str = await prepocess_tags(tags_list)
         except Exception as e:
             logger.debug(str(e))
             await aidraw.finish("tag处理失败!可能是翻译API错误, 请稍后重试, 或者使用英文重试")
@@ -470,48 +471,50 @@
         id = fifo.user_id if config.novelai_antireport else bot.self_id
         if isinstance(event, PrivateMessageEvent):
             nickname = event.sender.nickname
         else:
             resp = await bot.get_group_member_info(group_id=fifo.group_id, user_id=fifo.user_id)
             nickname = resp["card"] or resp["nickname"]
         # 开始生成
-        logger.info(
-            f"队列剩余{wait_len()}人 | 开始生成：{fifo}")
         try:
             im = await _run_gennerate(fifo)
         except Exception as e:
             logger.exception("生成失败")
             message = f"生成失败，"
             for i in e.args:
                 message += str(i)
             await bot.send(event=event, 
                            message=message,
             )
         else:
-            logger.info(f"队列剩余{wait_len()}人 | 生成完毕：{fifo}")
             pic_message = im[1]
-            res_msg = (f"分辨率:({fifo.width}x{fifo.hiresfix_scale})x({fifo.height}x{fifo.hiresfix_scale})") if (
+            res_msg = (f"分辨率:{fifo.width}x{fifo.hiresfix_scale}x{fifo.height}x{fifo.hiresfix_scale}") if (
                         fifo.hiresfix and fifo.img2img is False) else (
                         f"分辨率:{fifo.width}x{fifo.height}"
                         )
+            if fifo.sr:
+                sr_scale = config.novelai_SuperRes_generate_payload["upscaling_resize"]
+                res_msg = (f"分辨率:({fifo.width}x{fifo.hiresfix_scale}x{fifo.height}x{fifo.hiresfix_scale})x{sr_scale}")
             try:
                 if len(fifo.extra_info) != 0:
                     fifo.extra_info += "\n使用'-match_off'参数以关闭自动匹配功能\n"
                 message_data = await bot.send(event=event, 
-                                          message=pic_message+f"模型:{os.path.basename(fifo.model)}\n{fifo.img_hash}", 
+                                          message=pic_message+f"模型:{os.path.basename(fifo.model)}\n{fifo.img_hash}",
+                                          reply_message=True, 
                                           at_sender=True, 
             ) if (
                     await config.get_value(fifo.group_id, "pure")) or (
                     await config.get_value(fifo.group_id, "pure") is None and config.novelai_pure) else (
                     await send_forward_msg(bot=bot, event=event, name=nickname, uin=id, msgs=im)
                 )
 
             except ActionFailed:
                 message_data = await bot.send(event=event, 
-                                             message=pic_message, 
+                                             message=pic_message,
+                                             reply_message=True, 
                                              at_sender=True, 
                                 )
 
             revoke = await config.get_value(fifo.group_id, "revoke")
             if revoke:
                 message_id = message_data["message_id"]
                 loop = get_running_loop()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 import ast
 
 import aiohttp
 from nonebot import get_driver
 from nonebot.log import logger
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageEvent, PrivateMessageEvent
+from nonebot import logger
 from datetime import datetime
 from ..config import config, redis_client
-from ..utils import png2jpg, unload_and_reload
+from ..utils import png2jpg, unload_and_reload, get_generate_info
 from ..utils.data import shapemap
 from ..utils.load_balance import sd_LoadBalance
 
 
 class AIDRAW_BASE:
     max_resolution: int = 16
     sampler: str
@@ -252,15 +253,18 @@
     async def post_(self, header: dict, post_api: str, payload: dict):
         """
         向服务器发送请求的核心函数，不要直接调用，请使用post函数
         :header: 请求头
         :post_api: 请求地址
         :json: 请求体
         """
-        # 请求交互      
+        # 请求交互
+        generate_info = get_generate_info(self, "开始生成")
+        logger.info(
+            f"{generate_info}")
         async with aiohttp.ClientSession(headers=header, timeout=aiohttp.ClientTimeout(total=1800)) as session:
             # 向服务器发送请求
             async with session.post(post_api, json=payload) as resp:
                 if resp.status not in [200, 201]:
                     resp_dict = json.loads(await resp.text())
                     logger.error(resp_dict)
                     if resp_dict["error"] == "OutOfMemoryError":
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .base import AIDRAW_BASE
 from ..config import config
 import time
 from ..utils.load_balance import sd_LoadBalance, get_vram
+from ..utils import get_generate_info
 from nonebot import logger
 import json, aiofiles
 import asyncio
 import traceback
 
 header = {
                 "content-type": "application/json",
@@ -128,8 +129,11 @@
                 try:
                     self.model = resp_json["sd_model_checkpoint"]
                 except Exception:
                     self.model = ""
                 self.vram = resp_list[1]
                 break
                 
+        generate_info = get_generate_info(self, "生成完毕")
+        logger.info(
+            f"{generate_info}")
         return self.result
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         "hr_upscaler": "Lanczos",  # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
         "hr_second_pass_steps": 7,  # 高清修复步数, 个人建议7是个不错的选择, 速度质量都不错
     } # 以上为个人推荐值
     novelai_SuperRes_MaxPixels: int = 2000  # 超分最大像素值, 对应(值)^2, 为了避免有人用超高分辨率的图来超分导致爆显存(
     novelai_SuperRes_generate: bool = False  # 图片生成后是否再次进行一次超分
     novelai_SuperRes_generate_payload: dict = {
         "upscaling_resize": 1.2,  # 超分倍率, 为长宽分辨率各X1.2
-        "upscaler_1": "ScuNET",  # 第一次超分使用的方法
+        "upscaler_1": "Lanczos",  # 第一次超分使用的方法
         "upscaler_2": "R-ESRGAN 4x+ Anime6B",  # 第二次超分使用的方法
         "extras_upscaler_2_visibility": 0.6  # 第二层upscaler力度
     } # 以上为个人推荐值
     novelai_ControlNet_post_method: int = 0
     novelai_size_org: int = 640  # 最大分辨率
     if novelai_hr:
         novelai_size: int = novelai_size_org
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 @deepdanbooru.handle()
 async def deepdanbooru_handle(event: MessageEvent, bot: Bot):
     h_ = None
     url = ""
     reply = event.reply
+    for seg in event.message['image']:
+        url = seg.data["url"]
     if reply:
         for seg in reply.message['image']:
             url = seg.data["url"]
-    for seg in event.message['image']:
-        url = seg.data["url"]
     if url:
         async with aiohttp.ClientSession() as session:
             logger.info(f"正在获取图片")
             async with session.get(url) as resp:
                 bytes = await resp.read()
         str_img = str(base64.b64encode(bytes), "utf-8")
         start = "data:image/jpeg;base64,"
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,16 @@
 find_pic = on_command("找图片", aliases={"图片"})
 word_frequency_count = on_command("词频统计", aliases={"tag统计"})
 run_screen_shot = on_command("运行截图", aliases={"状态"}, block=False, priority=2)
 audit = on_command("审核")
 genera_aging = on_command("再来一张")
 reload_ = on_command("卸载模型", aliases={"释放显存"})
 style_ = on_command("预设")
+rembg = on_command("去背景", aliases={"rembg", "抠图"})
+read_png_info = on_command("读图", aliases={"读png", "读PNG"})
 
 more_func_parser, style_parser = ArgumentParser(), ArgumentParser()
 more_func_parser.add_argument("-i", "--index", type=int, help="设置索引", dest="index")
 more_func_parser.add_argument("-v", "--value", type=str, help="设置值", dest="value")
 more_func_parser.add_argument("-s", "--search", type=str, help="搜索设置名", dest="search")
 style_parser.add_argument("tags", type=str, nargs="*", help="正面提示词")
 style_parser.add_argument("-f", "--find", type=str, help="寻找预设", dest="find_style_name")
@@ -421,15 +423,15 @@
         state['super_res'] = super_res
     pass    
 
 
 @super_res.got("super_res", "请发送你要修复的图片")
 async def abc(event: MessageEvent, bot: Bot, msg: Message = Arg("super_res")):
     img_url_list = []
-    img_base64_list = []
+    img_byte_list = []
 
     if msg[0].type == "image":
         if len(msg) > 1:
             for i in msg:
                 img_url_list.append(i.data["url"])
                 upsale = 0
         else:
@@ -437,25 +439,25 @@
             upsale = 1
             
         for i in img_url_list:
             qq_img = await download_img(i)
             qq_img, text_msg, status_code = await super_res_api_func(qq_img[1], upsale)
             if status_code not in [200, 201]:
                 await super_res.finish(f"出错了,错误代码{status_code},请检查服务器")
-            img_base64_list.append(qq_img)
-        if len(img_base64_list) == 1:
-                img_mes = MessageSegment.image(img_base64_list[0])
+            img_byte_list.append(qq_img)
+        if len(img_byte_list) == 1:
+                img_mes = MessageSegment.image(img_byte_list[0])
                 await bot.send(event=event, 
                                message=img_mes+text_msg, 
                                at_sender=True, 
                                reply_message=True
                                ) 
         else:
             img_list = []
-            for i in img_base64_list:
+            for i in img_byte_list:
                 img_list.append(f"{MessageSegment.image(i)}\n{text_msg}")
             await send_forward_msg(bot, 
                                    event, 
                                    event.sender.nickname, 
                                    event.user_id, 
                                    img_list
                                    )
@@ -812,19 +814,19 @@
         await run_screen_shot.finish("未启动屏幕截图")
 
 
 @audit.handle()
 async def _(event: MessageEvent, bot: Bot):
     url = ""
     reply = event.reply
+    for seg in event.message['image']:
+        url = seg.data["url"]
     if reply:
         for seg in reply.message['image']:
             url = seg.data["url"]
-    for seg in event.message['image']:
-        url = seg.data["url"]
     if url:
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
                 bytes = await resp.read()
         img_base64 = str(base64.b64encode(bytes), "utf-8")
         message = await pic_audit_standalone(img_base64)
         await bot.send(event, message, at_sender=True, reply_message=True)
@@ -932,7 +934,98 @@
             await style_.finish("参数不完整, 请检查后重试")
     else:
         for style in style_list:
             name, tags, ntags = style["name"], style["prompt"], style["negative_prompt"]
             message_list.append(f"预设名称: {name}\n正面提示词: {tags}\n负面提示词: {ntags}\n")
         await risk_control(bot, event, message_list, True)
     
+
+@rembg.handle()
+async def rm_bg(state: T_State, rmbg: Message = CommandArg()):
+    if rmbg:
+        state['rmbg'] = rmbg
+    pass    
+
+
+@rembg.got("rmbg", "请发送你要去背景的图片")
+async def _(event: MessageEvent, bot: Bot, msg: Message = Arg("rmbg")):
+    img_url_list = []
+    img_byte_list = []
+
+    if msg[0].type == "image":
+        if len(msg) > 1:
+            for i in msg:
+                img_url_list.append(i.data["url"])
+        else:
+            img_url_list.append(msg[0].data["url"])
+        
+        for i in img_url_list:
+            qq_img = await download_img(i)
+            fifo = AIDRAW()
+            await fifo.load_balance_init()
+            payload = {
+            "input_image": qq_img[0],
+            "model": "isnet-anime",
+            "alpha_matting": "true",
+            "alpha_matting_foreground_threshold": 255,
+            "alpha_matting_background_threshold": 50,
+            "alpha_matting_erode_size": 20
+            }
+            resp_data, status_code = await aiohttp_func("post", f"http://{fifo.backend_site}/rembg", payload)
+            if status_code not in [200, 201]:
+                await rembg.finish(f"出错了,错误代码{status_code},请检查服务器")
+            img_byte_list.append(base64.b64decode(resp_data["image"]))
+        if len(img_byte_list) == 1:
+                img_mes = MessageSegment.image(img_byte_list[0])
+                await bot.send(event=event, 
+                               message=img_mes,
+                               at_sender=True, 
+                               reply_message=True
+                               ) 
+        else:
+            img_list = []
+            for i in img_byte_list:
+                img_list.append(f"{MessageSegment.image(i)}")
+            await send_forward_msg(bot, 
+                                   event, 
+                                   event.sender.nickname, 
+                                   event.user_id, 
+                                   img_list
+                                   )
+            
+    else:
+        await rembg.reject("请重新发送图片")
+        
+
+@read_png_info.handle()
+async def __(state: T_State, png: Message = CommandArg()):
+    if png:
+        state['png'] = png
+    pass    
+
+@read_png_info.got("png", "请发送你要读取的图片,请注意,请发送原图")
+async def __(event: MessageEvent, bot: Bot):
+    reply = event.reply
+    for seg in event.message['image']:
+        url = seg.data["url"]
+    if reply:
+        for seg in reply.message['image']:
+            url = seg.data["url"]
+    if url:
+        fifo = AIDRAW()
+        await fifo.load_balance_init()
+        img, _ = await download_img(url)
+        payload = {
+            "image": img
+        }
+        resp_data, status_code = await aiohttp_func("post", f"http://{fifo.backend_site}/sdapi/v1/png-info", payload)
+        if status_code not in [200, 201]:
+            await read_png_info.finish(f"出错了,错误代码{status_code},请检查服务器")
+        info = resp_data["info"]
+        if info == "":
+            await read_png_info.finish("图片里面没有元数据信息欸\n是不是没有发送原图")
+        else:
+            parameters = resp_data["items"]["parameters"]
+            await risk_control(bot, event, [f"这是图片的元数据信息: {info}\n", f"参数: {parameters}"], True)
+    else:
+        await read_png_info.reject("请重新发送图片")
+
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,8 +103,16 @@
 def tags_to_list(tags: str) -> list:
     separators = ['，', '。', ","]
     for separator in separators:
         tags = tags.replace(separator, separators[0])
     tag_list = tags.split(separators[0])
     tag_list = [tag.strip() for tag in tag_list if tag.strip()]
     tag_list = list(filter(None, tag_list))
-    return tag_list
+    return tag_list
+
+
+def get_generate_info(fifo, info):
+    generate_info = f"{info}\n"
+    fifo_dict = dict(fifo)
+    for key, value in zip(list(fifo_dict.keys()), list(fifo_dict.values())):
+        generate_info += f"[{key}]: {value}\n"
+    return generate_info
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.2/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.2"
+version = "0.3.9.3"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

