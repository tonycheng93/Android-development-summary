#	Android	开发资料汇总

收集这份资料的灵感来源于我的浏览器收藏夹快爆了，后来在github 上也看到了很优秀的开源库的收集资料，非常的好，但是太过于多，也不够新，所以决定自己来做一个。原始的markdowm文件已经放到github上，欢迎[下载和star](https://github.com/tonycheng93/Android-development-summary) 。这份资料我会不断的完善，也欢迎一些经验丰富的开发者可以一起来完善，直接[pull request](https://github.com/tonycheng93/Android-development-summary/pulls) 或者[issue](https://github.com/tonycheng93/Android-development-summary/issues)，我会定期筛选合并，有一些好的建议和意见随时[联系我](#联系我)，欢迎转载，谢谢收藏。
##	目录
-	[图片加载库](#图片加载库)
   -[网络请求库](#网络请求库)
   -[网络缓存](#网络缓存)
-	[联系我](#联系我)


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

##	联系我

- Email：tonycheng93@outlook.com
- Github:https://github.com/tonycheng93/
- Blog:http://tonycheng93.github.io/