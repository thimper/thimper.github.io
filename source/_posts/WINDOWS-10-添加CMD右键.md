---
title: WINDOWS 10 添加CMD右键
date: 2019-02-23 14:38:51
categories:
   - Windows
tags: 
   - Windows10
   - CMD
---
# 给windows 添加右键菜单CMD

有时候需要方便在windows 特定文件夹中唤起CMD命令行，很方便

- 准备注册脚本
```
Windows Registry Editor Version 5.00[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\background\shell\cmd_here] 
@="在此处打开命令行"
"Icon"="cmd.exe"[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\background\shell\cmd_here\command]
@="\"C:\\Windows\\System32\\cmd.exe\"" 
[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Folder\shell\cmdPrompt]
@="在此处打开命令行"[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Folder\shell\cmdPrompt\command]
 @="\"C:\\Windows\\System32\\cmd.exe\" \"cd %1\""[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\shell\cmd_here]
@="在此处打开命令行"
"Icon"="cmd.exe"[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\shell\cmd_here\command]
```
把上面脚本保存为.reg 文件

然后双击运行即可