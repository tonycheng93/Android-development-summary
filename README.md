#	Android	开发资料汇总

学习Android开发这一路走来，深知自学的不易。刚开始接触某一个新兴的技术，总是在网上漫无目的的搜索各种文章，而这些文章良莠不齐的，浪费了大量时间来辨别这些东西是否对自己有用。后来在github上面看到了许多优秀的开源项目，浏览器收藏夹也不知道到底收藏了多少，但是没有一个很好的分类。于是便萌生了一个想法，自己把学习过程中查阅的优秀文章和开源项目做一个整理。同时也会分享一些自己觉得能够提高工作效率的工具。希望这份资料能够给刚开始学习Android的开发者提供一点帮助，节约一些查找资料的时间。原始的markdowm文件已经放到github上，欢迎[下载和star](https://github.com/tonycheng93/Android-development-summary) 。这份资料我会不断的完善，也欢迎一些经验丰富的开发者可以一起来完善，直接[pull request](https://github.com/tonycheng93/Android-development-summary/pulls) 或者[issue](https://github.com/tonycheng93/Android-development-summary/issues)，我会定期筛选合并，有一些好的建议和意见随时[联系我](#联系我)，欢迎转载，谢谢收藏。
##	目录
-  [图片加载库](#图片加载库)

-  [网络请求库](#网络请求库)

-  [网络缓存](#网络缓存)

-  [博客推荐](#博客推荐)

-  [微信公众号推荐](#微信公众号推荐)

-  [开发工具](#开发工具)
-  [联系我](#联系我)

##	图片加载库

|                   图片库                    |    作者    |                   推荐理由                   |
| :--------------------------------------: | :------: | :--------------------------------------: |
| [Glide](https://github.com/bumptech/glide) | bumptech | 支持Gif，google官方推荐的图片加载库，在google的众多App中都采用了该库 |
| [Fresco](https://github.com/facebook/fresco) | Facebook | 支持Gif，Facebook出品，必属精品，Fresco另辟蹊径使用Native方法来管理图片，专注解决图片内存溢出问题 |
| [Picasso](https://github.com/square/picasso) |  Square  | 开源大户Square出品，和Glide用法极其相似，Glide体积更小，JakeWharton大神所在公司 |
| [Android-Universal-Image-Loader](https://github.com/nostra13/Android-Universal-Image-Loader) | nostra13 | 老牌图片加载库，在上述图片加载库没出来之前，使用最多的开源图片库。但是，该项目已被作者废弃不再维护，不建议使用，用来学习图片异步加载和图片管理还是极好的 |

##	网络请求库

|   网络库    |   作者   |                   推荐理由                   |
| :------: | :----: | :--------------------------------------: |
|  OkHttp  | Square | Google在6.0中删除了HttpClient API代码。取而代之的是OkHttp，已被google官方认可，值得信赖。[Android OkHttp完全解析 是时候来了解OkHttp了](http://blog.csdn.net/lmj623565791/article/details/47911083)；[拆轮子系列：拆OkHttp](http://blog.piasy.com/2016/07/11/Understand-OkHttp/) |
| Retrofit | Square | 基于OkHttp，Square出品。非常适用于ResetFul API格式网络请求，与RxJava结合有奇效。[Retrofit源码解析](http://blog.piasy.com/2016/06/25/Understand-Retrofit/)；[codeKK Retrofit源码解析](https://github.com/android-cn/android-open-project-analysis/tree/master/tool-lib/network/retrofit) |
|  Volley  | Google | Google官方出品，适用于数据量不大，但网络通信频繁的场景，不适用于大文件读取、上传场景。[Volley源码解析系列文章，郭神作品](http://blog.csdn.net/guolin_blog/article/details/17482095)；[codeKK Volley源码解析](http://www.codekk.com/blogs/detail/54cfab086c4761e5001b2542) |

##	网络缓存

|                   缓存库                    |     作者      |                   推荐理由                   |
| :--------------------------------------: | :---------: | :--------------------------------------: |
| [DiskLruCache](https://github.com/JakeWharton/DiskLruCache) | JakeWharton | JakeWharton大神的杰作，缓存神奇，值得信赖。源码解析和用法参考文章：[Android DiskLruCache完全解析，硬盘缓存的最佳方案](http://blog.csdn.net/guolin_blog/article/details/28863651)，[Android DiskLruCache源码解析 硬盘缓存的绝佳方案](http://blog.csdn.net/lmj623565791/article/details/47251585) |
| [ASimpleCache](https://github.com/yangfuhai/ASimpleCache) |     杨福海     | afinal框架作者，国内Android大神。它是一个为Android制定的轻量级的缓存框架，只有一个java文件。支持自定义缓存路径、大小、缓存超时时间等。[ASimpleCache源码分析](http://blog.csdn.net/zhoubin1992/article/details/46379055) |

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





##	开发工具

|                  工具名称                  |                   推荐理由                   |
| :------------------------------------: | :--------------------------------------: |
|              Shadowsocks               | 翻墙界的"瑞士军刀"，极其推荐，在专业搜索上，百度和google真的不是一个级别的 |
| [Lantern(蓝灯)](https://getlantern.org/) |            有免费版，速度一般，对于一般搜索足够            |
| [Postman](https://www.getpostman.com/) |     极其推荐，绝对的API调试神器，我的Chrome上必装的一个插件     |
|    [Bejson](http://www.bejson.com/)    |              在线查看和生成Json实体               |
|[矢量图标库](http://www.iconfont.cn/plus)|阿里巴巴矢量图标库，种类很全，对于不会设计的工程师太有用了|

##	联系我

- Email：tonycheng93@outlook.com
- Github:https://github.com/tonycheng93/
- Blog:http://tonycheng93.github.io/
