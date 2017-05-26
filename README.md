![](http://ww1.sinaimg.cn/large/005Xtdi2jw1f6307cu3krj30rs05kglz.jpg)

### 作者博客： 
- [个人博客](http://imlerry.com)
- [简书](http://www.jianshu.com/u/3287e4c61439)
- [掘金](https://juejin.im/user/57fcfe58a3413100601c7be8)


### 作者微博： [Lerry](http://weibo.com/u/5904475839)

**借鉴了[GcsSloop](https://github.com/GcsSloop/AndroidNote)的笔记风格**

#### 这是我在编程成长道路上的学习笔记，记录学习和工作过程中所遇到的问题。 在笔记中会用我自己的原创文章， 同时也会收录许多我自己看过觉得有用的博客链接。

> 我为什么要创建自己的Note?
>
> 其一当然是为了记录自己所掌握的知识， 另外也是为了大家能够流程式的去掌握一个知识点， 举个例子， 如果我们要学自定义View， 那其中包括事件传递， view的绘制流程， 基本绘图类的学习，包括很多知识点， 而市面上能将整套流程按顺序整理的博客少之又少， 参差不一， 至今知道的最系统的也就[GcsSloop](https://github.com/GcsSloop/AndroidNote)的自定义View系列了， 本人也在拜读中。 为此， 我建立了这个笔记， 可以更加的把一个知识点以一个流程的形式列下来， 更系统的掌握。

## 申明 ：所有的知识点系列的顺序都是在本人阅读过后排出的，列出的博文都是值得阅读的，自认为是比较合适的学习顺序。如果文章标题后带有【原创】的均为本人原创。
## Content
- [Android](#android)
- [React-Native](#react-native)
- [算法与数据结构](#算法与数据结构)
- [读书笔记](#读书笔记)
- [面试](#面试)
- [博客推荐](#博客推荐)
- [开放API](#开放api)
- [开发者网站](#开发者网站)


## [Android](https://github.com/lllerry/Note/tree/master/Android/README.md)

### RxJava2.0

- 基础
	- [给初学者的RxJava2.0教程(一)](https://juejin.im/post/5848d96761ff4b0058c9d3dc)
	- [给初学者的RxJava2.0教程(二)](https://juejin.im/post/5848dd11b123db0066030123)
	- [给初学者的RxJava2.0教程(三)](https://juejin.im/post/5848dd3eac502e00691385c5)
	- [给初学者的RxJava2.0教程(四)](https://juejin.im/post/584a6dd9128fe100589bf29d)
	- [给初学者的RxJava2.0教程(五)](https://juejin.im/post/584f76f48e450a006ad12ebf)
	- [给初学者的RxJava2.0教程(六)](https://juejin.im/post/58510ec3ac502e0067cfa4a2)
	- [给初学者的RxJava2.0教程(七)](https://juejin.im/post/5857a5e48e450a006c752701)
	- [给初学者的RxJava2.0教程(八)](https://juejin.im/post/585b8f741b69e600560602d3)
	- [给初学者的RxJava2.0教程(九)](https://juejin.im/post/58807ef92f301e00697f6ad8)
	- 看完这九篇只能简单的知道如何在Android中应用RxJava2.

- MVP模式中包含RxJava
	- 待续

### 自定义View系列（包含事件传递， view的绘制流程，绘图类使用）

- 事件传递（又称事件分发机制）
	- [Android事件分发机制完全解析，带你从源码的角度彻底理解(上)](http://blog.csdn.net/guolin_blog/article/details/9097463)
	- [ Android事件分发机制完全解析，带你从源码的角度彻底理解(下)](http://blog.csdn.net/guolin_blog/article/details/9153747)
	- 阅读[Android开发艺术探索](https://book.douban.com/subject/26599538/)第三章， 掌握知识点。
	- 巩固：[图解 Android 事件分发机制](http://www.jianshu.com/p/e99b5e8bd67b)

- View的绘制流程
	- [setContentView（）的源码解析	**【原创】**](http://imlerry.com/2017/05/08/02.Android%E9%AB%98%E7%BA%A7UI%E7%B3%BB%E5%88%97%EF%BC%881%EF%BC%89-setContentView-%E8%AF%A6%E8%A7%A3/)（view是怎样加载到界面上的）可以跳过。
	- [Android LayoutInflater原理分析，带你一步步深入了解View(一)](http://blog.csdn.net/guolin_blog/article/details/12921889) 这篇是让你对setContentView有一个简单的认识 跳过上篇的同学这篇一定要看。
	- [Android视图绘制流程完全解析，带你一步步深入了解View(二)](http://blog.csdn.net/guolin_blog/article/details/16330267) 对measure,layout,draw的浅析。
	- 阅读[Android开发艺术探索](https://book.douban.com/subject/26599538/)第四章view的工作原理， 读一遍肯定是不够的。这篇读懂了就能搞懂view的绘制流程了， 不用看其他的博文了。
	- 拓展： [Android视图状态及重绘流程分析，带你一步步深入了解View(三)](http://blog.csdn.net/guolin_blog/article/details/17045157)这是一篇对view状态分析的博客。 个人认为读一读可以加深对view的认知。
	- [ Android自定义View的实现方法，带你一步步深入了解View(四)](http://blog.csdn.net/guolin_blog/article/details/17357967) 读这篇是对郭霖老师的信仰， 如果你读懂Android开发艺术探索的第四章的话， 应该已经自己练习过两个例子了， 这个例子应该能轻松读懂。

- 自定义View
	- 准备阅读的系列，我还没有阅读 是GcsSloop, 启舰的博客。
	- [安卓自定义View教程目录](http://www.gcssloop.com/customview/CustomViewIndex)
	- [Android自定义控件三部曲文章索引](http://blog.csdn.net/harvic880925/article/details/50995268)

### 网络请求第三方库

- Okhttp
	- 待续
- Retrofit
	- 待续

### RecyclerView

- 基础
	- 待续

### MVP

 - 待续

 
---

## React Native

### 系列教程
- 尽请期待

### 第三方APP
- 尽请期待

### 第三方库
- 尽请期待

---

## 算法与数据结构
- 基础
	- [数据抽象]() 
	- [栈和队列](https://github.com/lllerry/Note/tree/master/数据结构与算法/栈和队列.md)
	- [算法分析]()
- 排序
	- [初级排序算法](https://github.com/lllerry/Note/tree/master/数据结构与算法/初级排序算法.md)
	- 归并排序
	- 快速排序
	- 优先队列

---

## 读书笔记
- Android开发艺术探索
	- [chapter01 Activity的生命周期和启动模式]()
- 图解HTTP
	- [整数读书笔记](http://imlerry.com/2017/05/17/%E3%80%8A%E5%9B%BE%E8%A7%A3HTTP%E3%80%8B%E8%AF%BB%E4%B9%A6%E7%AC%94%E8%AE%B0/)
- 算法（第四版）
	- 详见[算法Node](#算法与数据结构)
- Thinking in Java
	- 略
	
---

## 面试
- Java相关
	- [ThreadLoacal是什么？说说你对它的理解](http://droidyue.com/blog/2016/03/13/learning-threadlocal-in-java/index.html)

- Android相关
	- 略

---

## 博客推荐

- Android
	- [Hongyang](http://blog.csdn.net/lmj623565791?viewmode=contents)
	- [郭霖](http://blog.csdn.net/guolin_blog)
	- [启舰](http://blog.csdn.net/harvic880925)
	- [工匠若水](http://blog.csdn.net/yanbober)
	- [徐宜生](http://blog.csdn.net/eclipsexys)
	- [GcsSloop](http://gcssloop.com/#blog)
	- [D_clock爱吃葱花](http://blog.coderclock.com/)
	- [张涛-开源实验室](https://www.kymjs.com/)
	- [Lucida](http://zh.lucida.me/)
	- [技术小黑屋](http://droidyue.com/)
	- [Trinea](http://www.trinea.cn/)

- 前端
	- [阮一峰的网络日志](http://www.ruanyifeng.com/blog/)
	
---

## 开放API
- [Dribbble](http://developer.dribbble.com/v1/)
- [gank.io](http://gank.io/api)
- [豆瓣API](https://developers.douban.com/wiki/?title=guide)
- [Last.fm](https://www.last.fm)

---

## 开发者网站

- [极客导航](http://www.jikedaohang.com/)
- [谷歌开发者](https://developers.google.cn/)
- [Android](https://www.android.com/)
- [Android Developers](https://developer.android.com/index.html)
- [Android开发技术周报](http://androidweekly.cn/)
- [ImportNew](http://www.importnew.com/)

---

#### 转载注意事项

除注明外，所有文章均采用 [Creative Commons BY-NC-ND 4.0（自由转载-保持署名-非商用-禁止演绎）](http://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh)协议发布。

你可以在非商业的前提下免费转载，但同时你必须：

* 保持文章原文，不作修改。
* 明确署名，即至少注明 `作者：Lerry` 字样以及文章的原始链接，且不得使用 `rel="nofollow"` 标记。
* 微信公众号转载一律不授权 `原创` 标志。


[▲ 回到顶部](#top)