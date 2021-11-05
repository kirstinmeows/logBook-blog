---
title: teamviewer - 好强大的一款远程协助工具
date: 2016-04-23
tags: [tool,teamviewer]
---

这是一个强大的远程协助软件，[teamviewer官网](http://www.teamviewer.com)这样介绍它：

> 通过Internet进行远程访问和远程支持的一体化解决方案，TeamViewer可在几秒钟内连接到世界各地的任何PC或服务器上。您可以身临现场般地远程控制您伙伴的PC。

发现它对于我这个[系统控](http://lupeng.me/tags/%E7%B3%BB%E7%BB%9F%E6%8E%A7/)真是最大的福音，因为我的设备基本上覆盖了所有系统，家里客厅一台Mac mini外加显示器（主力），卧室放着Windows10笔记本，公司宿舍里的Linux系统笔记本，办公室使用的是Windows7系统PC；移动设备也是iOS和Andriod并用。面对这么多系统，同步是个很大的问题，往往刚在Mac上写了一篇文章，然后上班了在公司PC上完成它，之后又想把手机里的一张照片附上去，最后再回到Mac上通过Hexo发布。所以同步和远程的需求非常强烈。并且把我养成了“只使用跨平台软件”的习惯，使用一款软件之前先确认其他平台是否都有。

通常情况下，大部分的任务都可以通过ssh连接终端来解决，但是有些时候还是需要一下桌面的，如果远程的是windows，那桌面就必不可少了。使用`teamviewer`时，只需要连接互联网，打开`teamviewer`软件，根据它所提供的`ID`以及密码就可以远程连接了，当然也可以将远程的电脑类似通讯录似的保存起来，方便下次的连接。

![](/image/tools/teamviewer01.png)

同时它也提供了会议功能以及桌面共享功能，当你正在远程其他桌面的时候，你会发现每一个windows窗口都有下图所示的小按钮，点击它可以设置与远程终端共享该窗口并进行演示。

![](/image/tools/teamviewer02.png)

同时也支持手机终端控制电脑桌面，下载对应App，还是通过`ID`连接到电脑，支持Android、iOS以及BlackBerry。可谓是基本上包含了所有的系统终端（貌似不支持windows phone），在不同的终端来回控制桌面。

闲之无聊，也许你会想和我一样尝试一下，当A控制B的时候，然后操作B再来远程A，会出现什么样的结果呢？会不会陷入一个循环的桌面呢？没错你猜对了，如下图所示。

![](/image/tools/teamviewer.png)

最后，对于个人用户，该软件是免费使用的，所以直接上官网下载就可以了。