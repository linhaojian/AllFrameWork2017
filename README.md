# AllFrameWork2017


1. Retrofit　　
一句话介绍：Retrofit是一款类型安全的网络框架，基于HTTP协议，服务于Android和java语言

上榜理由：Retrofit以21.8k的stars量雄踞github中android子标题榜首，第一当之无愧。

官网地址 http://square.github.io/retrofit/

github   https://github.com/square/retrofit

作者：square团队

使用：

compile 'com.squareup.retrofit2:retrofit:2.3.0'
 

2.okhttp
一句话介绍：okhttp是一款基于HTTP和HTTP2.0协议的网络框架，服务于java和android客户端

上榜理由，okhttp以20.4k的stars量雄踞github中android子标题第二名。大型公司比如淘宝也封装的是okhttp。Retrofit2.0开始内置okhttp框架，Retrofit专注封装接口完成业务需求，okhttp专注网络请求的安全高效，笔者将两者区分开，是想让后来学习者知道，这是两套框架，学习框架原理时可以分开学习，以免理解混乱。

官网地址   http://square.github.io/okhttp/

github    https://github.com/square/okhttp

作者：square团队

使用：

compile 'com.squareup.okhttp3:okhttp:3.8.0'
 

　　

3.Butter Knife
一句话介绍：Butter Knife所提供了一种能力——使用注解生成模板代码，将view与方法和参数绑定。

上榜理由：github上16.5K个star，配合Androidstudio提供的Butter Knife插件，帮助开发者省却了频繁findviewbyid的烦恼，最新的Butter Knife还提供了onclick绑定以及字符串的初始化，初学者可以查阅Butter Knife以及Butter Knife插件进一步学习！

官网地址：http://jakewharton.github.io/butterknife/

github：https://github.com/JakeWharton/butterknife

作者：JakeWharton ，也是square团队成员之一

使用：

dependencies {
  compile 'com.jakewharton:butterknife:8.6.0'
  annotationProcessor 'com.jakewharton:butterknife-compiler:8.6.0'
}
 

4.MPAndroidChart
一句话介绍：MPAndroidChart是一款图表框架

上榜理由：github上16.1K个star，以快速、简洁。强大著称的图表框架

官网地址 https://github.com/PhilJay/MPAndroidChart  

github  https://github.com/PhilJay/MPAndroidChart

作者：PhilJay

使用：

1. 在AS中加入Gradle依赖

在根目录的 build.gradle上加入:
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
 

　　

在app的build.gradle上加入：
dependencies {
    compile 'com.github.PhilJay:MPAndroidChart:v3.0.2'
}
 

　

5. glide
一句话介绍：glide是一款专注于提供流畅划动能力的“图片加载和缓存框架”

上榜理由：15.9k个star，图片加载类框架排名第一的框架，google 在2014开发者大会上演示的camera app就是基于gilde框架开发的

github https://github.com/bumptech/glide

作者 Bump Technologies团队

使用：

复制代码
repositories {
  mavenCentral()
}

dependencies {
    compile 'com.github.bumptech.glide:glide:3.8.0'
    compile 'com.android.support:support-v4:19.1.0'
}
复制代码
6.leakcanary
一句话介绍：一款内存检测框架，服务于java和android客户端

上榜理由：方便，简洁是leakcanary最大的特点，只需在应用的apllication中集成，就可以直接使用它；15.5k个star说明了它有多么受欢迎

github https://github.com/square/leakcanary

作者 square团队

使用：

 dependencies {
   debugCompile 'com.squareup.leakcanary:leakcanary-android:1.5.1'
   releaseCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1'
   testCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1'
 }
在 Application 中写入:

复制代码
public class ExampleApplication extends Application {

  @Override public void onCreate() {
    super.onCreate();
    if (LeakCanary.isInAnalyzerProcess(this)) {
      // This process is dedicated to LeakCanary for heap analysis.
      // You should not init your app in this process.
      return;
    }
    LeakCanary.install(this);
    // Normal app init code...
  }
}
复制代码
 

7.Android-Universal-Image-Loader
一句话介绍：曾经的图片加载框架王者，android开发老手都用过它

上榜理由:android端图片加载框架的老大哥了，15.3k个star足以证明它的热门，UIL与gilde最大区别是可定制，UIL提供了大量配置方式，图片加载状态的回调（成功，失败，进行中），加载动画等；以及提供了移动端图片加载框架的缓存思路：三级缓存策略 sd卡-内存-网络；值得注意的是，UIL以及两年未更新了，但笔者仍推荐各位使用！

github https://github.com/nostra13/Android-Universal-Image-Loader

作者 nostra13

使用：

下载地址  universal-image-loader-1.9.5.jar

 

 

8.EventBus 
一句话介绍：EventBus是一款本地组件间通信框架

上榜理由：组件间通信框架star量第一：14.8k，在大型项目的Activities，fragments，Threads，Services都可以看到它的使用场景，尽管EventBus在向未创建的组件传递事件时有些局限，仅适合在“活着的”组件间传递消息，但仍不妨碍它活跃在各个大型项目各个场景里。

官网地址 http://greenrobot.org/eventbus/documentation/how-to-get-started/

github  https://github.com/greenrobot/EventBus

作者 greenrobot 

使用：

compile 'org.greenrobot:eventbus:3.0.0'
 

9.zxing
一句话介绍：条码图像处理库

上榜理由：如果你用过二维码，你肯定已经间接使用过大名鼎鼎的zxing了。13.9K的star量，让它排在本榜单第九，实至名归，如果你有了解二维码的需求，不妨从了解、修改它源码入手。

github  https://github.com/zxing/zxing

作者  Sean Owen

 

10.picasso
一句话介绍：强力的图片下载、缓存框架

上榜理由：本榜单出现的第三款图片类框架，不同的是picasso更强调图片下载，你可以将picasso集成进你的项目中，你也可以结合gilde和UIL与picasso，三者一齐封装至你的项目中，按需所用。

官网地址 http://square.github.io/picasso/

github  https://github.com/square/picasso

作者 square团队

使用：

compile 'com.squareup.picasso:picasso:2.5.2'
或者下载

jar包

 

11.lottie-android
一句话介绍：一款可以在Android端快速展示Adobe Afeter Effect（AE）工具所作动画的框架

上榜理由：动画类框架第一名，github上13.3k个star证明了他的优越性，利用json文件快速实现动画效果是它最大的便利，而这个json文件也是由Adobe提供的After Effects（AE）工具制作的，在AE中装一个Bodymovin的插件，使用这个插件最终将动画效果生成json文件，这个json文件即可由LottieAnimationView解析并生成绚丽的动画效果。而且它还支持跨平台哟。

github  https://github.com/airbnb/lottie-android

作者：Airbnb 团队

 

12.fresco
一句话介绍：一款可以管理图片内存的框架

上榜理由:github上12.8k个star，图片类排行榜第四名，facebook的出身证明了它并非是重复造的轮子，在管理图片内存领域上有着它的一片天地，渐进式加载、加载gif都是它与前三位相比独有的特性

官网地址： https://www.fresco-cn.org/

github  https://github.com/facebook/fresco

作者 facebook

使用：

dependencies {
  // 其他依赖
  compile 'com.facebook.fresco:fresco:0.12.0'
}
下面的依赖需要根据需求添加：

复制代码
dependencies {
  // 在 API < 14 上的机器支持 WebP 时，需要添加
  compile 'com.facebook.fresco:animated-base-support:0.12.0'

  // 支持 GIF 动图，需要添加
  compile 'com.facebook.fresco:animated-gif:0.12.0'

  // 支持 WebP （静态图+动图），需要添加
  compile 'com.facebook.fresco:animated-webp:0.12.0'
  compile 'com.facebook.fresco:webpsupport:0.12.0'

  // 仅支持 WebP 静态图，需要添加
  compile 'com.facebook.fresco:webpsupport:0.12.0'
}
复制代码
 

13.RxAndroid
一句话介绍：一款Android客户端组件间异步通信的框架

上榜理由：github上12.7k个star，位居组件通信框架的第二名，仅在EventBus之后，如果要问两者的区别，Eventbus是用来取代组件间繁琐的interface，RxAndroid是用来取代AnsyTask的，并不冲突；当然RxAndroid的优点并不仅限于此，更多优雅的实现，可以去官网查阅！

github  https://github.com/ReactiveX/RxAndroid

作者 JakeWharton

使用：

compile 'io.reactivex.rxjava2:rxandroid:2.0.1'
compile 'io.reactivex.rxjava2:rxjava:2.1.0'
 

14.SlidingMenu
一句话介绍：侧滑菜单栏框架

上榜理由：与Userval-Image-loader 齐名的上古神器框架——为你的app提供侧滑菜单栏的功能；github闪更有10.5k个star，证明了它的经久不衰，即使在Google推出了NavigationDrawer，仍然没有减少开发者对SildingMenu的拥簇，经典总是经得起考验的，这个上古神兽已经四年没有更新了；有太多太多的app使用过它，这些都可以在软件的开源许可上看到！

github https://github.com/jfeinstein10/SlidingMenu

作者 Jeremy Feinstein

使用：

在gihub上fork源码，集成进项目中

 

15.PhotoView
一句话介绍：一款ImageView展示框架，支持缩放，响应手势

上榜理由：10.3k的star数量，位于图片类框架排行榜第五位，PhotoView与前四位不同的是这次带来的是图片的展示能力，你一定好奇微信的头像点击放大是如何实现的，很多App的图片显示响应手势按压是如何实现的，了解PhotoView，你一定会开心的！（笔者也不会告诉你ImageView的点击放大效果在Android的sample也有）

github  https://github.com/chrisbanes/PhotoView

作者：chrisbanes

使用：

复制代码
在app根目录的build.gradle中加入：
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
在app的module目录的build.gralde中加入：

dependencies {
    compile 'com.github.chrisbanes:PhotoView:latest.release.here'
}
复制代码
使用

复制代码
<com.github.chrisbanes.photoview.PhotoView
    android:id="@+id/photo_view"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>


PhotoView photoView = (PhotoView) findViewById(R.id.photo_view);
photoView.setImageResource(R.drawable.image);
复制代码
 

16.material-dialogs
一句话介绍：一款自定义dialog框架

上榜理由：9.9k个star，也是继PhotoView，SlidingMenu之后第三款自定义View框架，也许你还是自定义View的新人，对Dialog使用的还有点生疏，你可以通过它提升你的Dilaog使用能力

github  https://github.com/afollestad/material-dialogs

作者：Aidan Follestad

使用：

dependencies {
    // ... other dependencies here
    compile 'com.afollestad.material-dialogs:core:0.9.4.5'
}
 

17.droid-async-http
 一句话介绍：一款基于Http协议的异步请求的网络框架，

上榜理由：虽然你有无数个使用retrofit+okhttp的理由，但9.8k个star，证明它仍然值得你深入学习。值得注意的是，它也已经有两年没更新了，你尽管拿去当你懒惰的理由！

github   https://github.com/loopj/android-async-http

作者：James Smith

使用：

复制代码
repositories {
  maven {
    url 'https://oss.sonatype.org/content/repositories/snapshots/'
  }
}
dependencies {
  compile 'com.loopj.android:android-async-http:1.5.0-SNAPSHOT'
}
复制代码
 

18.androidannotations
一句话介绍：一款基于注解的快速开发框架

上榜理由：与Butterknife一样基于注解，利用注解快速完成view的初始化，不同的是androidannotations提供了更多的能力：简单的线程模型等；笔者只接触过Butterknife，无法更进一步叙述androidannotations的优势，如果你志在深入了解注解的妙用，可以尝试探索一下！

官网地址 http://androidannotations.org/

github https://github.com/androidannotations/androidannotations

作者： WonderCsabo

 

19.fastjson
一句话介绍:一款基于json解析、生成的框架

上榜理由：从它的名字不难看出，快速是它最大的特性，阿里巴巴的出身保证了代码的质量和优越，9.4k的star数量，也是榜单里第一个出现的中国开源框架，涉及网络的app都会用到json，fastjson值得作为你的首选！

github  https://github.com/alibaba/fastjson

作者：alibaba

使用：

compile 'com.alibaba:fastjson:1.1.58.android'
 

20.Material-Animations
一句话介绍：一款提供场景转换过渡能力的动画框架

上榜理由：Android动画框架排行榜第二名，9.3k个star数量，与动画框架榜单第一名lottie-android不同的是，Material-Animations提供的是场景切换的动画效果。Android 官网sample中已经提供了部分Transition （转场动画）的展示，作为初学者很难快速拓展到自己项目中，Material-Animations的示例出现为开发者省去了此类麻烦，直接照搬应用到自己的App中吧。

 github  https://github.com/lgvalle/Material-Animations

作者：Luis G. Valle

使用：

down源码，修改学习

 

21.tinker
一句话介绍：它是微信官网的Android热补丁解决方案

上榜理由：9.1k个star，微信在用的热补丁方案，心动不如行动

官网地址  http://www.tinkerpatch.com/Docs/intro

github   https://github.com/Tencent/tinker

作者：Tencent

 

 

22.ViewPagerIndicator
一句话介绍：一款基于ViewPager的页面指示器开源框架

上榜理由：上古神器，尽管已经五年未更新了，但你仍然可以在淘宝等app中看到它的使用场景，8.9K的star量让它不愠不火的在矗立在榜单里

官网地址 http://viewpagerindicator.com/

github  https://github.com/JakeWharton/ViewPagerIndicator

作者：JakeWharton 

使用：

 下载 地址 https://github.com/JakeWharton/Android-ViewPagerIndicator/zipball/master

 

23.Android-CleanArchitecture
一句话介绍：一个讲解设计框架的demo

上榜理由：它不是框架，你可以把它当作一本书，它将教会你如何设计简洁的架构，工程里有一个sample app，配合图文讲解，你将对Android客户端的架构有更深一层的认识。8.8k的star数量，证明了它是一本“好书”哟。

github  https://github.com/android10/Android-CleanArchitecture

作者：Fernando Cejas

 

24..Android-PullToRefresh
一句话介绍：一款为普通视图提供刷新UI的视图框架

上榜理由：8.2K的star数量使它位居刷新类UI框架榜首，强大的兼容能力，该框架支持ListView，GrdiView，WebViewScrollView，ViewPager等众多View增加刷新的能力，如果你有增加上拉加载，下拉加载的需求，你应该考虑它了！

github https://github.com/chrisbanes/Android-PullToRefresh

作者：Chris Banes

使用：

github fork源码，集成到项目中

 

25.flexbox-layout
一句话介绍：一款弹性伸缩布局

上榜理由：8.1k个star，前端H5开发者转Android开发的福音，FlexboxLayout作为LinearLayout和RelativeLayout的替代者，值得各位一试，与其一同推出的还有ConstraintLayout。

github  https://github.com/google/flexbox-layout

作者：Google

使用：

dependencies {
    compile 'com.google.android:flexbox:0.3.0-alpha3'
}
 

26.AndroidSwipeLayout
一句话介绍：非常强大滑动式布局

上榜理由:滑动删除是国产app常见需求，商品详情的上下滑动需求作为开发者的我们也经常遇到，AndroidSwipeLayout在github上拥有8K个star，证明它经受住了检验，各位值得一试

github https://github.com/daimajia/AndroidSwipeLayout

作者：daimajia

使用：

dependencies {
    compile 'com.android.support:recyclerview-v7:21.0.0'
    compile 'com.android.support:support-v4:20.+'
    compile "com.daimajia.swipelayout:library:1.2.0@aar"
}
或下载 

AndroidSwipeLayout-v1.1.8.jar

 

27.realm-java
一句话介绍：Realm是一款移动端数据库框架

上榜理由：核心数据引擎C++打造，比普通的Sqlite型数据库快的多。笔者猜测正是如此，realm以7892个star数让它位于大名鼎鼎的数据库框架GreenDao（7877）之前

官网地址：https://realm.io/cn/

github https://github.com/realm/realm-java

作者：Realm团队 

使用：https://realm.io/docs/java/latest/

 

28.greenDAO
一句话介绍：greenDAO是一款高效、快速的SQLite型数据库

上榜理由：greenDAO的star数量与Realm不相上下，且与EventBus师出同门，也是由greenrobot团队开发维护的，质量有所保证，但若拷问笔者Realm与greenDao两者的优劣性，只能具体到实际使用当中，模拟线上的使用情形，进行高强度测试后才能下判断，故在此不能一言两语说完，深表遗憾

官网地址：http://greenrobot.org/greendao/

github  https://github.com/greenrobot/greenDAO

使用：

复制代码
buildscript {
    repositories {
        jcenter()
        mavenCentral() // add repository
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:2.3.1'
        classpath 'org.greenrobot:greendao-gradle-plugin:3.2.2' // add plugin
    }
}
 
-----

apply plugin: 'com.android.application'
apply plugin: 'org.greenrobot.greendao' // apply plugin
 
dependencies {
    compile 'org.greenrobot:greendao:3.2.2' // add library
}
复制代码
 

29.stetho
一句话介绍：一款提供在Chrome开发者工具上调试Android app能力的开源框架

上榜理由：上古时期Android程序员要调试本地数据库，需要进入Android Device Monitor找到/data/data/com.xxx.xxx/databases里面的db文件，导出到PC端，用PC的数据工具查看，现在使用stetho省却了如此的麻烦；如今的Android程序员如果想调试网络请求响应过程中的报文段，需要在请求中加入Log语句，一个信息一个信息打印出来，相当繁琐，现在请使用stetho，省却诸如此类的麻烦把！7.8K个star数，广大Android开发者调试的福音，你值得拥有！

作者：FaceBook

官网地址： http://facebook.github.io/stetho/

github   https://github.com/facebook/stetho

使用：

compile 'com.facebook.stetho:stetho:1.5.0'
 

30.BaseRecyclerViewAdapterHelper
一句话介绍：强大、流畅的Recyvlerview通用适配器

上榜理由：如果你是RecyclerView的拥簇者，你一定要体验这款专门服务该view的适配器，7.7K个star，让这个家伙位于github上Android 适配器排行榜第一，还有很多惊喜等你去探寻！

官网地址：http://www.recyclerview.org/

作者：陈宇明以及他的小伙伴

使用：

复制代码
allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}


dependencies {
        compile 'com.github.CymChad:BaseRecyclerViewAdapterHelper:VERSION_CODE'
}
复制代码
 

31.AndroidViewAnimations
一句话介绍：一款提供可爱动画集合的框架

上榜理由：正如作者所说，它囊括了开发需求过程中所有的动画效果，集成进了这个简洁可爱的动画框架。7.6K的star数，证明了它在动画框架领域的战斗力，让它仅仅位列lottie-android和Material-Animations两个动画框架霸主之后，屈居第三名

github https://github.com/daimajia/AndroidViewAnimations

作者：daimajia

使用：

dependencies {
        compile 'com.android.support:support-compat:25.1.1'
        compile 'com.daimajia.easing:library:2.0@aar'
        compile 'com.daimajia.androidanimations:library:2.2@aar'
}
sample：

YoYo.with(Techniques.Tada)
    .duration(700)
    .repeat(5)
    .playOn(findViewById(R.id.edit_area));
 

32. MaterialDrawer
一句话介绍：强大的塑料风格的抽屉框架

上榜理由：7.6K的star数量，作者的持续更新状态，如果你还在犹豫上手SlidingMenu遇到bug没人管的困境，那么你可以入手它作为你的抽屉布局 

github  https://github.com/mikepenz/MaterialDrawer

作者：Mike Penz

使用:

compile('com.mikepenz:materialdrawer:5.9.2@aar') {
    transitive = true
}
 

new DrawerBuilder().withActivity(this).build();
 

 

 33.Android-ObservableScrollView
一句话介绍：一款让视图滑动更具有视觉效果的滑动式框架

上榜理由：7.5K的star数量，证明了它曾经的价值，github上提供了12种滑动效果，你可以用它弥补其他框架的不足，提升你的App体验！

github https://github.com/ksoichiro/Android-ObservableScrollView

作者：Soichiro Kashima

使用：

compile com.github.ksoichiro:android-observablescrollview
 

34.CircleImageView
一句话介绍：圆角ImageView

上榜理由：也许你已经听说过无数种展示圆角图片的方法，但如果你不尝试尝试CircleImageView，那么你的知识库会因为少了它黯然失色，有的时候完成需求是开发者优先考虑的，不同实现方法牵扯到的性能差异更值得让人深思，如果你有心在图片性能上有所涉猎，那么CircleImageView绝对不会让你败兴而归。最后别忘了记得去看Romain Guy的建议哟。

github https://github.com/hdodenhof/CircleImageView

作者：Henning Dodenhof

使用：

dependencies {
    ...
    compile 'de.hdodenhof:circleimageview:2.1.0'
}
 

复制代码
<de.hdodenhof.circleimageview.CircleImageView
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/profile_image"
    android:layout_width="96dp"
    android:layout_height="96dp"
    android:src="@drawable/profile"
    app:civ_border_width="2dp"
    app:civ_border_color="#FF000000"/>
复制代码
 

35.logger
一句话介绍：一款让log日志优雅显示的框架

上榜理由：logger作为调试框架，并未给出很强大的能力，它最大的亮点是优雅的输出log信息，并且支持多种格式：线程、Json、Xml、List、Map等，如果你整日沉迷于汪洋大海般的log信息不能自拔，logger就是你的指路明灯！6.6k个star让他位列调试框架第二名，屈居facebook的stetho之后

github https://github.com/orhanobut/logger

作者：Orhan Obut

使用：

compile 'com.orhanobut:logger:2.1.1'
 

Logger.d(MAP);
Logger.d(SET);
Logger.d(LIST);
Logger.d(ARRAY);
Logger.json(JSON_CONTENT);
Logger.xml(XML_CONTENT);
 

36.agera
一句话介绍:一款服务于Android平台的响应式编程框架

上榜理由：google专门推出一套响应式编程框架服务于Android开发者，相比于之响应式编程框架榜首的 RxJava RxAndroid，它更轻量，两者最大的不同点在于agera基于push event、pull data （VS Rx系列 push data）。

github https://github.com/google/agera

作者：Google

使用：

  compile 'com.google.android.agera:agera:1.3.0'
扩展能力

  compile 'com.google.android.agera:content:1.3.0'
  compile 'com.google.android.agera:database:1.3.0'
  compile 'com.google.android.agera:net:1.3.0'
  compile 'com.google.android.agera:rvadapter:1.3.0'
  compile 'com.google.android.agera:rvdatabinding:1.3.0'
 

37.BottmBar
一句话介绍：一款底部导航栏视图框架

上榜理由：底部栏里的王者框架，6.3K的star数量，证明了它的优秀，完全遵循材料设计规范，上手非常方便。如果说缺点，无法设置icon与titile的间距，无法自定义视图的大小等，但这些都可以通过修改源代码解决，笔者献丑也修改了一套符合国内开发者的底部导航框架，即将开源。

github  https://github.com/roughike/BottomBar

作者：Iiro Krankka

使用：

compile 'com.roughike:bottom-bar:2.3.1'
 

38.Calligraphy
一句话介绍：一款自定义字体框架

上榜理由：如果你还在为一键修改App内所有字体样式而烦恼，6.3K个star的Calligraphy就值得你拥有，它可以同时修改整个整个项目的Textview字体，也可以单独 设置某个Textview的字体，还在等什么，快来试试吧！

github  https://github.com/chrisjenx/Calligraphy

作者：Christopher Jenkins

使用：

dependencies {
    compile 'uk.co.chrisjenx:calligraphy:2.3.0'
}
 

39.AndroidSlidingUpPanel
一句话介绍：可拖动的滑动面板视图框架

上榜理由：如果你的项目需要一个可拖拽的滑动式面板（展示某些详情信息，播放音乐，地图信息等），那么推荐你使用它，6.3k个star，来自创业公司umano的作品，证明它是用心推出的杰作

github https://github.com/umano/AndroidSlidingUpPanel

作者：umano

使用：

复制代码
dependencies {
    repositories {
        mavenCentral()
    }

    compile 'com.sothree.slidinguppanel:library:3.3.1'
}
复制代码
 

40.AppIntro
一句话介绍：一款提供快速制作欢迎页的框架

上榜理由：笔者从未把打算把欢迎页框架纳入排行榜当中，作为国内开发者，ViewPager开发App的欢迎页已经是手到擒来的需求，为何一个开源的欢迎页框架会在github上拥有6.3k个star？也许你会不屑一顾，是的，往往就在不屑一顾的瞬间，机遇就悄悄溜走了。

github https://github.com/apl-devs/AppIntro

作者：Paolo Rotolo

复制代码
    allprojects {
        repositories {
            ...
            maven { url 'https://jitpack.io' }
        }
    }

    dependencies {
            compile 'com.github.apl-devs:appintro:v4.2.0'
    }
复制代码
 

41.recyclerview-animators
一句话介绍：一款为Recyclerview提供扩展动画能力的框架

上榜理由：有一句老话：如果有天你失去对新事物的兴趣，那就说明你老了。recyclerview已经推出快三年了，还在用listview的人们，是否已经发掘自己渐渐变老；不要灰心，快为你的项目加入recyclerview-animators框架吧，为“自己”加入新鲜的血液和能量！（笔者备注：6.2K个star）

github  https://github.com/wasabeef/recyclerview-animators

作者；https://github.com/wasabeef

使用：

dependencies {
  // jCenter
  compile 'jp.wasabeef:recyclerview-animators:2.2.6'
}
 

42.dagger
一句话介绍：一款通过依赖注入降低程序间耦合的开发框架

上榜理由：github 上dagger1版本 有6.2k个star ， dagger2版本有7.3k个；由square完成的dagger1版本，到如今google团队接手的dagger2版本，强力开发团队保证了代码在设计上的优越性；如果你想探究Android 领域的设计模式，这也是不错的选择。

官网地址：https://google.github.io/dagger/

github ：https://github.com/google/dagger

作者：google

使用：

复制代码
dependencies {
  compile 'com.google.dagger:dagger:2.x'
  annotationProcessor 'com.google.dagger:dagger-compiler:2.x'
}
If you're using classes in dagger.android you'll also want to include:

compile 'com.google.dagger:dagger-android:2.x'
compile 'com.google.dagger:dagger-android-support:2.x' 
annotationProcessor 'com.google.dagger:dagger-android-processor:2.x'
复制代码
 

43.Android-Bootstarp
一句话介绍：一款提供在Android应用上实现Bootstrap（web框架）所作出效果的框架

上榜理由：榜单上第二款响应web技术的Android 端框架，还记得第一名是谁吗——flexbox-layout，作为Android开发者，你有必要去了解Web技术了。5.9k个star，证明它不容小觑

github https://github.com/Bearded-Hen/Android-Bootstrap

作者:Bearded-Hen团队

使用：

dependencies {
   compile 'com.beardedhen:androidbootstrap:{X.X.X}'
}
 

44.RxBinding
一句话介绍：一款提供UI组件事件响应能力的框架

上榜理由：如果你还未开始RxAndroid 之旅，RxBinding可以作为你的第一站，通过RXBinding，你将理解响应式编程的快乐，让项目里的事件流程更清晰。5.6K个star，RxAndroid作者亲自操刀，快来试用吧！

github  https://github.com/JakeWharton/RxBinding

作者：JakeWharton

复制代码
Platform bindings:

compile 'com.jakewharton.rxbinding2:rxbinding:2.0.0'
'support-v4' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-support-v4:2.0.0'
'appcompat-v7' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-appcompat-v7:2.0.0'
'design' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-design:2.0.0'
'recyclerview-v7' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-recyclerview-v7:2.0.0'
'leanback-v17' library bindings:

compile 'com.jakewharton.rxbinding2:rxbinding-leanback-v17:2.0.0'
复制代码
 

45.ListViewAnimations
一句话介绍：一款为ListView提供动展示画效果能力的框架

上榜理由：如果有一天我承认自己老了，我还会排排我的兄弟——ListView，证明我和它一起战斗过。ListViewAnimations的存在就是证明我们这些“老年人”仍有用武之地，也许你有说不出口的难处，无法体会到RecyclerView里动画的快乐，拥有ListViewAnimations，你一样可以骄傲的说，我的孩子（每个item）也有自己的动效啦。（笔者备注 5.6K个star）

github  https://github.com/nhaarman/ListViewAnimations

作者：nhaarman

使用：

复制代码
repositories {
    mavenCentral()
}

dependencies {
    compile 'com.nhaarman.listviewanimations:lib-core:3.1.0@aar'
    compile 'com.nhaarman.listviewanimations:lib-manipulation:3.1.0@aar'
    compile 'com.nhaarman.listviewanimations:lib-core-slh:3.1.0@aar'
}
复制代码
 

46.UItimateRecyclerView
一句话介绍：一款提供刷新、加载更多、动画特效等额外能力的RecyclerView框架

上榜理由：榜单上第三次出现RecyclerView的身影，足以证明RecyclerView的优异性，5.5K个star，框架里所提供众多的能力，如果你是个功利开发者，那么此框架会为你节省很多学习时间，它可以完成多item式布局的大多数需求，值得注意的是，这个项目也是在其他项目的思路上二次开发的。

github  https://github.com/cymcsg/UltimateRecyclerView

作者：MarshalChen

使用：

复制代码
repositories {
    jcenter()
    }
dependencies {
    ...
    compile 'com.marshalchen.ultimaterecyclerview:library:0.7.2'
}
复制代码
 

47.uCrop
一句话介绍：一款优雅的图片裁剪框架

上榜理由：5.3K个star，图片编辑模块单独拎出来也是一款优雅的App。

github  https://github.com/Yalantis/uCrop

作者：Yalantis

使用：

复制代码
allprojects {
   repositories {
      jcenter()
      maven { url "https://jitpack.io" }
   }
}

compile 'com.github.yalantis:ucrop:2.2.1' 
复制代码
 

48.RxJava-Android-Samples
一句话介绍：一款介绍RxJava使用场景的app

上榜理由：榜单出现的第一个“仅仅为告诉你如何使用另一个项目”的开源项目，它可以说是RxJava的用例，你想得到的想不到的RxJava用法这里都有，这就是为什么它以5.2k个star矗立在这份榜单里的原因。遗憾自己没有创作这么一个受人追捧的demo？赶快动手写个其他的“XX项目用例吧”

github  https://github.com/kaushikgopal/RxJava-Android-Samples

作者：kaushikgopal

使用：

clone到本地慢慢探索吧

 

49.AndroidAutoLayout
一句话介绍：一个提供适配能力的框架

上榜理由：5.2K个star，鸿洋老弟的作品，适合小项目的开发团队，拿到设计MM的px像素设计稿是不是很头疼捏？这个框架一键式搞定你的问题，它有很多的不足，但在追求完美适配的路上，你值得探索和了解它！笔者并不推荐把它应用到已经成熟运行的项目中，毕竟市面上已经有太多的适配解决方案了，适配问题就像是个大杂烩，想炒一盘好菜，就得备好各种佐料（适配小方案），当你把各种小佐料用的炉火纯青的时候，你离美食大厨就不远了。

github https://github.com/hongyangAndroid/AndroidAutoLayout

作者：张鸿洋

使用：

dependencies {
    compile 'com.zhy:autolayout:1.4.5'
}
 

50.EffectiveAndroidUI
一句话介绍：一款讲解高效展示UI的教学型App

上榜理由：编程新手很难对MVC MVP,MVVM等模式有深刻的理解，如果有一个示例型app，那对初学者会有很大裨益，笔者在遇到它时也是相见恨晚。4.8K个star，证明了它经受了广大开发者的考验与审视，其中Effective UI的编程思想更是与Android官方课程里的Effective UI课程不谋而合，并且，此项目还包含了fragment、dagger、主题样式、Butterknife等众多小知识点，作为编程初学者的学习用例再适合不过了

github  https://github.com/pedrovgs/EffectiveAndroidUI

作者：Pedro Vicente 

使用：

clone项目到本地

 

51.Luban
一句话介绍：最接近微信的图片压缩框架

上榜理由：好的思路总是可以让你大放异彩，Luban仅以图片压缩单一功能，俘获了4.8K个star，证明了它在图片压缩上的造诣，它可能不是最优秀的，但它是让你我最接近伟大的项目

github  https://github.com/Curzibn/Luban

作者：Curzibn

使用：

compile 'top.zibin:Luban:1.1.1'
 
52.DroidPlugin
一句话介绍：一款热门的插件化开发框架
上榜理由：4.8K个star，插件化框架榜单第一名，，360团队出品，框架质量有保证，有成功案例——360手机助手，并且持续维护着
github https://github.com/DroidPluginTeam/DroidPlugin/blob/master/readme_cn.md
作者：Andy Zhang
使用:
clone项目到本地
 
53. otto
一句话介绍:一款老旧且强大的事件总线框架
上榜理由：4.8K个star，是square团队早先推出的事件响应型框架，淘宝app的事件驱动也是基于此框架封装的，如今square已经建议开发者采用RxJava RxAndroid来代替otto了。但otto仍有与EventBus横向对比的价值，纵向来说，otto与square自家开发的Rx系列框架的差异同样值得开发者们去探究。
github https://github.com/square/otto
作者：square
使用：
repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }
}

compile 'com.michaelpardo:activeandroid:3.1.0-SNAPSHOT'
 

 
54.u2020
一句话介绍：一款提供Dagger的高级教学示例的app（额，名字是有点绕）
上榜理由：4.7K个star，JakeWharton牵头开发的教学类app，教你使用Dagger在其他高级框架的用法，它展示了Dagger与ButterKnife、Retrofit、Moshi、Picasso、Okhttp、RxJava、Timber、Madge、LeakCanar等众多优秀框架结合起来的高级用法，你也可以借鉴到自己的项目当中
github  https://github.com/JakeWharton/u2020
作者：JakeWharton
 
 
55.buck
一句话介绍：buck是一个快速构建系统
上榜理由：facebook+google出身的作者，对构建代码的出色理解，加上大型团队的维护，以及增量更新时的快速高效，让buck成为了微信Android团队构建项目的首选，构建大型项目时，它比gradle更快，然而中小公司并不适合此框架，但作为立志在框架设计领域有一番作为的人们，欢迎来一探究竟
官网地址：https://buckbuild.com/
github  https://github.com/facebook/buck
作者：facebook
使用：
linux or mac system  +docs
 

 
56.PermissionsDispatcher
一句话介绍：一款基于注解的提供解决运行时危险权限方案的框架
上榜理由：自Android6.0 Google提出危险权限一词起，用户安全性被提到一定的高度，一些运行时对用户较为危险的权限将不再自动被开发者获取，需要经过用户批准，开发者才可以继续使用该权限，如果你曾经被权限问题搞的抓耳挠腮，建议你试试这个框架，它足够解决你的问题
官网地址：https://hotchemi.github.io/PermissionsDispatcher/
github https://github.com/hotchemi/PermissionsDispatcher
作者：Shintaro Katafuchi
使用：
复制代码
dependencies {
  compile('com.github.hotchemi:permissionsdispatcher:${latest.version}') {
      exclude module: "support-v13"
  }
  annotationProcessor 'com.github.hotchemi:permissionsdispatcher-processor:${latest.version}'
}


repositories {
  jcenter()
  maven { url 'http://oss.jfrog.org/artifactory/oss-snapshot-local/' }
}
复制代码
 

57.android-gif-drawable
一句话介绍:一款提供展示GIF动画能力的视图框架

上榜理由：据我所查国内著名App——知乎使用了android-gif-drawable，因此证明了它的存在价值，尽管在榜单第十一位介绍了lottie-android直接应用AE动画的示例，但AE设计师不是每个公司都配备的，GIF的存在，就必然存在了展示GIF的需要，它值得你拥有！

github https://github.com/koral--/android-gif-drawable

作者：Karol Wrótniak

使用：

复制代码
repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
}
dependencies {
    compile 'pl.droidsonroids.gif:android-gif-drawable:1.2.+'
}
复制代码
 

58.Apktool
一句话介绍：一款反编译apk的工具

上榜理由：开源的反编译工具，对于志在了解apk逆向破解的诸位，值得拥有，4.5k个star，逆向破解apk神器！

github  https://github.com/iBotPeaches/Apktool

官网地址：https://ibotpeaches.github.io/Apktool/

作者：Connor Tumbleson

 

59.dynamic-load-apk
一句话介绍：插件化开发框架

上榜理由：4.5k个star，位于插件化开发框架第二名（第一名来自360团队），全面的文档介绍让你很快就能上手插件化开发，如果你喜欢大段文字讲解，那么这个项目一定适合你

github：https://github.com/singwhatiwanna/dynamic-load-apk

作者：singwhatiwanna

使用：

github上的文档配合作者博客更配哟

 

60.atlas
一句话介绍：淘宝推出的组件化开发框架

上榜理由：淘宝团队所出的精品，atlas框架提供了解耦、组件、动态的开发能力，4.5k个star让他位列组件化开发框架第一名

github https://github.com/alibaba/atlas

作者：alibaba

 

 61.volley
一句话介绍：google推荐使用的Android端网络请求框架

上榜理由：4.4k个star，并不是他不够优秀，而是使用volley已经渐渐成为广大开发者的习惯

github https://github.com/google/volley（新版volley地址）

作者：google

使用：

clone源码到本地

 
62.androidmvp
一句话介绍：一款展示Android端Mvp设计的demo
上榜理由：榜单里为数不多、仅凭展示某种设计模式就获得4.2K个star的项目，如果你有尝试mvp的打算，androidmvp可以作为你的前哨站
github  https://github.com/antoniolg/androidmvp
作者：Antonio Leiva
使用：
clone到本地
 
63.SwipeBackLayout
一句话介绍:一款可以让你通过滑动手势关闭页面的的框架
上榜理由：仿微信滑动退出当前聊天界面的效果，提供了activity的滑动关闭能力，通过这种思路，实现fragment的滑动关闭轻而易举;笔者坚持建议诸位clone源码到本地探索一番；4.2k个star证明很多人都喜爱它
github https://github.com/ikew0ng/SwipeBackLayout
作者：ike_w0ng
 使用:
compile 'me.imid.swipebacklayout.lib:library:1.0.0'
 

64.FlycoTabLayout
一句话介绍：一款可以让作出多种多样指示器效果的框架

上榜理由：尽管我们没有理由为了给app加入页面指示器功能就集成2.5M的依赖库，但是作为了解viewpager或swip views的指示器设计原理的优秀框架，你值得打开它试试，笔者建议单独拆分所需源码，加入到自己的项目中去。4.1K个star，二次开发的作品，仍然推荐！

github  https://github.com/H07000223/FlycoTabLayout

作者：Flyco

 

65.android-testing
一句话介绍：一款展示四大自动化测试框架用例的demo（Espresso，UiAutomator，AndroidJunitRunner，JUnit4）

上榜理由：学习者经常会陷入似懂非懂的境地，如果你有幸学习过Android Testing Support Library site的课程，那么你一定对android的四大测试框架迫不及待，这款demo非常适合你，快来学习这个4.1k个star的明星项目吧

github https://github.com/googlesamples/android-testing

作者：googlesampes团队

 

66.FileDownloader
一句话介绍：一款高效、稳定、灵活、易用的文件下载引擎

上榜理由：4.1k证明了它有多受人喜爱，文件下载看似简单的背后暗藏了多少的坑坑点点，我知道你有能力自己实现文件下载功能，但优秀的框架可以提升你的设计编码能力，这款框架可以提升你的实力！

github https://github.com/lingochamp/FileDownloader

作者:LingoChamp团队

使用：

dependencies {
    compile 'com.liulishuo.filedownloader:library:1.5.5'
}
 

 67.JieCaoVideoPlayer
一句话介绍：基于MediaPlayer api——VideoView 的多媒体播放框架

上榜理由：榜单里第三款多媒体播放框架，它以灵巧的身姿挤入本榜单，精巧是它最大的优点，不到100k，拥有它，你就可以快速开发类似今日头条那样的视频播放效果，4k个star，证明它值得一试

github https://github.com/lipangit/JieCaoVideoPlayer

作者：Nathen

使用：
compile 'fm.jiecao:jiecaovideoplayer:5.5.4'
 

68.glide-transformations
一句话介绍：为众多著名图片加载框架提供图片形状变幻能力的框架

上榜理由：在榜单靠前的部分已经介绍过glide，Picasso，Fresco等图片加载框架，glide-transformations就是一款为他们提供图片变形能力的框架，使用起来非常简单，因此受到了大家的喜爱，github上有3.8K个star
github  https://github.com/wasabeef/glide-transformations
作者：Daichi Furiya
使用：
复制代码
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:glide-transformations:2.0.2'
    // If you want to use the GPU Filters
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1'
}
复制代码
在Glide里设置变幻效果

Set Glide Transform.

Glide.with(this).load(R.drawable.demo)
        .bitmapTransform(new BlurTransformation(context))
        .into((ImageView) findViewById(R.id.image));
 

69.android-gpuimage
一句话介绍：一款基于OpenGL的图片渲染引擎
上榜理由：放下GpuImage在IOS平台的荣誉不谈，Android版的android-gpuimage就提供多达70多种图片渲染效果，你还在好奇美图秀秀是如何实现图片变幻的？有了它，一切都不是问题。如果你是美图工具类的工程师，此框架的建设思路也会对你大有裨益。笔者也是通过android-gpuimage仿造了美图App并俘获女友芳心的，再次为它的实力点赞。ios版+android版一共19k个star，已经证明了它的实力，还在等什么呢？
github：https://github.com/CyberAgent/android-gpuimage
作者：CyberAgent 团队
使用：
复制代码
repositories {
    jcenter()
}

dependencies {
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1'
}
复制代码
更多的改造方法，还需要阅读Ios的编程文档，对于有毅力的小伙伴强力推荐！

 
70.RxPermissions
一句话介绍：一款基于RxJava完成权限申请的框架
上榜理由：榜单里第二款提供权服务的框架，基于RxJava的设计，让你可以专心写业务，3.7K个star已经证明了它的实用价值
github https://github.com/tbruyelle/RxPermissions
作者：Thomas Bruyelle
使用：
复制代码
repositories {
    jcenter() // If not already there
}

dependencies {
    compile 'com.tbruyelle.rxpermissions:rxpermissions:0.9.4@aar'
}
复制代码
 

优雅的使用：
复制代码
RxPermissions rxPermissions = new RxPermissions(this); 

rxPermissions
    .request(Manifest.permission.CAMERA)
    .subscribe(granted -> {
        if (granted) { // I can control the camera now
        } else {
           // Oups permission denied
        }
    });
复制代码
 

71.freeline
一句话介绍：一款动态替换的编译构建框架

上榜理由：继Facebook的Buck，Androdi官方的InstRun之后，蚂蚁金服推出了Freeline编译框架，官网宣称Freeline与业内主流构建方式相比仍然有数倍的速度领先;排行有先后，编译速度并不在本榜单排序的考据因素中，因此freeline以3.7个star，暂列编译框架第二名

官网地址：https://www.freelinebuild.com/

github：https://github.com/alibaba/freeline

作者：alibaba

使用：

复制代码
buildscript {
    repositories {
        jcenter()
    }
    dependencies {
        classpath 'com.antfortune.freeline:gradle:0.8.7'
    }
}

apply plugin: 'com.antfortune.freeline'

android {
    ...
}
File → Settings... → Plugins → Browse repositories →freeline.
复制代码
 

72.RxLifecycle
一句话介绍：一款提供在使用RxJava过程中管理Activity和Fragment生命周期能力的框架

上榜理由：在榜单靠前的部分，你已经了解RxJava和RxAndroid的强大之处，但部分粗心的开发者因为没有及时取消订阅而产生严重的内存泄漏，不要担心，RxLifecycle可以为你解决难题，在gtihub上拥有3.7K个star，国内知名软件——知乎和淘宝也都在使用它

github  https://github.com/trello/RxLifecycle

作者：trello团队

使用：

clone源码到本地

 

73.classyshark
一句话介绍：一款可执行文件浏览器

上榜理由：榜单里继Apktool之后第二款apk逆向工具，如果你喜欢优雅的图形数据展示，那么你一定不能错过他，classyshark可以将破解的结果以图形化展示用户，方便分析，3.7K个star，让它暂列apk逆向工具第二位！

github  https://github.com/google/android-classyshark

作者：google

使用：

下载 JAR 

 

74.acra
一句话介绍：一款提供记录APP崩溃日志能力的框架

上榜理由：如果你面临着收集APP崩溃日志的需求，那么acra是个不错的选择。3.7K个star，让acra位列崩溃日志框架排行榜第一名，acra有足够的能力记录线上APP，并且发回服务端，acra也提供了相当棒的崩溃日志统计服务端框架Acralyzer，cralyzer工作在Apache CouchDB之上，所以除了CouchDB之外，没有必要安装任何额外的软件，移动端开发者也可以借此学习服务端的建设，一举两得！

github https://github.com/ACRA/acra

服务端github  https://github.com/ACRA/acralyzer

作者：acra团队

使用：

没有什么方法比clone源码到本地更方便了

 

75.DiskLruCache
一句话介绍：一款提供磁盘文件缓存管理能力的框架

上榜理由：3.7k个star并不足以说明DiskLruCache的优秀，仅仅以管理磁盘文件能力单独拎出来成为一个框架，作者需要很大的勇气，很幸运，作者做到了，并且也成为Google官网提倡的缓存  ；如还记得上次做“一键清除缓存”、“查看缓存文件大小”功能是什么时候吗？DiskLruCache一句话就可以搞定！

github https://github.com/JakeWharton/DiskLruCache

作者：JakeWharton

使用：

 

compile 'com.jakewharton:disklrucache:2.0.2'
或者下载 latest .jar

 

76.dexposed
一句话介绍：一款支撑阿里大部分App客户端热修复、线上调试能力的框架

上榜理由：榜单上再次出现热修复框架的身影，证明App热修复技术的火热，dexposed提供图形化的性能监控、在线热修复bug漏洞、支持AOP编程思想等，不论你是企业热修复技术的设计者还是打算在热修复领域一探究竟的新人，这款框架很适合你。3.5k个star，证明它作为一门技术框架的存在，是多么令人喜爱！

github  https://github.com/alibaba/dexposed

作者：alibaba

使用：

dependencies {
        compile 'com.taobao.android:dexposed:0.1.1@aar'
    }
 

77.Litho
一句话介绍：一款提供高效构建UI能力的框架 

上榜理由：作为一款专门构建UI的框架，Litho高效的地方在于：单独开辟了用于渲染和布局的线程，然后将创建好的组件传递给UI线程去完成最终的渲染，使用更少的视图层级，来提升界面的滚动速度，值得注意的是，它仅支持开发者作出不可改变的UI组件 ,3.5K个star，证明了它在构建UI领域的价值，更多的妙处，期待你亲自去发掘！

github  https://github.com/facebook/litho

作者：facebook

 使用：

复制代码
ependencies {
  // ...
  // Litho
  compile 'com.facebook.litho:litho-core:0.3.1'
  compile 'com.facebook.litho:litho-widget:0.3.1'
  provided 'com.facebook.litho:litho-annotations:0.3.1'

  annotationProcessor 'com.facebook.litho:litho-processor:0.3.1'

  // SoLoader
  compile 'com.facebook.soloader:soloader:0.2.0'

  // Optional
  // For debugging
  debugCompile 'com.facebook.litho:litho-stetho:0.3.1'

  // For integration with Fresco
  compile 'com.facebook.litho:litho-fresco:0.3.1'

  // For testing
  testCompile 'com.facebook.litho:litho-testing:0.3.1'
}
复制代码
 

78.mosby
一句话介绍：一款提供构建MVP项目能力的框架

上榜理由：榜单靠前的部分已经介绍了MVC,MVVM,MVP的框架项目，想必此时你在构建企业项目架构上，选择或者开发一款合适的MVP框架迫在眉睫，mosby可以作为你的第一步参考，你可以封装它，也可以照抄它，无论如何，3.4K个star，证明了它在框架设计上有多受开发者的喜爱

github https://github.com/sockeqwe/mosby

作者：Hannes Dorfmann

使用：

复制代码
dependencies {

  compile 'com.hannesdorfmann.mosby3:mvi:3.0.4' // Model-View-Intent
  // or
  compile 'com.hannesdorfmann.mosby3:mvp:3.0.4' // Plain MVP
  // or
  compile 'com.hannesdorfmann.mosby3:viewstate:3.0.4' // MVP + ViewState support
}
allprojects {
  repositories {
    ...

    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }
}
复制代码
 

79.AndResGuard
一句话介绍：一款提供资源文件路径混淆 的工具

上榜理由：如果你是个对APK大小很敏感的人，那么AndResGuard一定适合你，它的原理类似Java Proguard，但是只针对资源。他会将原本冗长的资源路径变短，例如将res/drawable/wechat变为r/d/a，3.4K个star，证明了在优化APK道路上，你不是一个人在战斗！

github  https://github.com/shwenzhang/AndResGuard

作者：wechat team

使用：

clone项目到本地，其实也就是个三两句话的文档

 

80.StatusBarUtil
一句话介绍：一款提供设置沉浸式状态栏样式能力的框架

上榜理由：设计师MM总是抱怨系统状态栏不优雅？那就给她一个完美的沉浸式状态栏。StatusBarUtil可以随心所欲的设置状态栏样式，3.3K个star，足以说明它有多受设计MM的喜爱

github https://github.com/laobie/StatusBarUtil

作者：Jaeger

使用：

compile 'com.jaeger.statusbarutil:library:1.4.0'
 

81.robolectric
一句话介绍：一款不依赖于Android设备的单元测试框架，

上榜理由：sample中列举了如何对Android四大组件和常见功能测试的用例，3.2K个star，值得充满好奇心的人尝试

官网地址：http://robolectric.org/

github  https://github.com/robolectric/robolectric

作者：robolectric

使用：

testCompile "org.robolectric:robolectric:3.3.2"
 

82.Fragmentation
一句话介绍:一款提供管理Fragmen嵌套t能力的框架

上榜理由：对于Activity和Fragment使用，你一定得心应手，但如果要做一套通用的Activity&Fragment嵌套设计，想必你有点手足无措了，Fragmentation可以作为你设计Fragment管理上的第一步，3.2K个star，笔者认为有点名副其实了，项目介绍里说的是Fragment的管理能力，但并未提供Fragment&Activity生命周期、任务栈的管理能力，因此很难直接应用到企业项目当中，但源码当中的设计思路，值得笔者与诸位借鉴，拾人牙慧留有余香！

github：https://github.com/YoKeyword/Fragmentation

作者：YoKey

使用：

// appcompat v7包是必须的
compile 'me.yokeyword:fragmentation:0.10.7'
// 如果想使用SwipeBack 滑动边缘退出Fragment/Activity功能，请再添加下面的库
// compile 'me.yokeyword:fragmentation-swipeback:0.10.4'
 

83.Small
一句话介绍：轻巧的插件化框架

上榜理由：作为插件框架榜单的新成员，Small的优点是轻巧，适合作为小团队的插件开发方案，3.1K个star，让它获得了酷狗音乐等著名开发团队的青睐，如果你们的团队想逐步实施插件化开发，Small是个不错的选择！

 官网地址：http://code.wequick.net/Small/cn/cases

github  https://github.com/wequick/Small

作者：wequick 团队

使用：

复制代码
buildscript  {
    dependencies {
        classpath 'net.wequick.tools.build:gradle-small:1.2.0-alpha6'
    }
}

apply plugin: 'net.wequick.small'

small {
    aarVersion = '1.2.0-alpha6'
}
复制代码
 

84.JsBridge
一句话介绍：一款提供WebView和Javascript通信能力的框架

上榜理由：该框架提供给了允许H5页面调用通过JS调用App方法的能力；3.1K个star，简洁的通讯方式，值得每一个Web\Hybrid App开发者尝试

gtihub https://github.com/lzyzsd/JsBridge

作者：hi大头鬼hi

使用：

复制代码
repositories {
    // ...
    maven { url "https://jitpack.io" }
}

dependencies {
    compile 'com.github.lzyzsd:jsbridge:1.0.4'
}
复制代码
 

85.richeditor-android
一句话介绍：一款强大的富文本编辑框架 

上榜理由：2.8k个star，榜单里第一个为TextView提供扩展能力的框架，你暂时不需要它，但不能不知道它

github  https://github.com/wasabeef/richeditor-android

作者：Daichi Furiya

使用：

复制代码
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:richeditor-android:1.2.2'
}
复制代码
 

86.Transitions-Everywhere
一句话介绍：一款教你正确使用Transitions API（Android 转场动画API）的教学型项目

上榜理由：你可能还未尝试过Android API的Transitions 框架，可能听过，但却无法做出优雅奇妙的动效——别担心，Transitions-Everywhere正如它的名字一样，它将带你全面体验Transitions 的强大之处

github  https://github.com/andkulikov/Transitions-Everywhere

作者：Andrey Kulikov

使用：

dependencies {
    compile "com.andkulikov:transitionseverywhere:1.7.4"
}
 

87.android-viewbadger
一句话介绍：能够快速的为Android 视图加入“勋章”能力的框架

上榜理由：如果说勋章一词听起来陌生，那么显示已读未读个数、小红点标记信息这一类词语你一定不太陌生，笔者相信在诸位实际开发中经常遇到为某些item加入小红点标记的需求，聪明的各位一定有着各种实现方案，为什么不能快速优雅的完成呢？android-viewbadger可以帮你实现，当然，在某些情况下，你需要具备修改源码的能力，以符合设计MM的需求！值得注意的是，这宽项目已经五年没有更新了！

github https://github.com/jgilfelt/android-viewbadger

作者：Jeff Gilfelt

使用：

clone源码到本地

View target = findViewById(R.id.target_view);
BadgeView badge = new BadgeView(this, target);
badge.setText("1");
badge.show();
 

88.AndroidWiFiADB
一句话介绍：一款不用数据线也可以让你调试手机设备APP的插件项目

上榜理由：你是否还在担心测试过程中高强度的拔插数据线对手机电池和USB端口造成终生难以弥补的损害？别担心，有wifi有AndroidWiFiADB，无须数据线也可以调试应用了，更有趣的是，在测试工程师一边拿着手机一边找你聊bug的时候，你已经偷偷在它的手机上修复了bug，深藏功与名！

github https://github.com/pedrovgs/AndroidWiFiADB

作者：Pedro Vicente Gómez Sánchez

使用：

Preferences/Settings->Plugins->Browse Repositories->serch AndroidWiFiADB
 

889.emojicon
一句话介绍：一款提供在TextView、EdiText展示表情包能力的框架

上榜理由：2.7k个star，,榜单第二款增强TextView显示能力的框架，这款专为表情包设计，如果你曾经好奇微信、QQ的表情显示是如何做到的？这款框架一定能满足你的求知欲。

 

90.packer-ng-plugin
一句话介绍：一款打爆工具插件

上榜利用：笔者尽力维护榜单涉及范围的全面性，因此引入此插件项目——项目号称完成100个渠道包只需要10秒钟，在市面上各种各样多渠道打包方案的今天，选择一款适合自己团队的，才是上上选择

github https://github.com/mcxiaoke/packer-ng-plugin

作者：Xiaoke Zhang

使用：

复制代码
buildscript {
    ......
    dependencies{
    // add packer-ng
        classpath 'com.mcxiaoke.gradle:packer-ng:1.0.9'
    }
} 
复制代码
 

复制代码
apply plugin: 'packer' 

dependencies {
    compile 'com.mcxiaoke.gradle:packer-helper:1.0.9'
} 

 android {
    //...
    signingConfigs {
      release {
          // 满足下面两个条件时需要此配置
          // 1. Gradle版本 >= 2.14.1
          // 2. Android Gradle Plugin 版本 >= 2.2.0
          // 作用是只使用旧版签名，禁用V2版签名模式
        v2SigningEnabled false 
      }
    }
  }
复制代码
 

91.android-priority-jobqueue
一句话介绍：一款提供后台任务管理能力的框架

上榜理由：如果你是个志在深入研究多线程操作的开发者，这个项目一定不要错过，不论是Activity重新加载、Service使用线程池时的任务优先级和并发问题，都不要担心，Job Manage会照顾优先级，持久性，负载平衡，延迟，网络控制，分组，2.4K个star，优秀的多线程管理能力，况且它依赖的第三方框架很少，值得你一试

github  https://github.com/yigit/android-priority-jobqueue

作者：Yigit Boyar

 

92.Android-Debug-Database
一句话介绍：一款提供测试App内部数据库能力的框架

上榜理由：榜单里第二款针对调试数据库的框架，一行代码集成，直接在浏览器增删改查App的数据库，2.3k个star，心动不如行动！

github  https://github.com/amitshekhariitbhu/Android-Debug-Database

作者：AMIT SHEKHAR

使用：

debugCompile 'com.amitshekhar.android:debug-db:1.0.0'
浏览器键入

 http://XXX.XXX.X.XXX:8080
 

93.conceal
一句话介绍：一款facebook提供的加密本地大文件的框架

上榜理由：如果还在担心App内的图片的隐私问题，这款facebook提供的文件加密框架足以解决你的问题，facebook客户端的图片和数据都是使用conceal加密的

官网地址：http://facebook.github.io/conceal/

github https://github.com/facebook/conceal

作者;facebook

使用：

clone项目到本地/官网下载jar

 

94.ARouter
一句话介绍：一款提供服务、页面跳转路由的框架

上榜理由：正如作者宣称的那样，该框架提供：从外部URL映射到内部页面、跨模块的页面跳转（页面解耦）、拦截跳转过程等能力，还有更多功能等你去发掘，2.1K个star，值得为企业级的框架喝彩

github  https://github.com/alibaba/ARouter

作者：alibaba 

使用：

复制代码
ndroid {
    defaultConfig {
    ...
    javaCompileOptions {
        annotationProcessorOptions {
        arguments = [ moduleName : project.getName() ]
        }
    }
    }
}

dependencies {
    // 替换成最新版本, 需要注意的是api
    // 要与compiler匹配使用，均使用最新版可以保证兼容
    compile 'com.alibaba:arouter-api:x.x.x'
    annotationProcessor 'com.alibaba:arouter-compiler:x.x.x'
    ...
}
// 旧版本gradle插件(< 2.2)，可以使用apt插件，配置方法见文末'其他#4'
// Kotlin配置参考文末'其他#5'
复制代码
 

95.MagicaSakura
一句话介绍：一款提供多主题切换能力的框架

上榜理由：框架所提供的能力，一直是本榜单所看重的，这款由bilibili提供的多主题框架，作为榜单所涉及范围能补充，1.9个star，感谢bilibili团队所作出的贡献！

github https://github.com/Bilibili/MagicaSakura

作者:Bilibili

使用：

compile 'com.bilibili:magicasakura:0.1.6@aar'
 

96.CustomActivityOnCrash
一句话介绍：一款当APP crash的时候自动载入某个Activity的框架（而不是显示Unfortunately, X has stopped）

上榜理由：新奇的创意是榜单所需要的，所以它赢得了1.8K个star；作为开发者应该拥有考虑到各种潜伏的bug的能力，但我们不能总是面面俱到，其他系统端的同事也可能造成程序的意外crash，因此，如何让程序优雅的crash->重启值得我们思考，这款框架就提供了这种能力

github  https://github.com/Ereza/CustomActivityOnCrash

作者：Eduard Ereza Martínez

使用：

dependencies {
    compile 'cat.ereza:customactivityoncrash:2.1.0'
}

添加到 Application class:
复制代码


@Override
public void onCreate() {
    super.onCreate();

    CaocConfig.Builder.create()
        .backgroundMode(CaocConfig.BACKGROUND_MODE_SILENT) 
        .enabled(false) //default: true
        .showErrorDetails(false) //default: true
        .showRestartButton(false) //default: true
        .trackActivities(true) //default: false
        .minTimeBetweenCrashesMs(2000) //default: 3000
        .errorDrawable(R.drawable.ic_custom_drawable) //default: bug image
        .restartActivity(YourCustomActivity.class) //default: null (your app's launch activity)
        .errorActivity(YourCustomErrorActivity.class) //default: null (default error activity)
        .eventListener(new YourCustomEventListener()) //default: null
        .apply();
}
复制代码
 

 

97.XhsEmoticonsKeyboard
一句话介绍：最开心的开源表情解决方案

上榜理由：如果你还在发愁如何为你的APP自制键盘，那么此框架非常适合你，而且还提供表情包展示能力，1.7个star证明了它的独特。此外作者还附赠了高仿微信键盘，QQ键盘的demo，分享给诸位

github https://github.com/w446108264/XhsEmoticonsKeyboard

作者：zhongdaxia

使用：

复制代码
allprojects {
    repositories {
        jcenter()
        maven { url "https://jitpack.io" }
    }
}


dependencies { 
    compile 'com.github.w446108264:XhsEmoticonsKeyboard:2.0.4'
}
复制代码
 

 

三.完整项目
1.iosche
一句话介绍：谷歌2016开发者大会的展示项目

上榜理由：github上有13.4k个star，位居企业级项目排行榜第一位，牛逼的开发者，权威的设计模式，标准的项目写法，值得一试；笔者建议初学者down下源码，找到app入口，每个页面走一通，配合设计模式的概念加深理解。

github https://github.com/google/iosched

作者： Google

 

2.Plaid
一句话介绍：提供设计新闻和灵感的开源app

上榜理由：标准的material design设计，新闻类app，github上9k的star量值得你摒弃市面上参差不齐的新闻app，快点下手研究它吧！

github  https://github.com/nickbutcher/plaid

 作者： Nick Butcher

 

3.PocketHub
一句话介绍：Github的Android版

上榜理由：8.7K的star数量，Github的亲生儿子，开放的源码值得各位一探究竟

github https://github.com/pockethub/PocketHub

作者:Fadil Sutomo

使用：

down下所有源码

 

4.Signal Android
一句话介绍：Signal是一款安全通讯的短信类app，

上榜理由：7.9K的star数量，工具类app的标签属性，让它在排行榜中独一无二，如果你对短信app有兴趣，可以深入探究一番

github https://github.com/WhisperSystems/Signal-Android

作者：WhisperSystems

使用：github上down源码

 

5.android-UniversalMusicPlayer
一句话介绍：一款跨设备运行的多媒体app

上榜理由：googlesamples良心推荐，github拥有7.9k个star，可以在Android手机，汽车，平板，穿戴设备上使用，对于仅仅体验过Android手机开发的程序员，会不会很新奇呢？你值得一试！

github https://github.com/googlesamples/android-UniversalMusicPlayer

作者：Google

使用：github上down源码

 

6.HomeMirror
 一句话介绍：如果你是个爱美的家伙那么你一定需要这面镜子！

上榜理由：工具类App很难再github上有一席之地，除非它提供特别新奇的功能，比如HomeMirror，github上有用7599个star，仅仅因为它提供了镜子的功能。从现在起，Android 手机、pad，都将成为你旅游居家神器，值得拥有！

github  https://github.com/HannahMitt/HomeMirror

作者：Hannah Mittens 

HomeMirror初体验：



 

7.ExoPlayer
一句话介绍：一款 替代Android原生MediaPlayer的媒体播放器

上榜理由：也许是Google对自家MediaPlayer API不甚满意，所以诞生了ExoPlayer，ExoPlayer提供了强大的扩展API，使用它来制作多媒体播放器更快捷，更容易扩展，对多媒体播放器感兴趣的同仁们可以用它来大展身手了！6.9K个star，证明它有多受开发者们喜爱，更难能可贵的是，google还在更新维护着！

官网地址：https://google.github.io/ExoPlayer/

github  https://github.com/google/ExoPlayer

作者：google

使用：

复制代码
repositories {
    jcenter()
}
compile 'com.google.android.exoplayer:exoplayer:r2.X.X'

compile 'com.google.android.exoplayer:exoplayer-core:r2.X.X'
compile 'com.google.android.exoplayer:exoplayer-dash:r2.X.X'
compile 'com.google.android.exoplayer:exoplayer-ui:r2.X.X'
复制代码
 

8.cheesesquare
一句话介绍：Android 材料设计的展示性项目

上榜理由:作者被称为是Android Support Lib背后的男人，他写出的展示性项目，怎能不推荐上榜？材料设计已经炒了好几年了，但作为最权威的展示项目，你一定需要它，6.7个star证明了它是多么的受欢迎。

github  https://github.com/chrisbanes/cheesesquare

作者：Chris Banes

 

9.DanmakuFlameMaster
一句话介绍：android端开源弹幕引擎

上榜理由：bilibili出品，保证了它的纯种品质，并且ndk源码也一并开源，可谓业界良心，该弹幕引擎的开源节省了很多视频直播小伙伴的开发成本，笔者强力推荐！

github https://github.com/Bilibili/DanmakuFlameMaster

作者：bilibili

使用：

复制代码
repositories {
    jcenter()
}

dependencies {
    compile 'com.github.ctiao:DanmakuFlameMaster:0.8.3'
    compile 'com.github.ctiao:ndkbitmap-armv7a:0.8.3'

    # Other ABIs: optional
    compile 'com.github.ctiao:ndkbitmap-armv5:0.8.3'
    compile 'com.github.ctiao:ndkbitmap-x86:0.8.3'
}
复制代码
 

10.facebook-android-sdk
 一句话介绍：一款提供接入facebook平台能力的框架

上榜理由：无论是你有接入facebook的需求，还是有学习自制sdk的需求，这都是很棒的途径；如何开发一套企业级sdk，是进阶优秀开发工程师的必须之路，4.1k个star，facebook持久更新质量保证，你值得拥有！

github https://github.com/facebook/facebook-android-sdk

作者：facebook

使用：

 https://developers.facebook.com/docs/android
 

11.android-oss
一句话介绍：国外创意社区Kickstarter 开源的Android版客户端

上榜理由：精致的企业级APP，每个页面处理得都很棒，如果你志在成为一个优雅工程师，这款开源项目一定适合你，3.8k个star证明了它不俗的生命力

github：https://github.com/kickstarter/android-oss

作者：kickstarter

使用;

clone源码到本地

 

12.k-9
一句话介绍：Android端客户端邮件App

上榜理由：还记得张小龙的成名作——FoxMail吗？如果你想做一款移动端Email App，k-9具有很好的借鉴价值，此外对于应用层协议你也会有更深的认识

官网地址： https://k9mail.github.io/

github  https://github.com/k9mail/k-9

使用：

clone项目到本地

 

13.Timber
一句话介绍：一款音乐播放器类App

 上榜理由：3K个star，完全按照材料设计规范，提供十几种播放特性，而且还提供App的通用设置能力，这一点做的同样优秀，对于志在提升开发技术的同学值得一试

github https://github.com/naman14/Timber

作者：Naman Dwivedi

使用：

clone源码是一个好习惯

 

14.remusic
一句话介绍：仿网易云音乐Android版App

上榜理由：学习完Timer，是否还不太满足你的胃口？remusic可以满足你的胃口——它甚至可以拿去直接当上线项目了！2.9K个star，基于Timber的设计（入手的前提是先搞懂Timber）值得入手；有一个问题：如果由你重构，你会如何做呢？

github https://github.com/aa112901/remusic

作者：MW

使用：

clone项目

 

15.Douya
一句话介绍：开源豆瓣客户端

上榜理由：一款功能全面、架构设计不俗的开源APP；仅仅是对豆瓣APP设计思路不满而进行的重构项目，可见作者对产品的痴迷和热爱，2.9K个star，证明该项目并不是头脑发热一时兴起的作品，如果每一个idea都能实现，那我们的世界将会多么美妙！

github  https://github.com/DreaminginCodeZH/Douya

作者：Zhang Hai

使用：

clone项目到本地

 

16.BookReader
一句话介绍：开源小说阅读器

上榜理由：2.7K个star，榜单里第一款阅读器APP，具有很高的学习价值（针对有兴趣往阅读工具类方向发展的同学）

github https://github.com/JustWayward/BookReader

作者：JustWayward 团队

使用：

clone到本地 

 

17.bilibili-android-client
一句话介绍:高仿bilibili的Android客户端

上榜理由：2.5K个star，榜单里第一款视频直播开源App；适合对视频直播、社区互动感兴趣的同学；bilibili-android-client里使用了很多大型框架，此项目并不适合基础薄弱的同学，不要灰心，学习页面的布局设计也是值得的！

github  https://github.com/HotBitmapGG/bilibili-android-client

作者：Hcc

使用：clone到本地

 

18.AndroidChromium
一句话介绍：Android版chrome浏览器

上榜理由：正如作者宣称的那样:

谷歌浏览器安卓版源码项目
世界级的安卓架构
理清本项目业务逻辑完全可以胜任国内一线公司工程师
　　对于志在梳理浏览器框架的你，值得拥有

github https://github.com/JackyAndroid/AndroidChromium

作者：JackYAndroid

使用：

clone源码到本地

四.开发框架：
（排名无先后、只按类型划分）
1.libgdx
一句话介绍：一款跨平台的android端游戏开发框架

上榜理由：android端开发框架类第一名，11.7K的star量，游戏框架是它的专属标签，更重要的是它是跨平台的

官网地址  http://libgdx.badlogicgames.com/

github https://github.com/libgdx/libgdx

2.xUtils
一句话介绍：老牌企业级开发框架

上榜理由：4.9K个star，xUtils作为上古时期程序员备受推崇的开发框架，最大的原因——省事。xUtls包含四大模块，与之而来的是提供四大操作能力：数据操作、UI操作、Http协议操作、图片操作。xUtils作为笔者初学Android框架设计的导师型项目，在笔者多年经验中，看到xUtils作为众多中小银行Android端框架方案首选，足以证明它的受欢迎程度。该框架现在已经更新到了xUtils3，如果你对Android框架涉及有一定的想法，可以从xUtils入手，进阶为框架大师行列。虽然框架中很多引擎已经过时，各个模块的做法都可以用其他框架替代，但xUtils作为国内开发者的骄傲，上古时期的框架宠儿，值得你拥有！

github  https://github.com/wyouflf/xUtils

作者：wyouflf

使用：

compile 'org.xutils:xutils:3.5.0'
3.android-common
一句话介绍： 一款android快速开发框架

上榜理由：滴滴资深级Android工程师出品，历经多年开发者的检验，以4.3K屹立于快速开发框架榜第三名，该框架提供了图片缓存、Http缓存、DropDownListView、下载模块、开发常用工具类等，作为上古时期程序员最早的总结性开发框架，它是一代人智慧的结晶，值得我们为作者Trinea鼓掌喝彩

github  https://github.com/Trinea/android-common

作者：Trinea

使用：

clone代码到本地

4.Vitamio
一句话介绍：一款支持跨平台的Android多媒体开发框架

上榜理由：如果之前提到的exoplayer不能满足你开发多媒体的需求，那我保证vitamio值得你一试

官网地址：https://www.vitamio.org/

github https://github.com/yixia/VitamioBundle

作者：yixia团队

使用：

clone源码到本地

 

5.Weex
一句话介绍：移动端跨平台开发的解决方案

上榜理由：14.4K个star，有成熟应用案例的企业级混合开发框架，阿里巴巴出品，为什么不试试呢？

官网地址：https://weex.apache.org/cn/

github  https://github.com/alibaba/weex

作者：alibaba

 

6.cordova-android（Hybrid 开发框架、WebApp开发框架）
一句话介绍：跨平台的开发框架

上榜理由：cordova有足够的能力完成混合开发、WebApp开发的需求：不论你是Web开发者，或者是Native开发者，使用cordova都可以作出跨平台的App 

官网地址：http://cordova.axuer.com/docs/zh-cn/latest/guide/overview/index.html

github https://github.com/apache/cordova-android

 

7.react-native
一句话介绍：一款以Javascript的语言来操作多个系统语言（Ios、Android）的框架

上榜理由：很难讲react-native属于什么类别，它适合前端工程师开发移动端App，也适合Native开发者进行跨平台的开发，但对于Navitve开发者来说陡峭的学习曲线会吓走一大批“框架爱好者”；前端界有一句名言：Web代表着未来，Native代表着现在，而我们处在现在与未来的道路上；49K个star，似乎让我们离未来更进一步

官网地址： http://facebook.github.io/react-native/docs/getting-started.html

github  https://github.com/facebook/react-native

作者：facebook 

 

五.其他：
1.AndroidUtilCode
一句话介绍：提供了数量庞大的工具类

上榜理由：10.8K的star个数，足以证明它是多么受欢迎，欢迎你提供常用的工具类壮大它！

github https://github.com/Blankj/AndroidUtilCode/blob/master/README-CN.md

 

File → Settings... → Plugins → Browse repositories...
and search for freeline.

 

2.kotiln
一句话介绍：Google推出的Android编程语言

上榜理由：就像AndroidStudio取代Eclipse那样，Goolg将kotiln作为Android的官网语言，也许是为了避免同Oracle的专利诉讼，但kotlin 100%兼容java，大幅精简java代码量，以及函数式编程的思想这些优异的特性同意值得我们注意，还记得在榜单之前说过的吗？未来是kotlin的，当下是java的，但我们处在当下通往未来的道路上——学习未来的编程语言，提升自己的工作效率，早点下班打豆豆，何乐而不为？

官网地址：http://kotlinlang.org/

github：https://github.com/JetBrains/kotlin

 使用：

http://kotlinlang.org/docs/reference/   提供了 api-android用例-书籍等资源

 

 

六.书籍类项目
（排序无先后）
1.Android developer中国官网培训课程
一句话介绍：符合中国国情的Google开发者官网的子产品——Android开发者官网

上榜理由：这里有培训课程、API用例课程、Sample用例、依赖库介绍、AndroidStudio官网...等等一系列公开免费的课程，尽管大部分内容还是英文讲解，可是你肯靠着英语词典一篇一篇啃完，相信我，你的Android知识水平将秒杀国内市面上大部分的Android书籍

官网地址：https://developer.android.google.cn/training/index.html

作者：google

 

2.android-architecture
一句话介绍：google提供的Android当下各种基本框架

上榜理由：看完它，mvp，mvvm都将入切瓜砍菜，秋风扫落叶一般...

github https://github.com/googlesamples/android-architecture

作者：google

 
3.andorid-open-project
一句话介绍：囊括Android几乎所有的开源项目的导航类目录

上榜理由：23k个star的导航类目录，与其盛名不符的是，该项目的导航、浏览阅读体验做的非常差，建议消遣之余阅读；推荐理由——中国人做的最全的Android 开源项目导航目录

github https://github.com/Trinea/android-open-project

作者：Trinea

 

4.awesome-android-ui
一句话介绍：Android的开源项目目录

上榜理由：国外的一款导航目录，23k个star

github  https://github.com/wasabeef/awesome-android-ui