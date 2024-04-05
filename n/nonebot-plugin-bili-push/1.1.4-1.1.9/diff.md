# Comparing `tmp/nonebot_plugin_bili_push-1.1.4.tar.gz` & `tmp/nonebot_plugin_bili_push-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-1.1.4.tar", last modified: Wed Oct 18 13:21:48 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-1.1.9.tar", last modified: Sun Oct 29 14:21:35 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-1.1.4.tar` & `nonebot_plugin_bili_push-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-10-18 13:21:48.994075 nonebot_plugin_bili_push-1.1.4/
--rw-rw-rw-   0        0        0     1096 2023-10-18 13:20:23.000000 nonebot_plugin_bili_push-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      527 2023-10-18 13:21:48.994075 nonebot_plugin_bili_push-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2475 2023-10-13 16:04:57.000000 nonebot_plugin_bili_push-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-10-18 13:21:48.985466 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0   151661 2023-10-18 13:07:28.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-18 13:21:48.992074 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      527 2023-10-18 13:21:48.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-10-18 13:21:48.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-18 13:21:48.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-10-18 13:21:48.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-10-18 13:21:48.000000 nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-18 13:21:48.995673 nonebot_plugin_bili_push-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-10-18 13:07:28.000000 nonebot_plugin_bili_push-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-29 14:21:35.755531 nonebot_plugin_bili_push-1.1.9/
+-rw-rw-rw-   0        0        0     1096 2023-10-18 13:20:23.000000 nonebot_plugin_bili_push-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      277 2023-10-29 14:21:35.754528 nonebot_plugin_bili_push-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2579 2023-10-25 14:17:26.000000 nonebot_plugin_bili_push-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-29 14:21:35.746606 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0   155615 2023-10-29 14:14:11.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-29 14:21:35.752470 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-10-29 14:21:35.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-10-29 14:21:35.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-29 14:21:35.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-10-29 14:21:35.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-10-29 14:21:35.000000 nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-29 14:21:35.755531 nonebot_plugin_bili_push-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-10-29 14:20:29.000000 nonebot_plugin_bili_push-1.1.9/setup.py
```

### Comparing `nonebot_plugin_bili_push-1.1.4/LICENSE` & `nonebot_plugin_bili_push-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-1.1.4/README.md` & `nonebot_plugin_bili_push-1.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # nonebot-plugin-bili-push
 
 B 订阅推送插件
 
-支持 OB11、Red 协议
+仅支持 OB11 适配器
+
+(kook 适配器请前往另一个仓库查看，但不建议使用-[bili_push for kook](https://github.com/SuperGuGuGu/nonebot_plugin_bili_push_kook))
 
 ## 示例
 
-![输入图片描述](README_md_files/9cf89890-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
-![输入图片描述](README_md_files/7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
+![输入图片描述](README_md_files/9cf89890-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image) ![输入图片描述](README_md_files/7fd7ee50-0952-11ee-8733-25d9c7397331.jpeg?v=1&type=image)
 
 ## 安装
 
 （以下方法二选一）
 
 一.命令行安装：
 
@@ -53,14 +54,16 @@
 
 详细配置方法- [详细配置](https://github.com/SuperGuGuGu/nonebot_plugin_bili_push/blob/master/Config.md)
 
 ## To-Do
 
 🔵 接下来：
 
+- [ ] 保存直播推送封面，推送样式修改
+
 - [ ] 配置仅直播推送或仅动态推送（接下来更新）
 
 - [ ] 开播添加 at 全体成员（接下来更新）
 
 - [ ] 对话式配置（接下来更新）
 
 - [ ] 推送黑名单（识别到文字或类型的时候不进行推送）
@@ -79,25 +82,21 @@
 
 - [ ] 增加多种适配器连接
 
 - [ ] ~~将请求 api 改为异步（无限期延迟~~
 
 🟢 已完成：
 
-- [x] 对 Red 协议支持
+- [x] 修复直播订阅
 
 - [x] 对海外服务器支持
 
-- [x] 动态获取不到名字，导致关注报错
-
 - [x] 配置推送样式
 
-- [x] 修复文件下载出错导致文件加载报错
-
-- [x] 设置默认字体。在禁用 api 时候使用默认字体
+- [x] 设置默认字体。在禁用 插件 api 的时候使用默认字体
 
 - [x] 单 nb 对接多 q 的兼容
 
 ## 灵感来源
 
 Mirai 动态绘制插件 [BilibiliDynamic MiraiPlugin](https://github.com/Colter23/bilibili-dynamic-mirai-plugin)
```

### Comparing `nonebot_plugin_bili_push-1.1.4/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-1.1.9/nonebot_plugin_bili_push/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,21 @@
     # 把api调用的代码放在一起，方便下一步进行异步开发
     if type == "json":
         if post_json is None:
             return json.loads(httpx.get(url).text)
         else:
             return json.loads(httpx.post(url, json=post_json).text)
     elif type == "image":
-        try:
-            image = Image.open(BytesIO(httpx.get(url).content))
-        except Exception as e:
+        if url in ["none", "None"] or url is None:
             image = draw_text("获取图片出错", 50, 10)
+        else:
+            try:
+                image = Image.open(BytesIO(httpx.get(url).content))
+            except Exception as e:
+                image = draw_text("获取图片出错", 50, 10)
         return image
     elif type == "file":
         cache_file_path = file_path + "cache"
         try:
             # 这里不能用httpx。用就报错。
             with open(cache_file_path, "wb") as f, requests.get(url) as res:
                 f.write(res.content)
@@ -169,54 +172,23 @@
 try:
     maximum_send = config.bilipush_maximum_send
     if maximum_send == 0:
         maximum_send = 99
 except Exception as e:
     maximum_send = 5
 # 配置10：
-# debug_log
+try:
+    beta_test = config.bilipush_beta_test
+except Exception as e:
+    beta_test = False
 # 配置11：
 try:
     push_style = config.bilipush_push_style
     if push_style == "":
         push_style = "[绘图][标题][链接]"
-    else:
-        # 检查配置是否正确
-        try:
-            # 替换同义符号
-            push_style = push_style.replace("【", "[")
-            push_style = push_style.replace("】", "]")
-            push_style = push_style.replace("（", "[")
-            push_style = push_style.replace("）", "]")
-            push_style = push_style.replace("{", "[")
-            push_style = push_style.replace("}", "]")
-            cache_push_style = push_style
-            num = 10
-            while num > 0:
-                num -= 1
-                if cache_push_style.startswith("[绘图]"):
-                    cache_push_style = cache_push_style.removeprefix("[绘图]")
-                elif cache_push_style.startswith("[标题]"):
-                    cache_push_style = cache_push_style.removeprefix("[标题]")
-                elif cache_push_style.startswith("[链接]"):
-                    cache_push_style = cache_push_style.removeprefix("[链接]")
-                elif cache_push_style.startswith("[内容]"):
-                    cache_push_style = cache_push_style.removeprefix("[内容]")
-                elif cache_push_style.startswith("[图片]"):
-                    cache_push_style = cache_push_style.removeprefix("[图片]")
-                elif cache_push_style == "":
-                    num = 0
-                else:
-                    logger.error("读取动态推送样式出错，请检查配置是否正确")
-            if cache_push_style != "":
-                logger.error("读取动态推送样式出错，请检查配置是否正确")
-                logger.error("正在读取默认配置[绘图][标题][链接]")
-                push_style = "[绘图][标题][链接]"
-        except Exception as e:
-            logger.error("读取动态推送样式出错，请检查配置是否正确")
 except Exception as e:
     push_style = "[绘图][标题][链接]"
 
 # 插件元信息，让nonebot读取到这个插件是干嘛的
 __plugin_meta__ = PluginMetadata(
     name="bili_push",
     description="推送b站动态",
@@ -2059,15 +2031,15 @@
 
 
 get_new = on_command("最新动态", aliases={'添加订阅', '删除订阅', '查看订阅', '帮助'}, block=False)
 
 
 @get_new.handle()
 async def bili_push_command(bot: Bot, messageevent: MessageEvent):
-    logger.info("bili_push_command_1.1.4")
+    logger.info("bili_push_command_1.1.9")
     botid = str(bot.self_id)
     bot_type = nonebot.get_bot(botid).type
     if bot_type != "OneBot V11":
         logger.error("暂不支持的适配器")
         await get_new.finish(MessageSegment.text("暂不支持的适配器"))
     returnpath = "None"
     message = " "
@@ -2076,18 +2048,23 @@
     if isinstance(messageevent, GroupMessageEvent):
         # 群消息才有群号
         groupcode = messageevent.group_id
         groupcode = str(groupcode)
     else:
         # 这是用户qq号
         groupcode = messageevent.get_user_id()
-        groupcode = 'p' + str(groupcode)
+        groupcode = "p" + str(groupcode)
     groupcode = "g" + groupcode
     msg = messageevent.get_message()
     msg = re.sub(u"\\[.*?]", "", str(msg))
+    msg = msg.replace("'", "“")
+    msg = msg.replace('"', "“")
+    msg = msg.replace("(", "（")
+    msg = msg.replace(")", "）")
+
     commands = []
     if ' ' in msg:
         messages = msg.split(' ', 1)
         for command in messages:
             commands.append(command)
     else:
         commands.append(msg)
@@ -2101,56 +2078,81 @@
         command2 = commands[1]
     else:
         command2 = ''
 
     date_year = str(time.strftime("%Y", time.localtime()))
     date_month = str(time.strftime("%m", time.localtime()))
     date_day = str(time.strftime("%d", time.localtime()))
-    cachepath = basepath + f"cache/draw/{date_year}/{date_month}/{date_day}/"
+    cachepath = f"{basepath}cache/draw/{date_year}/{date_month}/{date_day}/"
 
     # 新建数据库
     # 读取数据库列表
     conn = sqlite3.connect(livedb)
     cursor = conn.cursor()
     cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
     datas = cursor.fetchall()
     # 数据库列表转为序列
     tables = []
     for data in datas:
         if data[1] != "sqlite_sequence":
             tables.append(data[1])
-    # 检查是否创建订阅数据库2
-    if "subscriptionlist2" not in tables:
+    # 检查是否创建订阅数据库3
+    if "subscriptionlist3" not in tables:
         # 如未创建，则创建
-        cursor.execute('create table subscriptionlist2(id INTEGER primary key AUTOINCREMENT, '
-                       'groupcode varchar(10), uid int(10))')
-        # 判断是否存在数据库1
-        if "subscriptionlist" in tables:
+        cursor.execute('create table subscriptionlist3(id INTEGER primary key AUTOINCREMENT, '
+                       'groupcode varchar(10), uid int(10), liveid int(10))')
+        # 判断是否存在旧数据库
+        if "subscriptionlist2" in tables:
+            # 如果是，则存到数据库2
+            cursor.execute("SELECT * FROM subscriptionlist2")
+            datas = cursor.fetchall()
+            for data in datas:
+                # 自动获取房间号
+                # url = ""
+                liveid = 0
+                cursor.execute(f'replace into subscriptionlist3 ("groupcode","uid","liveid") '
+                               f'values("{data[1]}",{data[2]},{liveid})')
+        elif "subscriptionlist" in tables:
             # 如果是，则存到数据库2
             cursor.execute("SELECT * FROM subscriptionlist")
             datas = cursor.fetchall()
             for data in datas:
-                cursor.execute(f'replace into subscriptionlist2 ("groupcode","uid") values("{data[1]}",{data[2]})')
+                # 自动获取房间号
+                # url = ""
+                liveid = 0
+                cursor.execute(f'replace into subscriptionlist3 ("groupcode","uid","liveid") '
+                               f'values("{data[1]}",{data[2]},{liveid})')
     cursor.close()
     conn.commit()
     conn.close()
 
     if command == "最新动态":
         logger.info("command:查询最新动态")
         code = 0
+
+        # 判断command2是否为纯数字或l开头的数字
         if "UID:" in command2:
             command2 = command2.removeprefix("UID:")
+        if command2.startswith("L"):
+            command2 = command2.replace("L", "l")
+        if command2.startswith("l"):
+            command2_cache = command2.removeprefix("l")
+        else:
+            command2_cache = command2
         try:
-            command2 = int(command2)
-            command2 = str(command2)
+            command2_cache = int(command2_cache)
+            if command2.startswith("l"):
+                command2 = f"l{command2_cache}"
+            else:
+                command2 = str(command2_cache)
         except Exception as e:
             command2 = ""
         if command2 == "":
             code = 1
-            message = "请添加uid来查询最新动态"
+            message = "请添加uid或房间id来添加订阅"
         else:
             uid = command2
             logger.info(f"开始获取信息-{uid}")
             url = 'https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/space_history?host_uid=' + uid
             returnjson = connect_api("json", url)
             if returnjson["code"] == 0:
                 logger.info('获取动态图片并发送')
@@ -2193,15 +2195,18 @@
                             msg += cache_msg
                             cache_push_style = cache_push_style.removeprefix("[内容]")
                         elif cache_push_style.startswith("[图片]"):
                             num = 0
                             for url in message_images:
                                 num += 1
                                 image = connect_api("image", url)
-                                image_path = cachepath + dynamicid + "/" + str(num) + ".png"
+                                image_path = f"{cachepath}{dynamicid}/"
+                                if not os.path.exists(image_path):
+                                    os.makedirs(image_path)
+                                image_path = f"{image_path}{num}.png"
                                 image.save(image_path)
                                 file = open(returnpath, 'br')
                                 io_file = io.BytesIO(file.read())
                                 cache_msg = MessageSegment.image(io_file)
                                 msg += cache_msg
                             cache_push_style = cache_push_style.removeprefix("[图片]")
                         elif cache_push_style == "":
@@ -2213,43 +2218,86 @@
                 logger.info('returncode!=0')
                 code = 1
                 message = "获取动态失败"
     elif command == "添加订阅":
         if qq in plugin_config("admin", groupcode):
             logger.info("command:添加订阅")
             code = 0
+
+            # 判断command2是否为纯数字或l开头的数字
             if "UID:" in command2:
                 command2 = command2.removeprefix("UID:")
+            if command2.startswith("L"):
+                command2 = command2.replace("L", "l")
+            if command2.startswith("l"):
+                command2_cache = command2.removeprefix("l")
+            else:
+                command2_cache = command2
             try:
-                command2 = int(command2)
-                command2 = str(command2)
+                command2_cache = int(command2_cache)
+                if command2.startswith("l"):
+                    command2 = f"l{command2_cache}"
+                else:
+                    command2 = str(command2_cache)
             except Exception as e:
                 command2 = ""
             if command2 == "":
                 code = 1
-                message = "请添加uid来添加订阅"
+                message = "请添加uid或房间id来添加订阅"
             else:
-                uid = command2
+                if command2.startswith("l"):
+                    liveid = command2[1:]
+                    url = f"https://api.live.bilibili.com/room/v1/Room/get_info?id={liveid}"
+                    json_data = connect_api("json", url)
+                    if json_data["code"] != 0:
+                        logger.error(f"直播api出错请将此消息反馈给开发者，liveid={liveid},msg={json_data['message']}")
+                        uid = 0
+                    else:
+                        livedata = json_data["data"]
+                        uid = livedata["uid"]
+                else:
+                    liveid = 0
+                    uid = command2
 
                 conn = sqlite3.connect(livedb)
                 cursor = conn.cursor()
-                cursor.execute("SELECT * FROM subscriptionlist2 WHERE uid = " + str(uid) +
-                               " AND groupcode = '" + str(groupcode) + "'")
+                if command2.startswith("l"):
+                    cursor.execute(
+                        f"SELECT * FROM subscriptionlist3 WHERE liveid = {command2[1:]} AND groupcode = '{groupcode}'")
+                else:
+                    cursor.execute(
+                        f"SELECT * FROM subscriptionlist3 WHERE uid = {command2} AND groupcode = '{groupcode}'")
                 subscription = cursor.fetchone()
                 cursor.close()
                 conn.commit()
                 conn.close()
 
-                if subscription is None:
+                if uid == 0:
+                    code = 1
+                    message = "订阅失败，请检查错误日志"
+                elif subscription is not None and subscription[3] is None:
+                    # 写入数据
+                    conn = sqlite3.connect(livedb)
+                    cursor = conn.cursor()
+                    cursor.execute(f"replace into subscriptionlist3 ('groupcode','uid','liveid') "
+                                   f"values('{groupcode}','{uid}','{liveid}')")
+                    cursor.close()
+                    conn.commit()
+                    conn.close()
+
+                    code = 1
+                    message = "添加直播、动态间订阅成功"
+                elif subscription is None:
                     logger.info("无订阅，添加订阅")
 
                     # 写入数据
                     conn = sqlite3.connect(livedb)
                     cursor = conn.cursor()
-                    cursor.execute(f"replace into subscriptionlist2 ('groupcode','uid') values('{groupcode}',{uid})")
+                    cursor.execute(f"replace into subscriptionlist3 ('groupcode','uid','liveid') "
+                                   f"values('{groupcode}','{uid}','{liveid}')")
                     cursor.close()
                     conn.commit()
                     conn.close()
 
                     # 将历史动态存到数据库中
                     logger.info('关注成功，将历史动态存到数据库中')
                     url = f"https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/space_history?host_uid={uid}"
@@ -2279,15 +2327,18 @@
                             cursor.close()
                             conn.commit()
                             conn.close()
 
                             drawimage = get_draw(return_datas[0], only_info=True)
                             if drawimage["code"] != 0:
                                 returnpath = drawimage["draw_path"]
-                                message = "添加订阅成功"
+                                if command2.startswith("l"):
+                                    message = "添加直播、动态订阅成功"
+                                else:
+                                    message = "添加动态订阅成功\n如需订阅直播间，请发送“/添加订阅 L”+直播间号\n例：“/添加订阅 L1234”"
                                 code = 3
                             else:
                                 code = 1
                                 message = "添加订阅成功"
                         else:
                             code = 1
                             message = "添加订阅成功。\n该up主未发布任何动态，请确认是否填写了正确的uid"
@@ -2300,56 +2351,70 @@
         else:
             code = 1
             message = "您无权限操作哦"
     elif command == "删除订阅":
         if qq in plugin_config("admin", groupcode):
             logger.info("command:删除订阅")
             code = 0
+
+            # 判断command2是否为纯数字或l开头的数字
             if "UID:" in command2:
                 command2 = command2.removeprefix("UID:")
+            if command2.startswith("L"):
+                command2 = command2.replace("L", "l")
+            if command2.startswith("l"):
+                command2_cache = command2.removeprefix("l")
+            else:
+                command2_cache = command2
             try:
-                command2 = int(command2)
-                command2 = str(command2)
+                command2_cache = int(command2_cache)
+                if command2.startswith("l"):
+                    command2 = f"l{command2_cache}"
+                else:
+                    command2 = str(command2_cache)
             except Exception as e:
                 command2 = ""
             if command2 == "":
                 code = 1
-                message = "请添加uid来删除订阅"
+                message = "请添加uid或房间id来添加订阅"
             else:
-                uid = command2
-
                 conn = sqlite3.connect(livedb)
                 cursor = conn.cursor()
-                cursor.execute(f"SELECT * FROM subscriptionlist2 WHERE uid = {uid} AND groupcode = '{groupcode}'")
+                if command2.startswith("l"):
+                    cursor.execute(
+                        f"SELECT * FROM subscriptionlist3 WHERE liveid = {command2[1:]} AND groupcode = '{groupcode}'")
+                else:
+                    cursor.execute(
+                        f"SELECT * FROM subscriptionlist3 WHERE uid = {command2} AND groupcode = '{groupcode}'")
                 subscription = cursor.fetchone()
                 cursor.close()
                 conn.commit()
                 conn.close()
 
                 if subscription is None:
                     code = 1
                     message = "未订阅该up主"
                 else:
                     subid = str(subscription[0])
                     conn = sqlite3.connect(livedb)
                     cursor = conn.cursor()
-                    cursor.execute("delete from subscriptionlist2 where id = " + subid)
+                    cursor.execute(f"delete from subscriptionlist3 where id = {subid}")
                     conn.commit()
                     cursor.close()
                     conn.close()
                     code = 1
                     message = "删除订阅成功"
         else:
             code = 1
             message = "您无权限操作哦"
     elif command == "查看订阅":
 
         conn = sqlite3.connect(livedb)
         cursor = conn.cursor()
-        cursor.execute("SELECT * FROM subscriptionlist2 WHERE groupcode = '" + groupcode + "'")
+        cursor.execute("SELECT * FROM subscriptionlist3 WHERE groupcode = '" + groupcode + "'")
         subscriptions = cursor.fetchall()
         cursor.close()
         conn.commit()
         conn.close()
         if not subscriptions:
             code = 1
             message = "该群无订阅"
@@ -2386,34 +2451,34 @@
 
 
 minute = "*/" + waittime
 
 
 @scheduler.scheduled_job("cron", minute=minute, id="job_0")
 async def run_bili_push():
-    logger.info("bili_push_1.1.4")
+    logger.info("bili_push_1.1.9")
     # ############开始自动运行插件############
     now_maximum_send = maximum_send
     date = str(time.strftime("%Y-%m-%d", time.localtime()))
     date_year = str(time.strftime("%Y", time.localtime()))
     date_month = str(time.strftime("%m", time.localtime()))
     date_day = str(time.strftime("%d", time.localtime()))
     timenow = str(time.strftime("%H-%M-%S", time.localtime()))
-    dateshort = date_year + date_month + date_day
     cachepath = basepath + f"cache/draw/{date_year}/{date_month}/{date_day}/"
-    message = ""
+    message = "none"
 
     botids = list(nonebot.get_bots())
     for botid in botids:
         bot_type = nonebot.get_bot(botid).type
         if bot_type != "OneBot V11":
             logger.info("暂不支持的适配器类型")
             continue
         botid = str(botid)
 
+        # 获取成员名单与频道名单
         friendlist = []
         grouplist = []
         friends = await nonebot.get_bot(botid).get_friend_list()
         for friendinfo in friends:
             friendlist.append(str(friendinfo["user_id"]))
 
         groups = await nonebot.get_bot(botid).get_group_list()
@@ -2427,26 +2492,40 @@
         cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
         datas = cursor.fetchall()
         # 数据库列表转为序列
         tables = []
         for data in datas:
             if data[1] != "sqlite_sequence":
                 tables.append(data[1])
-        # 检查是否创建订阅数据库2
-        if "subscriptionlist2" not in tables:
+        # 检查是否创建订阅数据库3
+        if "subscriptionlist3" not in tables:
             # 如未创建，则创建
-            cursor.execute('create table subscriptionlist2(id INTEGER primary key AUTOINCREMENT, '
-                           'groupcode varchar(10), uid int(10))')
-            # 判断是否存在数据库1
-            if "subscriptionlist" in tables:
-                # 如果是，则存到数据库2
+            cursor.execute('create table subscriptionlist3(id INTEGER primary key AUTOINCREMENT, '
+                           'groupcode varchar(10), uid int(10), liveid int(10))')
+            # 判断是否存在旧数据库
+            if "subscriptionlist2" in tables:
+                # 如果是，则存到数据库3
+                cursor.execute("SELECT * FROM subscriptionlist2")
+                datas = cursor.fetchall()
+                for data in datas:
+                    # 自动获取房间号
+                    # url = ""
+                    liveid = 0
+                    cursor.execute(f'replace into subscriptionlist3 ("groupcode","uid","liveid") '
+                                   f'values("{data[1]}",{data[2]},{liveid})')
+            elif "subscriptionlist" in tables:
+                # 如果是，则存到数据库3
                 cursor.execute("SELECT * FROM subscriptionlist")
                 datas = cursor.fetchall()
                 for data in datas:
-                    cursor.execute(f'replace into subscriptionlist2 ("groupcode","uid") values("{data[1]}",{data[2]})')
+                    # 自动获取房间号
+                    # url = ""
+                    liveid = 0
+                    cursor.execute(f'replace into subscriptionlist3 ("groupcode","uid","liveid") '
+                                   f'values("{data[1]}",{data[2]},{liveid})')
         if "livelist3" not in tables:
             # 如未创建，则创建
             cursor.execute('create table livelist3(uid varchar(10) primary key, state varchar(10), '
                            'draw varchar(10), username varchar(10), message_title varchar(10), room_id varchar(10))')
         if "wait_push2" not in tables:
             cursor.execute(
                 "create table 'wait_push2' (dynamicid int(10) primary key, uid varchar(10), "
@@ -2459,28 +2538,28 @@
         # ############获取动态############
         run = True  # 代码折叠
         if run:
             logger.info('---获取更新的动态')
 
             conn = sqlite3.connect(livedb)
             cursor = conn.cursor()
-            cursor.execute("SELECT * FROM subscriptionlist2")
+            cursor.execute("SELECT * FROM subscriptionlist3")
             subscriptions = cursor.fetchall()
             cursor.close()
             conn.commit()
             conn.close()
 
             if not subscriptions:
                 logger.info("无订阅")
             else:
                 subscriptionlist = []
                 for subscription in subscriptions:
                     uid = str(subscription[2])
                     groupcode = subscription[1]
-                    if "p" in groupcode:
+                    if groupcode.startswith("gp"):
                         if groupcode[2:] in friendlist:
                             if uid not in subscriptionlist:
                                 subscriptionlist.append(uid)
                     else:
                         if groupcode[1:] in grouplist:
                             if uid not in subscriptionlist:
                                 subscriptionlist.append(uid)
@@ -2534,59 +2613,63 @@
                             conn.commit()
                             conn.close()
 
         # ############获取直播状态############
         run = True  # 代码折叠
         if run:
             logger.info('---------获取更新的直播----------')
-            fortsize = 30
 
             if use_api is True:
                 fontfile = get_file_path("腾祥嘉丽中圆.ttf")
             else:
                 fontfile = get_file_path("NotoSansSC[wght].ttf")
+            fortsize = 30
             font = ImageFont.truetype(font=fontfile, size=fortsize)
             logger.info("获取订阅列表")
 
             conn = sqlite3.connect(livedb)
             cursor = conn.cursor()
-            cursor.execute("SELECT * FROM subscriptionlist2")
+            cursor.execute("SELECT * FROM subscriptionlist3")
             subscriptions = cursor.fetchall()
             cursor.close()
             conn.commit()
             conn.close()
 
             if not subscriptions:
                 logger.info("无订阅")
             else:
                 subscriptionlist = []
+                if beta_test:
+                    print(f"debug:pass list: {subscriptionlist}")
                 for subscription in subscriptions:
-                    uid = str(subscription[2])
-                    subscriptionlist.append(uid)
+                    liveid = int(subscription[3])
+                    if liveid == 0:
+                        # 未获取房间号，开始获取房间号
+                        pass
+                        if beta_test:
+                            print(f"debug:pass uid: {subscription[2]}")
+                    if liveid != 0:
+                        subscriptionlist.append(str(liveid))
                 if subscriptionlist:
-                    url = "https://api.live.bilibili.com/room/v1/Room/get_status_info_by_uids"
-                    post_json = {"uids": subscriptionlist}
-                    json_data = connect_api("json", url, post_json=post_json)
-                    if json_data["code"] != 0:
-                        logger.error("直播api出错请将此消息反馈给开发者，sub[0]=" + str(subscriptionlist[0]) +
-                                     ",msg=" + json_data["message"])
-                    else:
-                        livedatas = json_data["data"]
-                        livedata_list = list(livedatas)
+                    for liveid in subscriptionlist:
+                        url = f"https://api.live.bilibili.com/room/v1/Room/get_info?id={liveid}"
+                        json_data = connect_api("json", url)
+                        if json_data["code"] != 0:
+                            logger.error("直播api出错请将此消息反馈给开发者，sub[0]=" + str(subscriptionlist[0]) +
+                                         ",msg=" + json_data["message"])
+                        else:
+                            livedata = json_data["data"]
+                            uid = livedata["uid"]
+                            logger.info(f"bili_live_开始获取消息:{uid}")
 
-                        conn = sqlite3.connect(livedb)
-                        cursor = conn.cursor()
-                        for uid in livedata_list:
-                            logger.info("bili_live_开始获取消息:" + str(uid))
-                            livedata = livedatas[uid]
+                            conn = sqlite3.connect(livedb)
+                            cursor = conn.cursor()
                             live_status = str(livedata["live_status"])
-
-                            cursor.execute("SELECT * FROM livelist3 WHERE uid='" + str(uid) + "'")
+                            cursor.execute(f"SELECT * FROM livelist3 WHERE uid='{uid}'")
                             data_db = cursor.fetchone()
-
                             if data_db is None or live_status != str(data_db[1]):
                                 uname = livedata["uname"]
                                 face = livedata["face"]
                                 cover_from_user = livedata["cover_from_user"]
                                 keyframe = livedata["keyframe"]
                                 live_title = livedata["title"]
                                 room_id = livedata["room_id"]
@@ -2653,26 +2736,25 @@
 
                                 elif live_status == "0":
                                     message = uname + "已下播"
                                     cursor.execute(
                                         f'replace into livelist3 (uid, state, draw, username, message_title, room_id) '
                                         f'values'
                                         f'("{uid}","{live_status}","none","{uname}","{live_title}","{room_id}")')
-
-                        cursor.close()
-                        conn.commit()
-                        conn.close()
+                            cursor.close()
+                            conn.commit()
+                            conn.close()
 
         # ############推送直播状态############
         run = True  # 代码折叠
         if run:
             logger.info('---------推送直播----------')
             conn = sqlite3.connect(livedb)
             cursor = conn.cursor()
-            cursor.execute("SELECT * FROM subscriptionlist2")
+            cursor.execute("SELECT * FROM subscriptionlist3")
             subscriptions = cursor.fetchall()
             cursor.close()
             conn.commit()
             conn.close()
 
             if not subscriptions:
                 logger.info("无订阅")
@@ -2746,15 +2828,15 @@
                                     cursor.close()
                                     conn.commit()
                                     conn.close()
                         if send is False:
                             logger.info("该订阅由另一个bot进行推送，本bot将不发送消息")
 
                     # 检查是否是好友、是否入群
-                    if "p" in groupcode:
+                    if groupcode.startswith("gp"):
                         if groupcode[2:] not in friendlist:
                             send = False
                     else:
                         if groupcode[1:] not in grouplist:
                             send = False
 
                     # 检查是否不推送动态或直播
@@ -2926,15 +3008,15 @@
 
         # ############推送动态############
         run = True  # 代码折叠
         if run:
             logger.info('---------推送动态----------')
             conn = sqlite3.connect(livedb)
             cursor = conn.cursor()
-            cursor.execute("SELECT * FROM subscriptionlist2")
+            cursor.execute("SELECT * FROM subscriptionlist3")
             subscriptions = cursor.fetchall()
             cursor.close()
             conn.commit()
             conn.close()
 
             if not subscriptions:
                 logger.info("无订阅")
@@ -3006,15 +3088,15 @@
                                     cursor.execute(
                                         'replace into ' + groupcode + '(botid,permission) values("' + botid + '","5")')
                                     cursor.close()
                                     conn.commit()
                                     conn.close()
 
                     # 检查是否是好友、是否入群
-                    if "p" in groupcode:
+                    if groupcode.startswith("gp"):
                         if groupcode[2:] not in friendlist:
                             send = False
                     else:
                         if groupcode[1:] not in grouplist:
                             send = False
 
                     # 检查是否不推送动态或直播
@@ -3077,15 +3159,15 @@
                                         pushlist.append(new_dynamicid)
                         logger.info("未推送的动态" + str(pushlist))
 
                         # 分别发送图片，并保存为已推送
                         for dynamicid in pushlist:
                             conn = sqlite3.connect(livedb)
                             cursor = conn.cursor()
-                            cursor.execute("SELECT * FROM 'wait_push2' WHERE dynamicid = " + dynamicid)
+                            cursor.execute(f"SELECT * FROM 'wait_push2' WHERE dynamicid = {dynamicid}")
                             data = cursor.fetchone()
                             cursor.close()
                             conn.commit()
                             conn.close()
 
                             draw_path = data[2]
                             message_title = data[3]
```

### Comparing `nonebot_plugin_bili_push-1.1.4/setup.py` & `nonebot_plugin_bili_push-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='1.1.4',
+      version='1.1.9',
       description='nonebot plugin bili push',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

