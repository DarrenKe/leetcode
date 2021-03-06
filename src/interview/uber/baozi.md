聊Startup，不能不说Uber。该家在最近一轮融资中估值超过170亿美金，techcrunch几乎每隔几天就出现他家的新闻。这样火热的公司自然会吸引大量的申请者，所以小编抱着重在参与的心态，投了一下简历，没想到面试过程并没有想象的那么难，此为后话。Uber的业务发展很快，甚至算得上疯狂扩张。比如走在三番大街上的小编，到处可以看见身边的人在用Uber或者Lyft打车，手机App叫车的概念已经深入人心。从一个使用者的角度上讲，Uber或者Lyft在城市里或者机场确实很好用，方便快捷，给人一种全新的美好的打车体验。

面试地点：加州三藩市
面试时间：2014年5月份
HR Screen

回国过完年后，小编深感自己不能再懈怠下去啦，于是开始和另一个准备跳槽的好朋友开始刷起了Leetcode。刷完两遍后开始准备一些design相关的的题目：主要是看一些paper和网上的technical talk，总结整理一下平时工作中做过的Projects。感觉准备的差不多之后开始投了一些湾区的Start ups，感觉这些公司在疯狂融资之后，马上就是一轮大规模扩充Engineer team，机会很多。Uber也不例外，上来就是Recruiter电话面试：主要是问小编现在的情况，为什么选择uber而不是别的公司，范围基本上是典型的Behivor questions。好在小编之前做了很多功课，查看过各种报道Uber的视频和文章（已经到了炒作的级别），对他们的愿景也很认同，甚至是Uber app的忠实用户。所以这部分没出问题，顺利通过。

Skype Interview

Recruiter电面之后要求我做一个Project，给了几个选择，但范围基本上都是Location based application。实现要求"code it up and demo"，然后Skype面试会问实现细节和trade off。由于小编时间紧，所以Recruiter给了我另外一个选项：即选择自己以前最拿得出手的Project，然后面试官会Go through implementation detail并且提问。思索再三，小编发了之前做的一个web search engine的项目过去。电面通过Skype进行，面试官是一个Dev manager。在聊项目的时候，他提出了一些问题：例如这个Project解决的是什么问？系统架构是什么？解释某个Function是干什么的？等等。谈完Project之后，他又问了一些宽泛的系统设计方面的问题，比如如何实现Asynchronous service call？如何retry？讨论了一下Service oriented architecture的好处和弊端。其实小编谈自己的Project的时候准备的不好，毕竟是很久以前写的代码，很多Function的细节已经记不得了（引以为戒啊）。但后半部分答得还算是不错，System design，分布式系统，Service oriented architecture准备的不错，所以和对方聊的比较投机。面试结束前，面试官说希望能尽快安排Onsite interview。

Baozi Tip

Start up一般强调Cultural fit：就是看面试者对公司产品是不是了解，是不是和公司有同样的愿景，是不是对公司和产品有足够的Passion。小公司本来人就不多，除了技术这道门槛，Cultural fit也非常关键。建议要准备以下问题：Why our company? How do you improve our current product? What can you bring to us if we hire you.
技术方面要能和面试官聊得来，可以阅读一些System design and architecture的资料。关注一下当前比较流行的技术，大数据（Hadoop，Spark，Non-sql, Kafka)， Distributed system（Zookeeper），Service oriented architecture。当然关注包子博客也是必须的。
Onsite Interview

Uber的HQ坐落于SF Downtown金融区附近的一栋小楼，听说之前是Yelp’s office。简单寒暄之后，Recruiter给小编找了一个屋子，静坐开始等待面试官。

第一轮：系统设计问题 How to design netflix?

这个其实小编也不太了解，就尽量根据自己之前看过的资料开始一步一步给出自己的Solution，然后进行优化。架构上：基本上就是数据层，Service层，前端。因为小编知道Netflix是AWS的忠实用户，所以基本就以AWS为例：数据存储使用s3，配合Relational db / Non sql database；然后是Service layer，功能包括：User authentication，session management，data streaming and other business logic；前台则主要是用户界面。优化包括：如何Cache，如何利用CDN network replicate data close to the users. 因为Netflix的数据大部分是静态数据，很少更新，电影电视剧的内容完全可以Replicate很多份放到Internet的Edge server上。

第二轮：Deep dive personal project.

聊过去的项目，这种类型的面试真的是因人而异，以下是小编对它的理解：Project在技术上要Impressive，如果你能让面试官认可Project的架构设计甚至从你的Project里学到东西，他肯定会希望和你成为同事，这是面试中很重要的一个标准。在日常工作中，每个人都要和组员或者公司其他员工交流沟通很多，如果面试官发现很难和你交流、或者很难理解你的话，过关的几率会大大下降。所以这轮面试的重点就是测试面试者是否有能力进行有效的交流沟通，从面试官的角度，以后愿不愿意Work on something together。

Baozi Tip

因为这类面试通常是自己准备话题，所以可以提前找好朋友多Mock interview几次，这样子可以确保真正面试的时候可以说的有条理，有主有细。

第三轮：Behavior question / Cultural fit面试。

这一轮面试基本和HR Recruiter的那轮差不多，区别就是这次时间更长，想象一下45分钟全是Behavior question，面对面。小编个人觉得这一轮真的就是看前期的准备工作是不是到位：最起码要使用几次面试公司的产品，最好发现一些需要改进的地方，能说清楚产品的优点，大体了解公司的愿景，潜在的客户群体。然后尽量多关注关于公司的报道，记得当时Uber刚刚在纽约Launch delivery service，所以当小编跟面试官提到的时候，可以明显感觉到她是很高兴的。

第四轮：Coding + OO design (Design windows excel)

这个主要是看OO design的功底，其实不难。Follow-up question: In excel, one cell can refer to other cells, if I update one cell, how do you update all the dependent cells？这个问题可以被转化成经典的Topological sort，所以这里就不详细展开啦，如果不知道可以看看算法书，或者关注包子博客之后的总结。

Reflection

三四天后受到了他家offer，并不算特别Impressive package。感觉和Recruiter negotiate offer的时候，对方一副拽拽的样子：公司融资或者估值的信息不透露，要去组的Project很保密，所以基本无法了解入职后的情形，略高冷。在给Offer之后两星期爆出公司估值涨到17billion的消息，喜欢这种刺激的同学，请认真考虑Uber。（包子原创，转载请注明）