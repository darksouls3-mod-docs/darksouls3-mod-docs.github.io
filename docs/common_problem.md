---
title: 常见问题
nav_order: 4
---

<details open markdown="block">
  <summary>
    目录
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

# Steam is not launched.

{: .note-title }
> 中文意思是
> 
> steam未启动

> 常见于学习版steam无缝联机玩家

![steam未启动.png](/assets/images/steam未启动.png)

1. 如果steam没有启动，那就启动steam，再启动游戏
1. 如果已经启动steam了，那就右键管理员启动游戏

---

# Unsupported SteamUser version! SteamUser023
> 常见于学习版steam无缝联机

![不支持的steam用户版本.png](/assets/images/不支持的steam用户版本.png)

出现这个情况是因为你游戏目录里的`OnlineFix64.dll`这个文件不是联机补丁里面的，正确的联机补丁这个文件的大小应该是`11,582 KB`

解决方案就是找到联机补丁里的这个文件重新覆盖进去

参考：[安装无缝联机，如果你是学习版需要额外打一个联机补丁]({{site.baseurl}}/docs/upgrade/esrc/#如果你是学习版需要额外打一个联机补丁)

---

# Failed to find "SeamlessCoop//ds3sc.dll" (Error = 2)

![ds3sc_dll文件丢失.png](/assets/images/ds3sc_dll文件丢失.png)

如图所示，你这个文件丢了，这个是无缝联机mod的其中一个文件，找一下放进去就行了

参考：[安装无缝联机]({{site.baseurl}}/docs/upgrade/esrc/)

---

# Please enter a session password in your settings file.

{: .note-title }
> 中文意思是
> 
> 请在配置文件中设置一个房间密码（会话密码）

这个是无缝联机mod的提示，提示你需要设置一个房间密码才能启动游戏，在无缝的配置文件`ds3sc_settings.ini`里设置一下房间密码就行了

![无缝没设置密码.png](/assets/images/无缝没设置密码.png)

设置密码步骤参考：[安装无缝联机]({{site.baseurl}}/docs/upgrade/esrc/)

---

# This version of seamless co-op (1.x.x) is depreciated and requires an update.

{: .note-title }
> 中文意思是
> 
> 当前版本的无缝联机mod已经被弃用，需要更新到最新版

![无缝不是最新版.png](/assets/images/无缝不是最新版.png)

如图所示 图片中出现的1.7.2就是代表当前版本，需要下载最新版覆盖进去就行了

下载最新版无缝参考：[安装无缝联机]({{site.baseurl}}/docs/upgrade/esrc/)

---

# The mod may not be compatible with the installed game version

{: .note-title }
> 大概意思是
> 
> 当前版本的无缝联机mod不兼容当前版本的游戏

![无缝不兼容当前游戏版本.png](/assets/images/无缝不兼容当前游戏版本.png)

一般情况下是你的无缝联机mod版本不兼容你的游戏版本，要么换无缝，要么换游戏版本，让这两个兼容就行了，最简单的就是用最新版的无缝和最新版的游戏就好了

如果你确定你的无缝和游戏是兼容的版本，可以尝试重启一下电脑

重启电脑还不行的话，就验证一下游戏完整性

---

# Failed to load dll from the list. 或者 WaitForSingleObject failed! Return value = 258, Error = 0

{: .note-title }
> 中文意思是
> 
> 从列表中加载dll文件失败

> 常见于学习版steam无缝联机

![dll文件未找到.png](/assets/images/dll文件未找到.png)

找到游戏目录中的`dlllist.txt`文件,并打开

![dlllist文件.png](/assets/images/dlllist文件.png)

![dlllist文件内容.png](/assets/images/dlllist文件内容.png)

确保文件中涉及到的dll文件都存在，最常见的就是`OnlineFix64.dll`文件被杀毒软件删了，
需要加一下白名单，把这个文件重新拖进来，不知道如何操作可以参考这个空降链接：
[法魂mod兼容无缝教程(含正版学习版)-授人以渔 【精准空降到 45:17】](https://www.bilibili.com/video/BV1cLieYtE5d/?t=2717){:target="_blank"}

我这里只有一个dll，所以只需要确认这一个dll文件是否存在，如果你有多个，需要依次确认是否存在

还有一点就是**不要有空行**，空行也会被认为是一个dll文件，导致报错

![dlllist文件空行示范.png](/assets/images/dlllist文件空行示范.png)
❌错误示范

如果你没有空行，涉及的dll文件也都存在，那就把涉及到的dll文件再重新覆盖一遍

---

# 我的游戏语言怎么是英文？怎么改成简体中文

> 学习版玩家会遇到这个问题

找到游戏目录的`OnlineFix.ini`，用记事本打开，找到`Language`那一行，把井号去掉，把`english`改成`schinese`，**保存然后重启游戏**

![游戏本体修改为简体中文.png](/assets/images/游戏本体修改为简体中文.png)

# 我的无缝mod道具为什么是英文？怎么改成简体中文

找到无缝的配置文件`ds3sc_settings.ini`，记事本打开，然后修改`mod_language_override`为`schinese`，前提是你打了简体中文补丁，**保存然后重启游戏**

![无缝修改为简体中文.png](/assets/images/无缝修改为简体中文.png)

# 打上无缝联机mod之后手柄没有反应？

> 常见于学习版steam无缝联机

找到steam库中的`spacewar`，右键-属性-控制器-禁用steam输入，如果还不行，就在`控制器配置器`里选一个steam映射
![禁用steam输入.png](/assets/images/禁用steam输入.png)

---

# 未找到可加入的世界

![未找到房间.png](/assets/images/未找到房间.png)

你和你的小伙伴想联机到一起，需要满足下列条件：
1. 无缝联机密码一样(注意等于号有没有空格，修改完配置文件有没有保存)
2. 标题页面左上角三个版本号一样
3. 都是学习版或者都是正版(正版想和学习版联机需要转成学习版，操作步骤参考：[正版变学习版]({{site.baseurl}}/docs/upgrade/esrc/#如果你是学习版需要额外打一个联机补丁)
4. 打了哪些mod也需要一样(不影响游戏数值的除外)

---

# dlc无缝联机不了？

[黑暗之魂3无缝联机进入dlc方法（ce）](https://www.bilibili.com/opus/1057903745582497831?spm_id_from=333.1387.0.0){:target="_blank"}

---

# 选完角色闪退？继续游戏闪退？进入游戏后角色原地打转？

检查游戏路径是否有中文

参考：[安装mod之前需要确认的事项]({{site.baseurl}}/docs/install_before/)

---