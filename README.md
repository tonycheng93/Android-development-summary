#	Android	开发资料汇总

学习Android开发这一路走来，深知自学的不易。刚开始接触某一个新兴的技术，总是在网上漫无目的的搜索各种文章，而这些文章良莠不齐的，浪费了大量时间来辨别这些东西是否对自己有用。后来在github上面看到了许多优秀的开源项目，浏览器收藏夹也不知道到底收藏了多少，但是没有一个很好的分类。于是便萌生了一个想法，自己把学习过程中查阅的优秀文章和开源项目做一个整理。同时也会分享一些自己觉得能够提高工作效率的工具。希望这份资料能够给刚开始学习Android的开发者提供一点帮助，节约一些查找资料的时间。原始的markdowm文件已经放到github上，欢迎[下载和star](https://github.com/tonycheng93/Android-development-summary) 。这份资料我会不断的完善，也欢迎一些经验丰富的开发者可以一起来完善，直接[pull request](https://github.com/tonycheng93/Android-development-summary/pulls) 或者[issue](https://github.com/tonycheng93/Android-development-summary/issues)，我会定期筛选合并，有一些好的建议和意见随时[联系我](#联系我)，欢迎转载，谢谢收藏。
##	目录
-  [图片加载库](#图片加载库)

-  [图片处理库](#图片处理库)

-  [网络请求库](#网络请求库)

-  [网络缓存](#网络缓存)

-  [数据解析](#数据解析)

-  [常用网站](#常用网站)

-  [博客推荐](#博客推荐)

-  [微信公众号推荐](#微信公众号推荐)

-  [书籍推荐](#书籍推荐)

-  [RxJava系列](#RxJava系列)

-  [开发工具](#开发工具)

-  [Android Studio常用插件](#Android Studio常用插件)

-  [联系我](#联系我)

##	图片加载库

|                   图片库                    |    作者    |                   推荐理由                   |
| :--------------------------------------: | :------: | :--------------------------------------: |
| [Glide](https://github.com/bumptech/glide) | bumptech | 支持Gif，google官方推荐的图片加载库，在google的众多App中都采用了该库 ;[Google I/O 2014 Glide 介绍](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0327/2650.html);[Glide非官方文档，超详细，值得看](http://mrfu.me/2016/02/27/Glide_Getting_Started/)|
| [Fresco](https://github.com/facebook/fresco) | Facebook | 支持Gif，Facebook出品，必属精品，Fresco另辟蹊径使用Native方法来管理图片，专注解决图片内存溢出问题;[Fresco官方文档中文翻译版，"秋百万"作品，Fresco看着就够了](https://www.fresco-cn.org/docs/)|
| [Picasso](https://github.com/square/picasso) |  Square  | 开源大户Square出品，和Glide用法极其相似，Glide体积更小，JakeWharton大神所在公司[Picasso官方文档](http://square.github.io/picasso/) |
| [Android-Universal-Image-Loader](https://github.com/nostra13/Android-Universal-Image-Loader) | nostra13 | 老牌图片加载库，在上述图片加载库没出来之前，使用最多的开源图片库。但是，该项目已被作者废弃不再维护，不建议使用，用来学习图片异步加载和图片管理还是极好的[Android-Universal-Image-Loader源码解析](http://a.codekk.com/detail/Android/huxian99/Android%20Universal%20Image%20Loader%20%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90) |

##  图片处理库
|图片处理库|推荐理由|
|:------:|:------:|
|[glide-transformations](https://github.com/wasabeef/glide-transformations)|结合Glide使用，基本满足对图片的常见处理|
|[picasso-transformations](https://github.com/wasabeef/picasso-transformations)|结合Picasso使用，基本满足对图片的常见处理|

##	网络请求库

|   网络库    |   作者   |                   推荐理由                   |
| :------: | :----: | :--------------------------------------: |
|  [OkHttp](http://square.github.io/okhttp/)  | Square | Google在6.0中删除了HttpClient API代码。取而代之的是OkHttp，已被google官方认可，值得信赖。[Android OkHttp完全解析 是时候来了解OkHttp了](http://blog.csdn.net/lmj623565791/article/details/47911083)；[拆轮子系列：拆OkHttp](http://blog.piasy.com/2016/07/11/Understand-OkHttp/) |
| [Retrofit](https://square.github.io/retrofit/) | Square | 基于OkHttp，Square出品。非常适用于ResetFul API格式网络请求，与RxJava结合有奇效。[Retrofit源码解析](http://blog.piasy.com/2016/06/25/Understand-Retrofit/)；[codeKK Retrofit源码解析](https://github.com/android-cn/android-open-project-analysis/tree/master/tool-lib/network/retrofit) |
|  [Volley](https://developer.android.com/training/volley/index.html)  | Google | Google官方出品，适用于数据量不大，但网络通信频繁的场景，不适用于大文件读取、上传场景。[Volley源码解析系列文章，郭神作品](http://blog.csdn.net/guolin_blog/article/details/17482095)；[codeKK Volley源码解析](http://www.codekk.com/blogs/detail/54cfab086c4761e5001b2542) |

##	网络缓存

|                   缓存库                    |     作者      |                   推荐理由                   |
| :--------------------------------------: | :---------: | :--------------------------------------: |
| [DiskLruCache](https://github.com/JakeWharton/DiskLruCache) | JakeWharton | JakeWharton大神的杰作，缓存神奇，值得信赖。源码解析和用法参考文章：[Android DiskLruCache完全解析，硬盘缓存的最佳方案](http://blog.csdn.net/guolin_blog/article/details/28863651)，[Android DiskLruCache源码解析 硬盘缓存的绝佳方案](http://blog.csdn.net/lmj623565791/article/details/47251585) |
| [ASimpleCache](https://github.com/yangfuhai/ASimpleCache) |     杨福海     | afinal框架作者，国内Android大神。它是一个为Android制定的轻量级的缓存框架，只有一个java文件。支持自定义缓存路径、大小、缓存超时时间等。[ASimpleCache源码分析](http://blog.csdn.net/zhoubin1992/article/details/46379055) |

##  数据解析

|解析工具|作者|推荐理由|
|:------:|:------:|:------:|
|[Gson](https://github.com/google/gson)|Google|Google官方出品，值得信赖|
|[FastJson](https://github.com/alibaba/fastjson)|阿里巴巴|号称Java语言中最快的Json库[官方文档](https://github.com/alibaba/fastjson)|

##  常用网站
|网站名称|推荐理由|
|:-----:|:------:|
|[Google](https://www.google.com/)|google搜索，码农必用搜索引擎(首先你要会翻墙:joy:)|
|[Android官网](https://developer.android.com/index.html)|Android官网，Android开发必看的网站，API Guides、Training(你还是要会翻墙:joy:)|
|[Github](https://github.com/)|全世界最大的同性交友网站:sweat_smile:，拥有众多的优秀开源项目，你想要的它都有|
|[StackOverflow](http://stackoverflow.com/)|最专业的技术问答网站，不要英语而放弃使用它，你遇到的问题基本都可以在上面找到答案|
|[CSDN](http://www.csdn.net/)|全球最大的中文IT社区，众多的博主在上面分享自己的文章|

##	博客推荐

|                   博客地址                   |                    简介                    |
| :--------------------------------------: | :--------------------------------------: |
| [Android Developers Blog](http://android-developers.blogspot.com/) |   Android官网博客，有Android开发第一手资料，英文，需要翻墙。   |
| [郭霖](http://blog.csdn.net/guolin_blog/)  | 人称"郭神"，CSDN著名博主，著有"第一行代码"，Android开发入门必看书籍。 |
| [张鸿洋](http://blog.csdn.net/lmj623565791/) |        CSDN著名博主，博客文章很有深度，参考价值很大。         |
|  [徐宜生](http://blog.csdn.net/eclipsexys)  | CSDN著名博主，著有《Android群英传》和《Android群英传：神兵利器》，擅长自定义View。 |
| [任玉刚](http://blog.csdn.net/singwhatiwanna) |     百度Android工程师，著有《Android开发艺术探索》。      |
|     [代码家](http://blog.daimajia.com/)     | "干活集中营"作者,做库达人，发表很多开源库，他的"干活集中营"免费提供API接口供开发者使用。 |
|     [Trinea](http://www.trinea.cn/)      | codeKK项目发起人，收集了众多的开源项目以及开源项目源码分析，查看开源项目源码的好地方。 |
|   [大头鬼](http://blog.csdn.net/lzyzsd/)    |     阿里巴巴工程师，力推RxJava，写了一系列RxJava文章。      |
|     [Piasy](http://blog.piasy.com/)      |        翻译达人，翻译了众多国外技术文档和开源项目源码分析。        |
|[廖祜秋](https://www.liaohuqiu.net/)|人称"秋百万"，Ultra-Pull-To-Refresh开源库作者，Facebook开源图片加载库Fresco翻译作者|


##	微信公众号推荐
|微信公众号ID|推荐理由|
|:------:|:------:|
|guolin_blog|"郭神"的公众号必须关注，每天都会有优质的技术文章推送，接受投稿|
|hongynagAndroid|CSDN博客专家，每天都会有高质量的文章推动|
|codek2|codeKK微信公众号，专注于Android开源分享、源码解析、框架设计、内推，由Trinea维护|

##  书籍推荐
|书籍名称|推荐理由|
|:------:|:------:|
|[第一行代码](https://book.douban.com/subject/25942191/)|“郭神”作品，新人入门必看书籍|
|[Android群英传](https://book.douban.com/subject/26599539/)|"徐医生"大作，适合有一定Android基础的读者|
|[Android 源码设计模式解析与实战](https://book.douban.com/subject/26644935/)|作者何红辉/关爱民，阿里巴巴旗下友盟的高级程序员，CSDN博客专家，将Android源码与设计模式完美结合起来，进阶必看书籍|
|[Android编程权威指南（第2版）](https://book.douban.com/subject/26789110/)|美国一家移动技术开发培训机构出版的书籍，十分专业，推荐阅读|

##  RxJava系列
|文章地址|推荐理由|
|:------:|:------:|
|[给 Android 开发者的 RxJava 详解](https://gank.io/post/560e15be2dca930e00da1083)|扔物线大作，RxJava入门必看文章|
|[RxJava 与 Retrofit 结合的最佳实践](https://gank.io/post/56e80c2c677659311bed9841)|匠心写作上一篇非常不错的RxJava与Retrofit结合的实战类文章|
|[关于RxJava的系列文章](https://github.com/lzyzsd/Awesome-RxJava)|收集了一系列关于RxJava的文章，很全面的文章|
|[ReactiveX官方文档中文翻译版](ReactiveX)|ReactiveX官方文档，深入学习ReactiveX必看文章|

##	开发工具

|                  工具名称                  |                   推荐理由                   |
| :------------------------------------: | :--------------------------------------: |
|              [Shadowsocks](https://shadowsocks.com/)               | 翻墙界的"瑞士军刀"，极其推荐，在专业搜索上，百度和google真的不是一个级别的 |
| [Lantern(蓝灯)](https://getlantern.org/) |            有免费版，速度一般，对于一般搜索足够            |
| [Postman](https://www.getpostman.com/) |     极其推荐，绝对的API调试神器，我的Chrome上必装的一个插件     |
|    [Bejson](http://www.bejson.com/)    |              在线查看和生成Json实体               |
|[矢量图标库](http://www.iconfont.cn/plus)|阿里巴巴矢量图标库，种类很全，对于不会设计的工程师太有用了|

##  Android Studio常用插件
|常用插件|推荐理由|
|:-----:|:------:|
|[GsonFormat](https://plugins.jetbrains.com/plugin/7654)|根据Json一键生成对应的实体类，不用自己手动去书写大量的实体类，极力推荐|
|[Android Studio翻译插件](https://github.com/Skykai521/ECTranslation)|Android Studio内部翻译插件，对于查看Android源码很有帮助|
##	联系我

- Email：tonycheng93@outlook.com
- Github:https://github.com/tonycheng93/
- Blog:http://tonycheng93.github.io/
