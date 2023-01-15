# 苹果设备，强制并有规律的熬夜解决方案

## 背景

​	这种想法源于我不想熬夜，但深知这是一个循序渐进的过程，所以需要一个能够强制熬夜，但又可以定期熬夜的解决方案，经过我几天熬夜的摸索，总结出了一个相对有效的解决方案。

## 原理

​	利用自动化技术，给你的电脑设置屏幕时间密码，这个密码是不可见的，密码通过网站生成一个只有三天之后才能访问的链接，只有三天之后你才能拿到密码，否则你只能强制性的去睡觉。

## 达成效果

- 说明：以下效果是电脑电脑自动执行的过程，你可以看着电脑自动执行，保证密码被正确设置，保证执行无误，而且你在全程无法看到密码，最后密码只能通过生成的链接和密码三天之后才能拿到。
- 如果你使用的是苹果全家桶，那么这个方案很适合你

ps:youtube演示视频，需翻墙
[![苹果设备，强制并有规律的熬夜解决方案](https://res.cloudinary.com/marcomontalbano/image/upload/v1673771554/video_to_markdown/images/youtube--_b0qzMdgXK8-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://youtu.be/_b0qzMdgXK8 "苹果设备，强制并有规律的熬夜解决方案")
## 前提条件

- 一台mac

## 教程

- 下载录屏自动化软件`Keysmith`，点击下载：https://www.keysmith.app/

- 生成密码网站使用了github的项目，改了源代码，使其能够把生成的密码隐藏，并自动复制到自己的剪贴板上
  - 源项目：https://github.com/52admln/ram-password
  - 改后的项目：https://github.com/MisteryLiuCode/PwdRamClip.git
  - 或者使用我的链接：http://pwd.misteryliu.top/
- 给密码生成链接的网站同样是修改了源代码
  - 源项目：https://github.com/BillKeenan/dead-drop-python
  - 改后的项目：https://github.com/MisteryLiuCode/GenLinkPeriod.git
  - 此代码最好部署在别人服务器上，或者使用我的链接生成：http://msg.misteryliu.top/

- 在给电脑设置屏幕时间密码的时候，原生不支持直接粘贴的方式设置密码，而使用键盘的方式使输入又暴露了密码，可以使用以下软件强制粘贴，下载方式
  - https://github.com/EugeneDae/Force-Paste
  - 如果不能使用，大概率可以通过这里找到答案
    - https://github.com/EugeneDae/Force-Paste/issues/12
- 最后的一步调出弹窗，输入1234使用的软件是`bob`，，此目的是为了覆盖之前的剪贴板，使密码彻底不可见！，软件链接的点这里https://github.com/ripperhe/Bob
- 接下来就靠你自由发挥了，如果有不懂的或者有新的想法欢迎提Issue，或者给我发邮件：misteryliu@outlookc.om
