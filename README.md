## 设计系统编程

> [原文地址 https://www.programmingdesignsystems.com/](https://www.programmingdesignsystems.com/) <br>
> 这是一本由[Rune Madsen](https://twitter.com/runemadsen)编著的介绍平面设计新基础和实际应用的免费电子书。本书还在连载中，更新动态可以关注[这里](https://twitter.com/designsystemsin)。
> 翻译&校验：[neekychan](https://github.com/neekychan)([微博](https://weibo.com/cwlay)) 和 [freedom](https://github.com/yylifen)

### 介绍

*“我们现在正从面向对象的文化过渡到面向系统的文化。这里的变化不是来自于事物，而是来自于做事的方式。“*

> 引用自Jack Burnham (1968)《系统美学》

你认为平面设计师是一个什么样的角色呢？这个问题的答案可能大相径庭，但我的定义是这样的：平面设计师是一个以形状和颜色传达内容的人。这项工作可以采取多种形式，但直到最近，印刷产品已经成为它主要的形式，如海报、名片、书籍封面等。

今天，我们发现自己面临着新的挑战，这并不是因为设计的定义发生了很大变化，而是因为我们需要构建的产品发生了变化。我们现在大部分时间都花在屏幕上而不是纸上，这对懂得如何为数字设备设计的设计师产生了极大的需求。但是数字产品和印刷产品不一样。数字产品显示在不同尺寸和动态内容的屏幕上。数字产品允许用户利用动作和动画与其内容交互。此外，数字产品往往具有时间逻辑，线性叙事被一组复杂的状态和过渡动作所取代。总之，数字产品都有一个共同的特点：它们是用编程语言创建的。

对于一个植根于美术领域的人来说，这是一个艰难的转变。许多平面设计学校都采用了瀑布式教学理念，学生们可以认为自己是有创造性的人，为其他人提出构思。毕竟，这比采用一整套新流程更容易。然而，这种方法的基本问题是像Illustrator和Sketch这样的静态设计工具在数字系统原型设计中失败了。即使页面隐喻仍然普遍存在于网页设计中，这似乎限制了将设计定义为页面的样式。 因为搜索领域google.com的外观就是一个很好的网站吗？传统的美术是非常乐观的，这本书建立在这个基础之上。然而，在设计领域和技术的新进展之间存在长达一个世纪的联系，如果平面设计师不熟悉这种新的数字现实，它们将变得无关紧要。我们现在有能力编写能够产生漂亮设计的代码，未来的设计师理解如何实现这些讲师一项必备技能。

这本书讲述了一个简单问题的答案：当我们尝试使用编程语言作为设计师的工具重新定义平面设计课程时会发生什么？这个强大的概念包含几个方面。首先，平面设计师总是在他们的工作中使用系统。我们使用网格系统来平衡我们的布局和颜色环来选择有适当距离的颜色。历史告诉我们，系统可以治愈对空白画布的恐惧，将这些想法编码到实际软件中是一个强大的概念。其次，代码使设计人员能够做他们以前无法做的事情。在原型设计阶段，可以更快地测试设计的变化，并且可以用于揭示设计者永远不会用铅笔创建的随机化设计。第三，它使设计人员能够创建动态系统，可以根据时间，地点或用途改变他们的设计。在墙上投掷设计进行生产是印刷页面的遗留问题，设计过程没有理由以产品的诞生而结束。

这本书的结构就像一篇关于平面设计的介绍性文章，重点介绍视觉设计的元素以及它们与算法设计的关系。这本书是为希望成为更好的程序员的设计师而写的，反之亦然。当你阅读本文时，你会注意到它是从最基本的开始。代码很简单，练习也很有限。如果这感觉过于简单，请继续阅读。我们很快就会谈到更具挑战性的主题，但这些基本概念为一些更复杂的想法奠定了基础。在这本书的结尾，我希望你已经学到了两种新的技能：如何使用代码来创建新的有趣的平面设计，以及如何评估这些设计是否可以被认为是成功的。

我决定将[JavaScript库P5.js](http://p5js.org/)用于本书中的所有示例。事实证明，对于初学者来说，它提供了一个很好的编程环境，同时对高级用户来说也足够强大。我知道不可能选择一种适用于每个人的单一编程语言，读者可以根据具体项目需要的性质将这本书中的想法移植到其他语言和框架中。因此，我试图把文案写得尽可能通用。同样重要的是，要注意，这不是一本关于网页设计的书。虽然这些例子可以嵌入到任何网页上，但这些技术也可以应用于应用于数字和印刷工作。事实上，我看到我的学生多年来使用它创作了各种各样的设计，包括雕塑、绘画、时尚、摄影、游戏设计、网页设计和印刷品方面的项目。

这本书是为具有JavaScript编程入门知识的读者编写的，这意味着几乎没有时间用于解释变量、函数和循环等概念。对于这些读者，我强烈推荐Daniel Shiffman的[YouTube频道：Coding Rainbow](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA)，在那里Dan比以往任何时候都能更好地解释这些概念。这些视频还将介绍P5编程的基本概念。

我不是第一个写平面设计系统的作者，这本书写了很多来自不同作者的令人难以置信的想法，这些作者太多，不能在这里提及。我也不是第一个写代码和平面设计的人，但我对这一主题的书感到并不满意，这些书似乎分为两类：那些专注于代码和生成设计的人根本没有教授平面设计原则，而那些将计算设计作为一个场景来庆祝，而没有确定项目的制作方式或成功的原因。需要的教育材料，以现代的方式教授平面设计的基础知识，特别是如果它还为学生提供了批评数字设计项目的心理模型。

我选择在没有出版商的情况下免费在线出版这本书。其主要原因是自由。它允许我编写和设计我会阅读的书的类型。这反映在这本书的结构中，这本书由许多较短的章节组成，这些章节在网络上更容易阅读，并且教师可以直接在教室中重新组合（由于知识共享许可证，这完全合法）。我将以一种非线性的方式编写这些章节，研究我在特定时间发现最有趣的主题。完成的书没有具体的截止日期，尽管我将其作为一项全职工作。这本书的源代码可以在[GitHub](https://github.com/runemadsen/programmingdesignsystems.com/tree/master/content)上找到，我鼓励所有的读者提交问题或使用编辑的请求。要及时了解本书的进展情况，你还可以订阅实时资讯。

我要感谢一群人，没有他们，这本书就不可能存在。2009年，当我搬到纽约，在纽约大学的互动电信项目学习时，我只有一个模糊的概念，想要在艺术和代码的交汇处工作。作为一个主要为广告制作横幅的Flash开发者，在ITP工作的两年完全改变了我的想法。我要感谢丹·奥沙利文(DanO‘Sullivan)对这个项目的巨大支持，该项目始于ITP的一门课程，目前正在编写成一本书，而我当时是那里的一名研究人员。没有丹尼尔·希夫曼(DanielShiffman)的帮助和指导，这本书就不会存在，他的工作激励了成千上万的学生学习代码。我想感谢斯图尔特史密斯，他教的可视化数据类，从早期的想法，也是这本书的开始。我感谢所有帮助塑造这些想法的ITP教员和校友，包括Patrick Hebron、Greg Borenstein、Clay Shirky、Danny Rozin、Tom Igoe、David Nolen、Gabe Barcia-Colombo和George Agudow。特别感谢P5.js的原作者Lauren McCarthy，以及Casey Reas和Ben Fry在审阅方面的工作。我要感谢钱德勒·亚伯拉罕在色彩空间一章中的详细编辑，感谢克莱尔·科尔尼-沃尔普回答了我关于可访问性的众多问题，感谢玛丽亚·马尔卡德·詹森不懈的编辑工作。现在我们开始学习吧。
