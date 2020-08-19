# 作恶的冰块

08.19.2020（月日年） 创建，08.19.2020 修改。

KurisuCat 整理资料 / 编写。

# 前言

如果您未参与到这场“战争”中，请关闭本页面。

如果您需要了解此事件也请留下。

**本页面非官方（QNotified 官方）页面**

如果有补充的话请提 [Issues](https://github.com/kurisucat/evil_bk/issues)，如果需要修正语法请提 [Pull resquests](https://github.com/kurisucat/evil_bk/pulls)。

*用户行为不代表 QNotified 开发团队立场，QNotified 开发团队不对用户的个人行为负责。*

# 什么是冰块？

冰块是一个增强 腾讯QQ 手机应用的 Xposed（以下简称 XP）模块。

这一切都很正常，对吧？但是接下来的信息可能会让你恶心。

冰块，全称“冰块高级模块”，是基于 KQ / QNotified 模块（以下简称 QN 模块）魔改而来。

> 魔改内容：修改部分文本。

冰块所有者魔改了 QN 模块之后辱骂 QN / KQ 模块作者，并且辱骂 “QQ 复读机” 模块作者（BUG）。QN 开发者得知后暂停了 QN 模块的开发，使冰块无法继续魔改 QN 模块。（但是开始魔改了其他 XP 模块）

> 虽然 KQ 模块也是基于 QN 模块魔改而来，但是 KQ 模块内署名了原版，QNotified 开发团队暂时没有追究。

并且，冰块所有者将冰块发布至所谓官方 QQ 群组，「葫芦侠」、「蓝奏云」等平台，并且冰块所有者发布了诸如「付费5元激活」、「QNotified抄袭冰块高级模块」等言论。

还有更多，诸如冰块模块没有开源，违反 QNotified 模块项目所使用的 GPLV3.0 开源协议。

目前（8月19日 2020年）冰块没有做出更多“坏事”。

KurisuCat 整理资料 / 编写。

# 分析冰块的apk，证明魔改

**大量图片警告。尽管图片已压缩处理，图片可能还是加载有点慢，请耐心等待**

> 冰块的下载地址：<https://www.lanzoui.com/b054ku65g>（欢迎以侵权为理由进行举报）

咱使用MT管理器打开冰块模块的apk（图）（这图标土的要死对吧→_→正经点的软件图标都是设计出来的）

![dlJab8.jpg](https://s1.ax1x.com/2020/08/19/dlJab8.jpg)

编辑classes.dex（图）

开   门   见   山

![dlYrdO.jpg](https://s1.ax1x.com/2020/08/19/dlYrdO.md.jpg)

dex里面的包名nil.nadph.qnotified是QN的。连这都不改，技术过差。

咱们简单搜索一下代码，QNotified之类的字符遍地都是。（图）

![dlNFUS.jpg](https://s1.ax1x.com/2020/08/19/dlNFUS.md.jpg)

想问问作者，既然这个软件是你自己做的，是QN盗版你的，那么为啥dex里面一搜全是QNotified？

冰块盗版QN的方法是替换常量，把QNotified换成冰块，文字变了，软件就是自己的了。

咱们康康这些常量（图）

![dlam7V.jpg](https://s1.ax1x.com/2020/08/19/dlam7V.md.jpg)

免费开源？我怎么没见过你开过源还免费？

