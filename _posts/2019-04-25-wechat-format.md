---
title: 为了用 Markdown 写微信公众号，自定义了一个编辑器
date: 2019-04-28
tags: [编程,开源项目,公众号,编辑器]
---

身边应该有不少朋友在写公众号，不知道你们用的是什么编辑器呢？

- [135编辑器](http://www.135editor.com/)
- [i排版](http://ipaiban.com/bianji)
- [秀米 XIUMI](https://xiumi.us/#/)
- [易点编辑器](http://www.wxeditor.com/)

上面这些编辑器，应该是小编们用得最多的几款，它可以快速添加各种样式插件，使文章更吸引眼球，让用户看起来很爽，欲罢不能。毕竟他们最注重的是阅读量，而非内容。

我也有写文章的习惯，但我不是小编，格式上只追求简约大方即可，重点在文字上，希望内容能产生一些价值。自从用了 `Markdown` 标记语言后，写文章就再也没用过其他的编辑器。

### 什么是 Markdown？
什么是 Markdown？它是目前最流行的写作标记语言，没有之一。它能够通过简单标记就能实现文档格式，让写作者**专注于内容**。

由于它是纯文本，所以它可以像代码一样进行版本管理，同时，它对 Web 也非常友好，方便转成 HTML，甚至直接将 Markdown 文档生成静态站点，很多免费的自建博客服务都是采用的这种方案。目前几乎所有主流的写作平台，其编辑器都支持 Markdown。

一些 Markdown 编辑器，甚至在其基础上，扩展了很多功能。例如：公式及表格的支持。前段时间，一个外国小哥的数学笔记火了，全程像敲代码一般，紧追数学老师板书，记了 1700 + 页笔记。感兴趣可以看下这篇文章：

[1700页数学笔记火了！全程敲代码，速度飞快易搜索，硬核小哥教你上手LaTeX+Vim](https://mp.weixin.qq.com/s/QpJWyLY5AyrXGF-j7LYTGg)

### 为什么不支持 Markdown？
虽然支持它的编辑器多到数不过来，可是国内最著名的内容发布平台 —— 微信公众号，它的编辑器就不支持 Markdown，可算折腾坏了一帮写作者。为什么不支持？可能有两个原因吧。

> 用户学习成本

Markdown 语法虽然简单，但对大部分人来说，毕竟也是一门新的知识，这就增加了用户的学习使用成本。你要知道，绝大部分的人，哪怕一点点的新东西都是接受不了的，微信没把编辑器做成 Word 的样式，我觉得已经是克制了的。

> 支持的样式并不完整

Markdown 只提供了简单的样式标签，例如：标题，引用，链接等等，而对于复杂的样式，例如文字背景色等等，它是不支持的。

而微信面对的是全体创作者，单纯使用 Markdown 编辑器定然不能满足基本需求，而兼容 Markdown 的需求优先级并不高。

所以，一直以来，微信并不支持 Markdown，但我猜测，支持 Markdown 的功能迟早还是会做的。

### Markdown 写公众号的痛
你不是说了 Markdown 对 Web 非常友好嘛，转成富文本样式，然后贴到微信公众号的编辑器里，就可以了呀。道理是没错，但这正是折腾人的关键所在，因为 Markdown 只定义了基础的标签，而没有样式。

于是，各家的 Markdown 编辑器导出的样式都是有差异的，并且，跟微信公众号上的默认样式也不兼容。所以，贴进去后，显示出来的样式各不相同，如果文章里再有一些非标准的 Markdown 语法，显示出来更是五花八门了。一直以来都很纠结，对于一些样式复杂的文章，几乎就不发公众号了，因为调整样式，就要耗费大量的精力。

除了样式兼容性问题，还有微信公众号对外部链接限制问题，公众号内文章只允许引用微信内部链接，不支持外部链接。文章里若添加了第三方链接，我们只能硬生生的将 链接重新再贴进去。或者通过「阅读原文」链接原文地址。

### 解决方案
微信公众号编辑器都几乎成为一种新的行业了，文章开头的那些编辑器，都能自力更生了，说明对小编们来说，公众号编辑器问题真的是一个痛点。

而对于适配公众号样式的 Markdown 编辑器，几乎没有，之前接触过 [Md2All](http://md.aclickall.com/)，功能上很完整，但是它并非只针对微信公众号，所以在细节方面的处理，总是差强人意。

一直想着，应该写一款符合自己样式风格的公众号编辑器。然而，一个偶然机会，发现了它，[花三小时写这个工具，只为一分钟拯救公众号排版](https://mp.weixin.qq.com/s/pn0LzyfgUj6rGUfVHUksjg)。

在程序世界里，有句老话说「不要重复造轮子」，你费好大劲去研究怎么做，没准别人已经都出成品了，这样就造成了资源浪费。幸运的是，我的「轮子」还没有开始动手呢。

### 总要做点自己的贡献
这款公众号编辑器基本符合我的心里预期，简单的界面，优雅的样式风格，你看到的这篇文章的样式，就是通过它生成的。

它还有一些特殊的增强项，比如将外部链接自动生成脚注，放在文章底部；支持日语注音假名和汉语拼音，例如：小夜時雨【さ・よ・しぐれ】  上海【Shàng・hǎi】

虽然默认的样式已经基本满足我了，但还是缺少一些自定义的功能，比如字体大小的设置，以及主题切换等功能，作者并没有实现。但是，作者已经将源代码开源了，而我们不能只知道一味索取，而不懂得付出。

于是，我便动手实现了这部分的功能。好在代码并不复杂，简单研究一下，周末花了点时间，就把这部分的功能填补上了。

### 最后
这个过程还是很有趣，不仅解决了自己的痛点，还学到了知识，同时还做出了一点点自己的贡献。

如果你也喜欢这篇文章的样式，这个微信公众号编辑器分享给你。[微信公众号格式化编辑器 - 作者原版本](https://lab.lyric.im/wxformat/)
 
根据源代码，我重写了一个后台服务版本，计划提供一些在线 API 的功能。仓库地址：[wechat-format-server: 基于 wechat-format 的服务端版本](https://github.com/pengloo53/wechat-format-server)

完