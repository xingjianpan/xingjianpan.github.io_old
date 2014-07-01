---
layout: post
title: (译文)大数据行业信息图以及一些思考
date: 2014-7-1 14:16:36
categories: data
author: Xingjian Pan

---


### [The State Of Big Data in 2014: a Chart](http://mattturck.com/2014/05/11/the-state-of-big-data-in-2014-a-chart/)

##### 原著 MATT TURCK 翻译 [XINGJIAN PAN](http://xingjian.me)

##### 转载请注明出处



从我第一次尝试为繁荣发展的大数据生态系统绘制一张信息图已经过去了两年， 而这期间大数据行业发生了很多巨大的变化。 我早就该对这张图做一个更新，现在终于完成了。


<a href="https://raw.githubusercontent.com/xingjianpan/xingjianpan.github.io/master/_posts/big_data_map.png"><img width="600" height="400" src="https://raw.githubusercontent.com/xingjianpan/xingjianpan.github.io/master/_posts/big_data_map.png"></a>



从VC的角度，我想谈谈对这张图以及大数据行业的一些想法：


**越来越拥挤**：创业者们蜂拥至这个行业， VC们将大笔的资金投资到看起来有机会成功的创业公司，其结果是，这个行业正变得越来越拥挤。 一些类别如数据库（不管是[NoSQL](http://en.wikipedia.org/wiki/NoSQL)还是[NewSQL](http://en.wikipedia.org/wiki/NewSQL)）和社交媒体数据分析正趋于成熟，且开始出现并购或者淘汰出局（Twitter对BlueFin[^BlueFin]和GNIP[^GNIP]的收购可能意味着在社交媒体数据分析领域这种趋势早已经开始了）。 对于后来者来说， 虽然空间依然存在，但看起来早期的大笔风投资金都下注在基础设施（infrastructure）和分析（analytics）领域，导致成功的标准变得越来越高。 不过， 这并不意味着VC的资金会停止流入这些领域。

对于一些领域，公司的数量之多显然已经达到了一张地图所能容纳的上限。 我相信还有一些不错的公司我们没能纳入进来，也许是我们没有发现，也许是因为地方不够了， 我在此表示非常抱歉， 同时我也希望大家在评论里对于应当纳入那些公司提出反馈和意见。


**尚处在早期阶段**： 总体而言，这个市场还处在发展的早期阶段。 过去几年， 一些被看好的公司失败了（如[Drawn to Scale](http://drawntoscale.com/)），一些公司的创业者提前退出了[^提前退出了] (例如： [Precog](http://precog.com/) [^Precog], Prior Knowledge, [Lucky Sort](http://luckysort.com/)[^LuckySort], [Rapleaf](https://www.rapleaf.com/), Nodeable[^Nodeable], [Karmasphere](http://www.karmasphere.com/)[^Karmasphere], 等 )，还有一些的结局稍好(例如: [Infochimps](http://www.infochimps.com/)[^Infochimps], Causata[^Causata], Streambase[^Streambase], ParAccel[^ParAccel], [Aspera](http://asperasoft.com/)[^Aspera], GNIP, BlueFin labs, [BlueKai](http://bluekai.com/)[^BlueKai])。

与此同时，一些公司看起来正越做越大，并获得大笔惊人的风投注资（比如， MongoDB 已经融资超过2.3亿美元， Palantir融资近9亿美元， Cloudera近10亿美元[^Cloudera] 。一些大公司正积极出击进行并购（Oracle收购BlueKai， IBM收购[Cloudant](https://cloudant.com/)[^Cloudant]），但是总体而言，多数公司离成功实现IPO和投资者功成身退还差的很远（虽然 [Splunk](http://www.splunk.com/?r=header)[^Splunk] 和 [Tableau](http://www.tableausoftware.com/)[^Tableau]做到了）。 在很多类别，创业公司和大公司互相竞争，但并没有出现市场领导者。


**市场宣传遭遇现实**:在经历这些年狂轰滥炸的市场宣传之后，大数据还是焦点么？未来几年，也许大数据不再是媒体的热门，但对于大数据市场而言却是至关重要的， 因为企业将要开始把大数据项目从试验转而全面的部署实施。 虽然这意味着一些大数据提供商的利润会迅猛增长，但同时这些项目也将成为大数据是否能带来它所宣传的价值的一块试金石。与此同时，随着“物联网”行业的迅速崛起，数据将会如潮水般加速增长，进一步推高市场对大数据技术的需求。


**基础设施**：[Hadoop](http://hadoop.apache.org/)似乎已经奠定了其作为整个大数据生态系统的关键部分，一些竞争者依然虽在， 这一领域也许会进一步发展和整合。 [Sprak](http://spark.apache.org/)是另一个的基于Hadoop分布式文件系统（HDFS[^HDFS]）的开源框架，它试图填补Hadoop的弱项，提供更快的的数据分析和良好的编程接口，目前正吸引大量关注（一些迹象显示它做的还不错）。一些主题（比如，实时数据处理）依然是重中之重，同时新的主题也在不断涌现（比如，新一代处理、变换、清洗数据的工具，包括[Trifacta](http://www.trifacta.com/)， [Paxata](http://www.paxata.com/) 和 [DataTamer](http://www.tamr.com/)）。 企业数据是否会真正的放到云里（公共云或私有云），如果是，还有多久才发生，将是另一个大的话题。很多人认为财富500公司在接下来的几年来会继续把数据（以及处理数据的软件）放在机房里。一批云服务+Hadoop的创业公司则认为长期来看，所有的数据最终都会放到云中。


**分析工具**：从创业公司和VC投资的数量来看，这一领域最为活跃。从excel表格式的用户界面，到时间轴动画和3D动画， 创业公司提供各种各样的数据分析工具和用户界面，而不同的客户也确实有不同的需求，所以这一领域大概依然有足够的发展空间。推广产品的策略也不尽相同 --- 有些创业公司更针对于数据科学家，这群人目前不多但增长迅速。 另一些则正好相反，他们销售自动化的解决方案给一般商业用户，完全忽略数据科学家的存在。

**大数据应用**： 正如之前预测的，大数据缓慢但的确朝着应用层面发展。 这张图列出了一些令人兴奋的创业公司 -- 他们本质上都是基于大数据技术和工具（当然我们无法把所有的相关公司都在这里列出来）。一些公司提供横向应用[^横向应用] --- 如基于大数据的营销系统，客户关系管理系统和欺诈甄别解决方案。 金融业和广告科技业一直是大数据推广的领导者和最早的拥趸，甚至早于大数据被称作大数据。慢慢的，大数据推广到各行各业，如医疗行业和生化行业（特别是基因研究领域）和教育行业。现在才刚刚开始。

*特别感谢我在FirstMark的同事Sutian Dong，她为这张图做了很多的基础工作。以及我在彭博Beta的前同事Shivon Zilis，他对这张图的之前版本做了巨大的贡献。*



#### 原文作者Matt Turck曾任Bloomberg Ventures常务董事，现为FirstMark Capital合伙人。


[^BlueFin]: [TWITTER ACQUIRES SOCIAL TV ANALYTICS BLUEFIN LABS](http://www.fastcompany.com/3005470/twitter-acquires-social-tv-analytics-bluefin-labs)
[^GNIP]:[Twitter Acquires Longtime Partner And Social Data Provider Gnip](http://techcrunch.com/2014/04/15/twitter-acquires-longtime-partner-and-social-data-analytics-provider-gnip/)
[^提前退出了]:原文为 a number saw early exits
[^Precog]:[RichRelevance Acquires Precog To Add Large-Scale Analytics Engine To E-Commerce Personalization Platform](http://techcrunch.com/2013/08/14/richrelevance-acquires-precog-to-add-large-scale-analytics-engine-to-e-commerce-personalization-platform/)
[^LuckySort]:[Twitter Acquires Big Data Visualization Startup Lucky Sort, Service To Shutter In Months Ahead](http://techcrunch.com/2013/05/13/twitter-acquires-big-data-visualization-startup-lucky-sort-service-to-shutter-in-months-ahead/)
[^Nodeable]:[Appcelerator Acquires Nodeable to Provide Next Generation Real-Time Data Insights](http://www.appcelerator.com/press-releases/appcelerator-acquires-nodeable-real-time-mobile-analytics/)
[^Karmasphere]:[Hadoop analytics startup Karmasphere sells itself to FICO](http://gigaom.com/2014/04/17/hadoop-analytics-startup-karmasphere-sells-itself-to-fico/)
[^Infochimps]:[CSC buys Infochimps and its big data platform](http://gigaom.com/2013/08/07/csc-buys-infochimps-and-its-big-data-platform/)
[^Causata]:[NICE to Acquire Causata to Enable a Seamless Customer Experience across the Web and Contact Center](http://www.nice.com/nice-acquire-causata-enable-seamless-customer-experience-across-web-and-contact-center)
[^Streambase]:[TIBCO SOFTWARE ACQUIRES STREAMBASE SYSTEMS](http://www.tibco.com/company/news/releases/2013/press1274.jsp)
[^ParAccel]:[Actian Acquires MPP Big Data Market Leader ParAccel](http://www.actian.com/company/news-and-events/press-releases/actian-paraccel/)
[^Aspera]:[IBM Buys Aspera, A File Transfer Company That Counts Apple And Netflix As Customers](http://techcrunch.com/2013/12/19/ibm-buys-aspera-a-file-transfer-company-that-counts-apple-and-netflix-as-customers/)
[^BlueKai]:[Oracle Buys BlueKai](http://www.oracle.com/us/corporate/press/2150812)
[^Cloudera]:[Cloudera创始人Amr Awadallah：创业三年，如何获得10亿美元融资](http://www.csdn.net/article/2012-04-25/2805001)
[^Cloudant]:[IBM to Acquire Cloudant: Open, Cloud Database Service Helps Organizations Simplify Mobile, Web App and Big Data Development](http://www-03.ibm.com/press/us/en/pressrelease/43238.wss)
[^Tableau]:[Big Data Analytics Specialist Tableau Software Raises $254M In IPO, Shares Close 64% Up; Marketo’s First Day Up 78% To $23.10](http://techcrunch.com/2013/05/17/big-data-visualization-goes-public-tableau-software-raises-254m-as-shares-pop-58-while-marketo-raises-85m/)
[^Splunk]:[Splunk Prices Initial Public Offering](http://www.splunk.com/view/splunk-prices-initial-public-offering/SP-CAAAGW7)
[^HDFS]:[What is the Hadoop Distributed File System (HDFS)?](http://www-01.ibm.com/software/data/infosphere/hadoop/hdfs/)
[^横向应用]:指广泛适合各个行业的应用，[wiki](http://en.wikipedia.org/wiki/Horizontal_market_software