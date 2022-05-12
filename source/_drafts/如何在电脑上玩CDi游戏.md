---
title: {{ title }}
date: 2022-05-12 08:23:34
tags:
---

**提示：本文假设您已经可以正常访问特殊网络；本文假设您有过使用模拟器的经验**

# 序言

相信很多人都听说过飞利浦CD-i的大名了吧，它上面屎作多多，神作也不是没有，但现在很难在实机上游玩了。幸亏CD-i的大部分游戏已经被模拟出来了
，我就总结一下经验，让一些想要玩到这些游戏的读者们体验到~~屎~~CD-i的~~力量~~！

# 一、准备工作

想要模拟CD-i，你将需要：一台运行正常的**电脑（手机不行！！）**、游戏ROM文件、CD-i的BIOS以及模拟器。

游戏ROM可以到[互联网档案馆（.bin格式，用CD-i Emulator打开）](https://archive.org/download/redump.cdi.revival)以及[edge|emulation（.chd格式，用SAME CD-i打开）](https://edgeemu.net/browse-cdi.htm)去下载。你也可以自己dump一份或者使用其他来源的ROM。

# 二、使用[CD-i Emulator](https://cdiemu.org)进行模拟

### 作者提醒：这个模拟器使用**鼠标**进行操作！你没听错，是**鼠标**！这把CDi的操作屎度直接放大了114.5141919810倍！如果受不了的话请直接跳转到下一章。

## 介绍

CD-i Emulator，一个闭源付费软件模拟器。 最新的公开版本 0.5.3 beta 4 可以追溯到 2018 年，不幸的是，由于 beta 版本中处理免费试用时间的方式，现在无法播放。 测试版确实具有*数字视频盒*（不知道这是啥）的概念验证仿真，但兼容性可能仍然是一个问题。 尽管发布之间的时间很长，但截至 2021 年 7 月，该模拟器似乎仍在积极开发中，正在开发下一个版本（可能称为 0.6），据报道该版本支持大多数 DVC 游戏，并且还有其他一些改进。（摘录自[Emulation General Wiki](https://emulation.gametechwiki.com/index.php/Philips_CD-i_emulators)）

## 方法

首先，[下载（破解过的）模拟器](http://tgames.fr/tgames/cdiemu-0.5.3-beta4-PatchedV1.2.zip),然后，把它解压到电脑的任意地方。打开“wcdiemu-v053b4.exe”，它应该会显示一个窗口：
![Rp5bfh.png](https://www.helloimg.com/images/2022/05/12/Rp5bfh.png)
这时我们不用担心，下载[BIOS文件](https://drive.google.com/file/d/1S9Xqhb7sCXC3SZhxMUHjMuPSbHXRnJyD/view?usp=sharing)，解压到模拟器文件夹里的rom文件夹即可。再次打开之后应该不会显示提示了。如图[![RpBCGA.png](https://www.helloimg.com/images/2022/05/12/RpBCGA.png)](https://www.helloimg.com/image/RpBCGA)
之后，点击File，再点击Open...，选择你下载的ROM文件。最后，点击窗口左上角的[![Rp5uan.png](https://www.helloimg.com/images/2022/05/12/Rp5uan.png)](https://www.helloimg.com/image/Rp5uan)即可。不出意外的话，会显示这个画面： [![RpB3ar.png](https://www.helloimg.com/images/2022/05/12/RpB3ar.png)](https://www.helloimg.com/image/RpB3ar)用鼠标点击Play CD-i，就可以畅快开玩了！

## 总结

用这种方法玩CD-i游戏，配置较为简单，但是用鼠标操作是一个硬伤，另外还有音画不同步等种种问题，个人不推荐使用，但如果有特殊需求的话可以使用。

# 三、使用RetroArch中的[SAME CDi](https://docs.libretro.com/library/same_cdi/)进行模拟

## 介绍

SAME CDi 是一个用于 libretro 的 S(ingle) A(rcade) M(achine) E(mulator)，从 MAME libretro 分叉出来，而 MAME libretro 又是 MAME 的一个分支。 它仅包括飞利浦 CD-i 驱动程序，并简化了 CD 内容的加载以提供“即插即用”体验。（摘录自[Libretro Docs](https://docs.libretro.com/library/same_cdi/)）

## 方法

这个难一点。首先，打开RetroArch，选择加载内核。（如果没有下载内核的话，要先下载内核Philips-CDi (SAME CDi)）下载完成之后关掉Retroarch。
然后，下载[BIOS](https://drive.google.com/file/d/110hzDtFX0NjOYr9Xnsxq5Mrh5tjJRoRj/view?usp=sharing)
把里面的三个文件 **（里面三个压缩包不用再解压！如果不行的话再解压）**解压到 %你的RetroArch系统文件夹（可以到设置-最后一个Directory-第一个System/BIOS中查看）%/same_cdi/bios中（如果文件夹没有就自己创建）。
最后，打开RetroArch,选择加载内容，选择你的ROM文件（仅支持.chd和.iso格式），就可以畅玩了！（进入BIOS后点击Play CD-i）效果图：
[![RpCsSz.png](https://www.helloimg.com/images/2022/05/12/RpCsSz.png)](https://www.helloimg.com/image/RpCsSz)

## 总结

这种方法虽然有些麻烦，但是解决了CD-i Emulator的一个硬伤：只能用鼠标操作。在这里你可以用键盘操作了！（键盘配置的教程自行百度）并且没有音画不同步的问题，但是加载速度有一点小慢，不过可以忍受。

