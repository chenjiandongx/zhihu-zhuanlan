# 如何分析一个知乎大 V 的专栏文章

最近今日头条签约知乎大 V 的消息让人议论纷纷，当然，这对我来说没有半毛钱关系，我也不用瞎操心这个。  
我只是来尝试简单分析一个大 V 的专栏文章，就拿 [路人甲](https://www.zhihu.com/people/sgai) 的知乎专栏 [学习编程](https://zhuanlan.zhihu.com/passer) 来举例

![passer](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/passer.png)

**已关注** 看到没有，我一直紧跟着路人甲大哥的步伐。  
首先先爬取专栏的所有文章的信息，共 123 篇，包括作者，作者首页，文章标题，文章地址，发布时间，点赞数，评论数等信息

专栏作者及文章数量信息
* 102 [路人甲](https://www.zhihu.com/people/sgai)
* 11 [stormzhang](https://www.zhihu.com/people/stormzhang)
* 2 [Crossin](https://www.zhihu.com/people/crossin)
* 1 [林安](https://www.zhihu.com/people/lin-an-71)
* 1 [简浅](https://www.zhihu.com/people/jianzu1126)
* 1 [龚元浩](https://www.zhihu.com/people/gongyuanhao)
* 1 [迪公主](https://www.zhihu.com/people/dorothy-33-6)
* 1 [Wayne Shi](https://www.zhihu.com/people/sw2016)
* 1 [Ray Cao](https://www.zhihu.com/people/xi-lan-hua-66)
* 1 [Glowin](https://www.zhihu.com/people/glow)
* 1 [Brian Way](https://www.zhihu.com/people/brianway)

可以看到，路人甲自己有 103 篇，stormzhang 有 11 篇，其余均为作者的文章数均为个位数。

分别排序出点赞数和评论数前 10 的文章

点赞数
* 8301 [微信消息防撤回工具](https://zhuanlan.zhihu.com/p/25706692)
* 7349 [如何学习Python爬虫[入门篇]？](https://zhuanlan.zhihu.com/p/21479334)
* 6237 [程序员常用的技术网站](https://zhuanlan.zhihu.com/p/21638054)
* 4530 [豆瓣5.6分的《西游伏妖篇》评论有水军吗？](https://zhuanlan.zhihu.com/p/25047215)
* 3646 [哪些比较好的在线编程网站？](https://zhuanlan.zhihu.com/p/21808087)
* 3424 [程序员把妹指南之电脑配置篇](https://zhuanlan.zhihu.com/p/21771612)
* 3422 [如何一步一步的学Java](https://zhuanlan.zhihu.com/p/21454718)
* 3339 [Google Interview University - 坚持完成这套学习手册，你就可以去 Google 面试了](https://zhuanlan.zhihu.com/p/22881223)
* 2987 [哪些知乎收藏夹关注数超过一万？](https://zhuanlan.zhihu.com/p/22687249)
* 2975 [Java工程师笔试题整理[校招篇]](https://zhuanlan.zhihu.com/p/21513402)


评论数
* 697 [豆瓣5.6分的《西游伏妖篇》评论有水军吗？](https://zhuanlan.zhihu.com/p/25047215)
* 653 [微信消息防撤回工具](https://zhuanlan.zhihu.com/p/25706692)
* 555 [如何学习Python爬虫[入门篇]？](https://zhuanlan.zhihu.com/p/21479334)
* 378 [程序员常用的技术网站](https://zhuanlan.zhihu.com/p/21638054)
* 349 [C、C++语言学习资料](https://zhuanlan.zhihu.com/p/21472075)
* 320 [你所不知道的周黑鸭和绝味鸭脖。](https://zhuanlan.zhihu.com/p/23151994)
* 265 [国庆节，我们用代码来画个国旗～](https://zhuanlan.zhihu.com/p/22754747)
* 260 [程序员把妹指南之电脑配置篇](https://zhuanlan.zhihu.com/p/21771612)
* 248 [爬取知乎60万用户信息之后的简单分析](https://zhuanlan.zhihu.com/p/24411711)
* 231 [有哪些适合新手练手的Python项目？](https://zhuanlan.zhihu.com/p/22164270)

### 点赞数-评论数

先看评论数超过 300 的文章，共 6 篇

![scatter-0](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/scatter-0.png)

虽有波动，但总体上随着点赞数增多还是呈上升趋势的

总体情况

![scatter-1](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/scatter-1.png)

点赞数 < 2000 并且评论数 < 100 格子所占的比例是最大的

### 发布日期
![line-0](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/line-0.png)

可以看到，该专栏从 2016 年 5 月发表了第一篇文章，该年 7 月份是创作高潮，发表了 16 篇文章。不过 2017 年总体发布文章的频率还是不如 2016 年。截止到 2017 年 8 月，每月平均发表 7.69 篇文章。

每个月份文章的总点赞数

![line-1](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/line-1.png)

平均每月能获得 9938.56 个赞 

每个月份文章的总评论数

![line-2](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/line-2.png)

平均每月能获得 702 条评论

从这两张图的可以很明显地看出来，总体的趋势基本上是一致的。即点赞数和评论数基本上还是能成正比的。

### 发布时间
一天 24 小时中，哪个时间发布文章的频率最高呢？

![pie-0](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/pie-0.png)

早上 7 点和 8 点是最常发布文章的时间，所占的比例都超过 60% 了

把这两个时间暂时先取出，看看其他时间点的比例

![pie-1](https://github.com/chenjiandongx/zhihu-zhuanlan/blob/master/images/pie-1.png)

这下比例就相差不是特别大了。不过总体上来讲还是白天要大于晚上的。活还是得留在白天干，是吧。