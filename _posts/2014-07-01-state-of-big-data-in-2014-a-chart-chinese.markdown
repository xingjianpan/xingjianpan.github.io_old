---
layout: post
title: 大数据行业现状
date: 2014-7-1 14:16:36
categories: data
author: Xingjian Pan

---


### [The State Of Big Data in 2014: a Chart](http://mattturck.com/2014/05/11/the-state-of-big-data-in-2014-a-chart/)

##### 原著 MATT TURCK 翻译 [XINGJIAN PAN](http://xingjian.me)

##### 转载请注明出处



从我第一次尝试为繁荣发展的大数据生态系统绘制一张信息图已经过去了两年， 而这期间大数据行业发生了很多巨大的变化。 我早就该对这张图做一个更新，现在终于完成了。

<iframe src="//www.slideshare.net/slideshow/embed_code/34540368" width="427" height="356" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px 1px 0; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> <div style="margin-bottom:5px"> <strong> <a href="https://www.slideshare.net/mjft01/big-data-landscape-matt-turck-may-2014" title="Big data landscape v 3.0 - Matt Turck (FirstMark) " target="_blank">Big data landscape v 3.0 - Matt Turck (FirstMark) </a> </strong> from <strong><a href="http://www.slideshare.net/mjft01" target="_blank">Matt Turck</a></strong> </div>


从VC的角度，我想谈谈对这张图以及大数据行业的一些想法：


**越来越拥挤**：创业者们蜂拥至这个行业， VC们将大笔的资金投资到看起来有机会成功的创业公司，其结果是，这个行业正变得越来越拥挤。 一些类别如数据库（不管是NoSQL还是NewSQL）和社交媒体数据分析正趋于成熟，且开始出现并购或者淘汰出局（Twitter对BlueFin和GNIP的收购可能意味着在社交媒体数据分析领域这种趋势早已经开始了）。 对于后来者来说， 虽然空间依然存在，但看起来早期的大笔风投资金都下注在基础设施（infrastructure）和分析（analytics）领域，导致成功的标准变得越来越高。 不过， 这并不意味着VC的资金会停止流入这些领域。

对于一些领域，公司的数量之多显然已经达到了一张地图所能容纳的上限。 我相信还有一些不错的公司我们没能纳入进来，也许是我们没有发现，也许是因为地方不够了， 我在此表示非常抱歉， 同时我也希望大家在评论里对于应当纳入那些公司提出反馈和意见。


**尚处在早期阶段**： 总体而言，这个市场还处在发展的早期阶段。 过去几年， 一些被看好的公司失败了（如Drawn to Scale），一些公司的创业者提前退出了（early exit）(例如： Precog, Prior Knowledge, Lucky Sort, Rapleaf, Nodeable, Karmasphere, 等 )，还有一些的结局稍好(例如: Infochimps, Causata, Streambase, ParAccel, Aspera, GNIP, BlueFin labs, BlueKai)。

与此同时，一些公司看起来正越做越大，并获得大笔惊人的风投注资（比如， MongoDB 已经融资超过 2.3亿美元， Palantir融资近9亿美元， Cloudera近10亿美元 [相关报道](http://www.csdn.net/article/2012-04-25/2805001)）。一些大公司正积极出击进行并购（Oracle收购BlueKai， IBM收购Cloudant），但是总体而言，多数公司离成功实现IPO和投资者功成身退还差的很远（虽然 Splunk和 Tableau做到了）。 在很多类别，创业公司和大公司互相竞争，但并没有出现市场领导者。


**市场宣传遭遇现实**:在经历这些年狂轰滥炸的市场宣传之后，大数据还是焦点么？未来几年，也许大数据不再是媒体的热门，但对于大数据市场而言却是至关重要的， 因为企业将要开始把大数据项目从试验转而全面的部署实施。 虽然这意味着一些大数据提供商的利润会迅猛增长，但同时这些项目也将成为大数据是否能带来它所宣传的价值的一块试金石。与此同时，随着“物联网”行业的迅速崛起，数据将会如潮水般加速增长，进一步推高市场对大数据技术的需求。


**基础设施**：Hadoop似乎已经奠定了其作为整个大数据生态系统的关键部分，一些竞争者依然虽在， 这一领域也许会进一步发展和整合。 Sprak是另一个的基于Hadoop分布式文件系统（HDFS）的开源框架，它试图填补Hadoop的弱项，提供更快的的数据分析和良好的编程接口，目前正吸引大量关注（一些迹象显示它做的还不错）。一些主题（比如，实时数据处理）依然是重中之重，同时新的主题也在不断涌现（比如，新一代处理、变换、清洗数据的工具，包括Trifacta， Paxata 和 DtaTamer）。 企业数据是否会真正的放到云里（公共云或私有云），如果是，还有多久才发生，将是另一个大的话题。很多人认为财富500（Fortune 500）公司在接下来的几年来会继续把数据（以及处理数据的软件）放在机房里。一批云服务+Hadoop的创业公司则认为长期来看，所有的数据最终都会放到云中。


**分析工具**：从创业公司和VC投资的数量来看，这一领域最为活跃。从excel表格式的用户界面，到时间轴动画和3D动画， 创业公司提供各种各样的数据分析工具和用户界面，而不同的客户也确实有不同的需求，所以这一领域大概依然有足够的发展空间。推广产品的策略也不尽相同 --- 有些创业公司更针对于数据科学家，这群人目前不多但增长迅速。 另一些则正好相反，他们销售自动化的解决方案给一般商业用户，完全忽略数据科学家的存在。

**大数据应用**： 正如之前预测的，大数据缓慢但的确朝着应用层面发展。 这张图列出了一些令人兴奋的创业公司 -- 他们本质上都是基于大数据技术和工具（当然我们无法把所有的相关公司都在这里列出来）。一些公司提供横向应用（译者注，指广泛适合各个行业的应用，[wiki](http://en.wikipedia.org/wiki/Horizontal_market_software)） --- 如基于大数据的营销系统，客户关系管理系统和欺诈甄别解决方案。 金融业和广告科技业一直是大数据推广的领导者和最早的拥趸，甚至早于大数据被称作大数据。慢慢的，大数据推广到各行各业，如医疗行业和生化行业（特别是基因研究领域）和教育行业。现在才刚刚开始。

*特别感谢我在FirstMark的同事Sutian Dong，她为这张图做了很多的基础工作。以及我在彭博Beta的前同事Shivon Zilis，他对这张图的之前版本做了巨大的贡献。*



#### 原文作者Matt Turck曾任Bloomberg Ventures常务董事，现为FirstMark Capital合伙人。

