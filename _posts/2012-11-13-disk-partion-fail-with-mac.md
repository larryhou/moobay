---
layout: post
title: "MAC分区失败解决方法"
date: 2012-11-13 21:27
comments: true
categories: 
---

我的MAC硬盘分了三个分区，我把其中两个删掉了，然后扩大主分区的可用空间，结果出错：  

## Mac分区失败 (未能修改分区图，因为文件系统验证失败）

Google了一下这种情况还蛮普遍的，解决方法也很简单：
	
>* 重启系统，按住<code>⌘+s</code>进入MAC命令行模式
>* 输入<code>fsck -f</code>回车
>* 输入<code>reboot</code>回车

经过以上三步后我的问题解决了，第一次围观命令行模式还是挺欣喜的。不过话说回来，Apple一向很重视用户体验，但现在居然出现这种问题实在有点费解：我差点就想格式化重装系统了...orz