# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.4.1.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.4.1.tar", last modified: Mon May  1 17:57:50 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.5.0.tar", last modified: Tue May  2 17:18:13 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1.tar` & `nonebot-plugin-chatgpt-on-qq-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:57:50.160346 nonebot-plugin-chatgpt-on-qq-1.4.1/
--rw-rw-rw-   0        0        0      770 2023-05-01 17:57:50.158889 nonebot-plugin-chatgpt-on-qq-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 17:57:50.145058 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    16525 2023-05-01 17:57:39.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     1194 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py
--rw-rw-rw-   0        0        0    10536 2023-05-01 17:57:39.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/sessions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:57:50.156419 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-01 17:57:50.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-05-01 17:57:50.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:57:50.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-01 17:57:50.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-01 17:57:50.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 17:57:50.160874 nonebot-plugin-chatgpt-on-qq-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-05-01 17:56:05.000000 nonebot-plugin-chatgpt-on-qq-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.434898 nonebot-plugin-chatgpt-on-qq-1.5.0/
+-rw-rw-rw-   0        0        0      770 2023-05-02 17:18:13.433916 nonebot-plugin-chatgpt-on-qq-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.419764 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    21908 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    11359 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.431780 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:18:13.434898 nonebot-plugin-chatgpt-on-qq-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-05-02 17:17:55.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.4.1
+Version: 1.5.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 from datetime import datetime
 from json import JSONDecodeError
 from typing import Dict, List, Any
 
 from nonebot.adapters.onebot.v11 import (Bot, MessageEvent,
                                          GroupMessageEvent, PrivateMessageEvent,
                                          GROUP_ADMIN, GROUP_OWNER, MessageSegment, Message)
@@ -14,38 +15,48 @@
 
 from .config import Config, plugin_config
 from .loadpresets import presets_str
 from .custom_errors import NeedCreatSession
 from .sessions import session_container, Session, get_group_id
 
 __usage__: str = (
-        "太长不看版:\n"
-        + "先用/chat new命令,选择模板来创建会话,随后/talk 内容 来会话\n\n"
-        + "/chat :获取菜单\n"
-        + "/chat new :利用模板创建一个会话并加入\n"
-        + "/talk <内容> :在当前的会话进行聊天\n"
-        + "/chat list :获得当前已创建的会话列表\n"
-        + "/chat list <@user> :查看@的用户创建的会话\n"
-        + "/chat join 序号(指/chat list中的序号) :参与list中的某个会话\n"
-        + "/chat new (prompt) :自定义prompt来创建一个新的会话\n"
-        + "/chat del :删除当前所在会话\n"
-        + "/chat del 序号(指/chat list中的序号) :删除list中的某个会话\n"
-        + "/chat dump :导出当前会话json字符串格式的上下文信息\n"
-        + "/chat cp <chat id> :复制会话并新建\n"
-        + "/chat who :查看当前会话\n"
+    "指令表：\n"
+    "    /chat help 获取指令帮助菜单\n"
+    "    /talk <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
+    ">> 增\n"
+    "    /chat new  根据预制模板prompt创建并加入一个新的会话\n"
+    "    /chat new <自定义prompt> 根据自定义prompt创建并加入一个新的会话\n"
+    "    /chat json 根据历史会话json来创建一个会话，输入该命令后会提示你在下一个消息中输入json\n"
+    "    /chat cp 根据当前会话创建并加入一个新的会话\n"
+    "    /chat cp <id> 根据会话<id>为模板进行复制新建加入（id为/chat list中的序号）\n"
+    ">> 删\n"
+    "    /chat del 删除当前所在会话\n"
+    "    /chat del <id> 删除序号为<id>的会话（id为/chat list中的序号）\n"
+    "    /chat clear 清空本群全部会话\n"
+    "    /chat clear <@user> 删除@用户创建的会话\n"
+    ">> 改\n"
+    "    /chat join <id> 加入会话（id为/chat list中的序号）\n"
+    "    /chat rename <name> 重命名当前会话\n"
+    ">> 查\n"
+    "    /chat who 查看当前会话信息\n"
+    "    /chat list 获取当前群所有存在的会话的序号及创建时间\n"
+    "    /chat list <@user> 获取当前群查看@的用户创建的会话\n"
+    "    /chat prompt 查看当前会话的prompt\n"
+    "    /chat dump 导出当前会话json字符串格式的上下文信息，可以用于/chat json导入\n"
+
 )
 __plugin_meta__ = PluginMetadata(
     name="多功能ChatGPT插件",
     description="基于chatGPT-3.5-turbo API的nonebot插件",
     usage=__usage__,
     config=Config,
     extra={
         "License": "BSD License",
         "Author": "颜曦",
-        "version": "1.4.1",
+        "version": "1.5.0",
     },
 )
 
 allow_private: bool = plugin_config.allow_private
 api_keys: List[str] = session_container.api_keys
 temperature: float = plugin_config.temperature
 model: str = plugin_config.model_name
@@ -64,43 +75,139 @@
 
 async def _allow_private_checker(event: MessageEvent) -> bool:
     return isinstance(event, GroupMessageEvent) or allow_private
 
 
 ALLOW_PRIVATE = Permission(_allow_private_checker)
 
-Chat = on_regex(rf"^{prefix_str}{talk_cmd_str}\s+(?P<content>.+)", permission=ALLOW_PRIVATE)  # 聊天
-CallMenu = on_regex(rf"^{pattern_str}$", permission=ALLOW_PRIVATE)  # 呼出菜单
+Chat = on_regex(rf"^{prefix_str}{talk_cmd_str}\s+(?P<content>.+)", flags=re.S, permission=ALLOW_PRIVATE)  # 聊天
+CallMenu = on_regex(rf"^{pattern_str}\s+help$", permission=ALLOW_PRIVATE)  # 呼出菜单
 ShowList = on_regex(rf"^{pattern_str}\s+list\s*$", permission=ALLOW_PRIVATE)  # 展示群聊天列表
 Join = on_regex(rf"^{pattern_str}\s+join\s+(?P<id>\d+)", permission=ALLOW_PRIVATE)  # 加入会话
 Delete = on_regex(rf"^{pattern_str}\s+del\s+(?P<id>\d+)", permission=ALLOW_PRIVATE)  # 删除会话
 DelSelf = on_regex(rf"^{pattern_str}\s+del\s*$", permission=ALLOW_PRIVATE)  # 删除当前会话
 Dump = on_regex(rf"^{pattern_str}\s+dump$", permission=ALLOW_PRIVATE)  # 导出json
-CreateConversationWithPrompt = on_regex(rf"^{pattern_str}\s+new\s+(?P<prompt>.+)$",
+CreateConversationWithPrompt = on_regex(rf"^{pattern_str}\s+new\s+(?P<prompt>.+)$", flags=re.S,
                                         permission=ALLOW_PRIVATE)  # 利用自定义prompt创建会话
 CreateConversationWithTemplate = on_regex(rf"^{pattern_str}\s+new$", permission=ALLOW_PRIVATE)  # 利用模板创建会话
 CreateConversationWithJson = on_regex(rf"^{pattern_str}\s+json$", permission=ALLOW_PRIVATE)  # 利用json创建会话
 ChatCopy = on_regex(rf"^{pattern_str}\s+cp\s+(?P<id>\d+)$", permission=ALLOW_PRIVATE)
+ChatCP = on_regex(rf"^{pattern_str}\s+cp$", permission=ALLOW_PRIVATE)
 ChatWho = on_regex(rf'^{pattern_str}\s+who$', permission=ALLOW_PRIVATE)
 ChatUserList = on_regex(rf"^{pattern_str}\s+list\s*\S+$", permission=ALLOW_PRIVATE)  # 展示群聊天列表
+ReName = on_regex(rf"^{pattern_str}\s+rename\s+(?P<name>.+)$", permission=ALLOW_PRIVATE)  # 重命名当前会话
+ChatPrompt = on_regex(rf"^{pattern_str}\s+prompt$", permission=ALLOW_PRIVATE)
+ChatClear = on_regex(rf"{pattern_str}\s+clear$", permission=ALLOW_PRIVATE)
+ChatClearAt = on_regex(rf"{pattern_str}\s+clear\s*\S+$", permission=ALLOW_PRIVATE)
+
+
+@ChatClear.handle()
+async def _(bot: Bot, event: MessageEvent):
+    userId: int = int(event.get_user_id())
+    groupId: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    if isinstance(event, PrivateMessageEvent):  # 私聊
+        session: Session = group_usage.pop(userId)
+        if not session:
+            await ChatClear.finish("当前不存在会话")
+        session_container.sessions.remove(session)
+        session.delete_file()
+        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
+        await ChatClear.finish("已删除当前会话")
+
+    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+    if not perm_check:
+        await ChatClear.finish("只有群主或管理员才能清空本群全部会话!")
+    session_list: List[Session] = session_container.get_group_sessions(groupId)
+    num = len(session_list)
+    for session in session_list:
+        await session_container.delete_session(session, groupId)
+    await ChatClear.finish(f"成功删除本群全部共{num}条会话")
+
+
+@ChatClearAt.handle()
+async def _(bot: Bot, event: MessageEvent, message: Message = EventMessage()):
+    if isinstance(event, PrivateMessageEvent):
+        await ChatClearAt.finish()
+    segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
+    if not segments:
+        await ChatClearAt.finish()
+    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+    senderId: int = int(event.get_user_id())
+    userId: int = int(segments[0].data.get("qq", ""))
+    groupId: str = get_group_id(event)
+    if userId != senderId and not perm_check:
+        await ChatClearAt.finish("您不是该会话的创建者或管理员!")
+    session_list: List[Session] = [s for s in session_container.sessions if s.group == groupId and s.creator == userId]
+    num = len(session_list)
+    if num == 0:
+        await ChatClearAt.finish(f"本群用户 {userId} 还没有创建过会话哦")
+    for session in session_list:
+        await session_container.delete_session(session, groupId)
+    await ChatClearAt.finish(f"成功删除本群用户 {userId} 创建的全部会话共{num}条")
+
+
+@ChatCP.handle()
+async def _(event: MessageEvent):
+    if isinstance(event, PrivateMessageEvent):
+        await ChatCP.finish('私聊中无法复制会话，如果想导出json字符串请使用 /chat dump')
+    userId: int = int(event.get_user_id())
+    groupId: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    if userId not in group_usage:
+        await ChatCP.finish('请先加入一个会话，再进行复制当前会话 或者使用 /chat cp <id> 进行复制')
+    session: Session = group_usage[userId]
+    group_usage[userId].del_user(userId)
+    new_session: Session = session_container.create_with_session(session, userId, groupId)
+    await ChatCP.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
+
+
+@ChatPrompt.handle()
+async def _(event: MessageEvent):
+    userId: int = int(event.get_user_id())
+    groupId: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    if userId not in group_usage:
+        await ChatPrompt.finish('请先加入一个会话，再进行重命名')
+    session: Session = group_usage[userId]
+    await ChatPrompt.finish(f'会话：{session.name}\nprompt：{session.prompt}')
+
+
+@ReName.handle()
+async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
+    if isinstance(event, PrivateMessageEvent):
+        await ReName.finish('私聊中只存在一个会话，无法命名，如果想导出json字符串请使用 /chat dump')
+    userId: int = int(event.get_user_id())
+    groupId: str = get_group_id(event)
+    group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
+    if userId not in group_usage:
+        await ReName.finish('请先加入一个会话，再进行重命名')
+    perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+    session: Session = group_usage[userId]
+    name: str = info.get('name', '').strip()
+    if session.creator == userId or perm_check:
+        session.rename(name[:32])
+        await ReName.finish(f'当前会话已命名为 {session.name}')
+    logger.info(f'重命名群 {groupId} 会话 {session.name} 失败：权限不足')
+    await ReName.finish("您不是该会话的创建者或管理员!")
 
 
 @ChatUserList.handle()
 async def _(event: MessageEvent, message: Message = EventMessage()):
     if isinstance(event, PrivateMessageEvent):
         await ChatUserList.finish('私聊只有一个会话，如果想导出json字符串请使用 /chat dump')
     segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
     if not segments:
         await ChatUserList.finish()
     userId: int = int(segments[0].data.get("qq", ""))
     groupId: str = get_group_id(event)
     session_list: List[Session] = [s for s in session_container.sessions if s.group == groupId and s.creator == userId]
     msg: str = f"在群中创建会话{len(session_list)}条：\n"
     for index, session in enumerate(session_list):
-        msg += f" 名称:{session.name} " \
+        msg += f" 名称:{session.name[:10]} " \
                f"创建者:{session.creator} " \
                f"时间:{datetime.fromtimestamp(session.creation_time)}\n"
     await ChatUserList.finish(MessageSegment.at(userId) + msg)
 
 
 @ChatWho.handle()
 async def _(event: MessageEvent):
@@ -109,15 +216,15 @@
     userId: int = int(event.get_user_id())
     groupId: str = get_group_id(event)
     group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
     if userId not in group_usage:
         await ChatWho.finish('当前没有加入任何会话，请加入或创建一个会话')
     session: Session = group_usage[userId]
     msg = f'当前所在会话信息:\n' \
-          f"名称:{session.name}\n" \
+          f"名称:{session.name[:10]}\n" \
           f"创建者:{session.creator}\n" \
           f"时间:{datetime.fromtimestamp(session.creation_time)}\n" \
           f"可以使用 /chat dump 导出json字符串格式的上下文信息"
     await ChatWho.finish(msg)
 
 
 @ChatCopy.handle()
@@ -126,22 +233,22 @@
         await ChatCopy.finish('私聊中无法复制会话，如果想导出json字符串请使用 /chat dump')
     session_id = int(info.get('id', '').strip())
     userId: int = int(event.get_user_id())
     groupId: str = get_group_id(event)
     group_sessions: List[Session] = session_container.get_group_sessions(groupId)
     group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
     if not group_sessions:
-        await Join.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
+        await ChatCopy.finish("本群尚未创建过会话!请用/chat new命令来创建会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
-        await Join.finish("序号超出!", at_sender=True)
+        await ChatCopy.finish("序号超出!", at_sender=True)
     session: Session = group_sessions[session_id - 1]
     if userId in group_usage:
         group_usage[userId].del_user(userId)
     new_session: Session = session_container.create_with_session(session, userId, groupId)
-    await Join.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
+    await ChatCopy.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
 
 
 @Dump.handle()
 async def _(event: MessageEvent):
     userId: int = int(event.get_user_id())
     groupId: str = get_group_id(event)
     try:
@@ -202,31 +309,26 @@
 @DelSelf.handle()
 async def _(bot: Bot, event: MessageEvent):
     userId: int = int(event.get_user_id())
     groupId: str = get_group_id(event)
     group_usage: Dict[int, Session] = session_container.get_group_usage(groupId)
     session: Session = group_usage.pop(userId)
     if not session:
-        await Delete.finish("当前不存在会话")
+        await DelSelf.finish("当前不存在会话")
     if isinstance(event, PrivateMessageEvent):  # 私聊
         session_container.sessions.remove(session)
         session.delete_file()
         logger.success(f'成功删除群 {groupId} 会话 {session.name}')
-        await Delete.finish("已删除当前会话")
+        await DelSelf.finish("已删除当前会话")
     perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
     if session.creator == userId or perm_check:
-        users = set(uid for uid, s in group_usage.items() if s is session)
-        for user in users:
-            group_usage.pop(user)
-        session_container.sessions.remove(session)
-        session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
-        await Delete.finish("删除成功!")
+        await session_container.delete_session(session, groupId)
+        await DelSelf.finish("删除成功!")
     logger.info(f'删除群 {groupId} 会话 {session.name} 失败：权限不足')
-    await Delete.finish("您不是该会话的创建者或管理员!")
+    await DelSelf.finish("您不是该会话的创建者或管理员!")
 
 
 @Delete.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
     userId: int = int(event.get_user_id())
     groupId: str = get_group_id(event)
@@ -238,26 +340,21 @@
         session_container.sessions.remove(session)
         session.delete_file()
         logger.success(f'成功删除群 {groupId} 会话 {session.name}')
         await Delete.finish("已删除当前会话")
     # 群聊
     group_sessions: List[Session] = session_container.get_group_sessions(groupId)
     if not group_sessions:
-        await Join.finish("本群尚未创建过会话!", at_sender=True)
+        await Delete.finish("本群尚未创建过会话!", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
-        await Join.finish("序号超出!", at_sender=True)
+        await Delete.finish("序号超出!", at_sender=True)
     perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
     session: Session = group_sessions[session_id - 1]
     if session.creator == userId or perm_check:
-        users = set(uid for uid, s in group_usage.items() if s is session)
-        for user in users:
-            group_usage.pop(user)
-        session_container.sessions.remove(session)
-        session.delete_file()
-        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
+        await session_container.delete_session(session, groupId)
         await Delete.finish("删除成功!")
     else:
         logger.info(f'删除群 {groupId} 会话 {session.name} 失败：权限不足')
         await Delete.finish("您不是该会话的创建者或管理员!")
 
 
 # 暂时已完成
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/config.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     model_name: str = 'gpt-3.5-turbo'
     allow_private: bool = True
     change_chat_to: str = None
     max_tokens: int = 1024
     auto_create_preset_info: bool = True
     customize_prefix: str = '/'
     customize_talk_cmd: str = 'talk'
+    timeout: int = 10
 
     @validator('api_key')
     def api_key_validator(cls, v) -> List[str]:
         if not v:
             raise NoApiKeyError('请输入APIKEY')
         if isinstance(v, list):
             return v
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq/sessions.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,23 @@
         self.dir_path: Path = dir_path
         self.sessions: List[Session] = []
         self.session_usage: Dict[group_id, Dict[user_id, Session]] = {}
         if not dir_path.exists():
             dir_path.mkdir(parents=True)
         self.load()
 
+    async def delete_session(self, session: "Session", groupId: str) -> None:
+        group_usage: Dict[int, Session] = self.get_group_usage(groupId)
+        users = set(uid for uid, s in group_usage.items() if s is session)
+        for user in users:
+            group_usage.pop(user)
+        self.sessions.remove(session)
+        session.delete_file()
+        logger.success(f'成功删除群 {groupId} 会话 {session.name}')
+
     def get_group_sessions(self, group_id: Union[str, int]) -> List["Session"]:
         return [s for s in self.sessions if s.group == str(group_id)]
 
     def load(self) -> None:
         for file in self.dir_path.glob('*.json'):
             session = Session.reload_from_file(file)
             if not session:
@@ -121,14 +130,23 @@
             self.basic_len: int = basic_len
         else:
             self.basic_len = len(self.history)
         if is_save:
             self.save()
 
     @property
+    def prompt(self) -> str:
+        return self.history[0].get('content', '').strip()
+
+    def rename(self, name: str) -> None:
+        self.file_path.unlink(missing_ok=True)
+        self.name = name
+        self.save()
+
+    @property
     def users(self) -> Set[int]:
         return self._users
 
     def add_user(self, user: int) -> None:
         self._users.add(user)
         self.save()
 
@@ -171,14 +189,15 @@
             openai.api_key = key
             try:
                 completion: dict = await openai.ChatCompletion.acreate(
                     model=model,
                     messages=self.chat_memory,
                     temperature=temperature,
                     max_tokens=max_tokens,
+                    timeout=timeout,
                 )
                 self.update_from_completion(completion)
                 if completion.get("choices") is None:
                     raise NoResponseError("未返回任何choices")
                 if len(completion["choices"]) == 0:
                     raise NoResponseError("返回的choices长度为0")
                 if completion["choices"][0].get("message") is None:
@@ -246,14 +265,15 @@
 
     def dump2json_str(self) -> str:
         return json.dumps(self.chat_memory, ensure_ascii=False)
 
 
 chat_memory_max = plugin_config.chat_memory_max if plugin_config.chat_memory_max > 2 else 2
 history_max = plugin_config.history_max if plugin_config.history_max > chat_memory_max else 100
+timeout = int(plugin_config.timeout) if plugin_config.timeout and plugin_config.timeout > 0 else 10
 
 session_container: SessionContainer = SessionContainer(
     dir_path=plugin_config.history_save_path,
     chat_memory_max=chat_memory_max,
     api_keys=plugin_config.api_key,
     history_max=history_max,
 )
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.4.1
+Version: 1.5.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.4.1/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.4.1',
+    version='1.5.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

