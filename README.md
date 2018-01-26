# AllFrameWork2017


1. Retrofit����
һ�仰���ܣ�Retrofit��һ�����Ͱ�ȫ�������ܣ�����HTTPЭ�飬������Android��java����

�ϰ����ɣ�Retrofit��21.8k��stars���۾�github��android�ӱ�����ף���һ��֮������

������ַ http://square.github.io/retrofit/

github   https://github.com/square/retrofit

���ߣ�square�Ŷ�

ʹ�ã�

compile 'com.squareup.retrofit2:retrofit:2.3.0'
 

2.okhttp
һ�仰���ܣ�okhttp��һ�����HTTP��HTTP2.0Э��������ܣ�������java��android�ͻ���

�ϰ����ɣ�okhttp��20.4k��stars���۾�github��android�ӱ���ڶ��������͹�˾�����Ա�Ҳ��װ����okhttp��Retrofit2.0��ʼ����okhttp��ܣ�Retrofitרע��װ�ӿ����ҵ������okhttpרע��������İ�ȫ��Ч�����߽��������ֿ��������ú���ѧϰ��֪�����������׿�ܣ�ѧϰ���ԭ��ʱ���Էֿ�ѧϰ�����������ҡ�

������ַ   http://square.github.io/okhttp/

github    https://github.com/square/okhttp

���ߣ�square�Ŷ�

ʹ�ã�

compile 'com.squareup.okhttp3:okhttp:3.8.0'
 

����

3.Butter Knife
һ�仰���ܣ�Butter Knife���ṩ��һ����������ʹ��ע������ģ����룬��view�뷽���Ͳ����󶨡�

�ϰ����ɣ�github��16.5K��star�����Androidstudio�ṩ��Butter Knife���������������ʡȴ��Ƶ��findviewbyid�ķ��գ����µ�Butter Knife���ṩ��onclick���Լ��ַ����ĳ�ʼ������ѧ�߿��Բ���Butter Knife�Լ�Butter Knife�����һ��ѧϰ��

������ַ��http://jakewharton.github.io/butterknife/

github��https://github.com/JakeWharton/butterknife

���ߣ�JakeWharton ��Ҳ��square�Ŷӳ�Ա֮һ

ʹ�ã�

dependencies {
  compile 'com.jakewharton:butterknife:8.6.0'
  annotationProcessor 'com.jakewharton:butterknife-compiler:8.6.0'
}
 

4.MPAndroidChart
һ�仰���ܣ�MPAndroidChart��һ��ͼ����

�ϰ����ɣ�github��16.1K��star���Կ��١���ࡣǿ�����Ƶ�ͼ����

������ַ https://github.com/PhilJay/MPAndroidChart  

github  https://github.com/PhilJay/MPAndroidChart

���ߣ�PhilJay

ʹ�ã�

1. ��AS�м���Gradle����

�ڸ�Ŀ¼�� build.gradle�ϼ���:
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
 

����

��app��build.gradle�ϼ��룺
dependencies {
    compile 'com.github.PhilJay:MPAndroidChart:v3.0.2'
}
 

��

5. glide
һ�仰���ܣ�glide��һ��רע���ṩ�������������ġ�ͼƬ���غͻ����ܡ�

�ϰ����ɣ�15.9k��star��ͼƬ��������������һ�Ŀ�ܣ�google ��2014�����ߴ������ʾ��camera app���ǻ���gilde��ܿ�����

github https://github.com/bumptech/glide

���� Bump Technologies�Ŷ�

ʹ�ã�

���ƴ���
repositories {
  mavenCentral()
}

dependencies {
    compile 'com.github.bumptech.glide:glide:3.8.0'
    compile 'com.android.support:support-v4:19.1.0'
}
���ƴ���
6.leakcanary
һ�仰���ܣ�һ���ڴ����ܣ�������java��android�ͻ���

�ϰ����ɣ����㣬�����leakcanary�����ص㣬ֻ����Ӧ�õ�apllication�м��ɣ��Ϳ���ֱ��ʹ������15.5k��star˵�������ж�ô�ܻ�ӭ

github https://github.com/square/leakcanary

���� square�Ŷ�

ʹ�ã�

 dependencies {
   debugCompile 'com.squareup.leakcanary:leakcanary-android:1.5.1'
   releaseCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1'
   testCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.1'
 }
�� Application ��д��:

���ƴ���
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
���ƴ���
 

7.Android-Universal-Image-Loader
һ�仰���ܣ�������ͼƬ���ؿ�����ߣ�android�������ֶ��ù���

�ϰ�����:android��ͼƬ���ؿ�ܵ��ϴ���ˣ�15.3k��star����֤���������ţ�UIL��gilde��������ǿɶ��ƣ�UIL�ṩ�˴������÷�ʽ��ͼƬ����״̬�Ļص����ɹ���ʧ�ܣ������У������ض����ȣ��Լ��ṩ���ƶ���ͼƬ���ؿ�ܵĻ���˼·������������� sd��-�ڴ�-���磻ֵ��ע����ǣ�UIL�Լ�����δ�����ˣ����������Ƽ���λʹ�ã�

github https://github.com/nostra13/Android-Universal-Image-Loader

���� nostra13

ʹ�ã�

���ص�ַ  universal-image-loader-1.9.5.jar

 

 

8.EventBus 
һ�仰���ܣ�EventBus��һ��������ͨ�ſ��

�ϰ����ɣ������ͨ�ſ��star����һ��14.8k���ڴ�����Ŀ��Activities��fragments��Threads��Services�����Կ�������ʹ�ó���������EventBus����δ��������������¼�ʱ��Щ���ޣ����ʺ��ڡ����ŵġ�����䴫����Ϣ�����Բ���������Ծ�ڸ���������Ŀ���������

������ַ http://greenrobot.org/eventbus/documentation/how-to-get-started/

github  https://github.com/greenrobot/EventBus

���� greenrobot 

ʹ�ã�

compile 'org.greenrobot:eventbus:3.0.0'
 

9.zxing
һ�仰���ܣ�����ͼ�����

�ϰ����ɣ�������ù���ά�룬��϶��Ѿ����ʹ�ù�����������zxing�ˡ�13.9K��star�����������ڱ��񵥵ھţ�ʵ�����飬��������˽��ά������󣬲������˽⡢�޸���Դ�����֡�

github  https://github.com/zxing/zxing

����  Sean Owen

 

10.picasso
һ�仰���ܣ�ǿ����ͼƬ���ء�������

�ϰ����ɣ����񵥳��ֵĵ�����ͼƬ���ܣ���ͬ����picasso��ǿ��ͼƬ���أ�����Խ�picasso���ɽ������Ŀ�У���Ҳ���Խ��gilde��UIL��picasso������һ���װ�������Ŀ�У��������á�

������ַ http://square.github.io/picasso/

github  https://github.com/square/picasso

���� square�Ŷ�

ʹ�ã�

compile 'com.squareup.picasso:picasso:2.5.2'
��������

jar��

 

11.lottie-android
һ�仰���ܣ�һ�������Android�˿���չʾAdobe Afeter Effect��AE���������������Ŀ��

�ϰ����ɣ��������ܵ�һ����github��13.3k��star֤����������Խ�ԣ�����json�ļ�����ʵ�ֶ���Ч���������ı����������json�ļ�Ҳ����Adobe�ṩ��After Effects��AE�����������ģ���AE��װһ��Bodymovin�Ĳ����ʹ�����������ս�����Ч������json�ļ������json�ļ�������LottieAnimationView����������Ѥ���Ķ���Ч������������֧�ֿ�ƽ̨Ӵ��

github  https://github.com/airbnb/lottie-android

���ߣ�Airbnb �Ŷ�

 

12.fresco
һ�仰���ܣ�һ����Թ���ͼƬ�ڴ�Ŀ��

�ϰ�����:github��12.8k��star��ͼƬ�����а��������facebook�ĳ���֤�������������ظ�������ӣ��ڹ���ͼƬ�ڴ���������������һƬ��أ�����ʽ���ء�����gif��������ǰ��λ��ȶ��е�����

������ַ�� https://www.fresco-cn.org/

github  https://github.com/facebook/fresco

���� facebook

ʹ�ã�

dependencies {
  // ��������
  compile 'com.facebook.fresco:fresco:0.12.0'
}
�����������Ҫ����������ӣ�

���ƴ���
dependencies {
  // �� API < 14 �ϵĻ���֧�� WebP ʱ����Ҫ���
  compile 'com.facebook.fresco:animated-base-support:0.12.0'

  // ֧�� GIF ��ͼ����Ҫ���
  compile 'com.facebook.fresco:animated-gif:0.12.0'

  // ֧�� WebP ����̬ͼ+��ͼ������Ҫ���
  compile 'com.facebook.fresco:animated-webp:0.12.0'
  compile 'com.facebook.fresco:webpsupport:0.12.0'

  // ��֧�� WebP ��̬ͼ����Ҫ���
  compile 'com.facebook.fresco:webpsupport:0.12.0'
}
���ƴ���
 

13.RxAndroid
һ�仰���ܣ�һ��Android�ͻ���������첽ͨ�ŵĿ��

�ϰ����ɣ�github��12.7k��star��λ�����ͨ�ſ�ܵĵڶ���������EventBus֮�����Ҫ�����ߵ�����Eventbus������ȡ������䷱����interface��RxAndroid������ȡ��AnsyTask�ģ�������ͻ����ȻRxAndroid���ŵ㲢�������ڴˣ��������ŵ�ʵ�֣�����ȥ�������ģ�

github  https://github.com/ReactiveX/RxAndroid

���� JakeWharton

ʹ�ã�

compile 'io.reactivex.rxjava2:rxandroid:2.0.1'
compile 'io.reactivex.rxjava2:rxjava:2.1.0'
 

14.SlidingMenu
һ�仰���ܣ��໬�˵������

�ϰ����ɣ���Userval-Image-loader �������Ϲ�������ܡ���Ϊ���app�ṩ�໬�˵����Ĺ��ܣ�github������10.5k��star��֤�������ľ��ò�˥����ʹ��Google�Ƴ���NavigationDrawer����Ȼû�м��ٿ����߶�SildingMenu��ӵ�أ��������Ǿ�������ģ�����Ϲ������Ѿ�����û�и����ˣ���̫��̫���appʹ�ù�������Щ������������Ŀ�Դ����Ͽ�����

github https://github.com/jfeinstein10/SlidingMenu

���� Jeremy Feinstein

ʹ�ã�

��gihub��forkԴ�룬���ɽ���Ŀ��

 

15.PhotoView
һ�仰���ܣ�һ��ImageViewչʾ��ܣ�֧�����ţ���Ӧ����

�ϰ����ɣ�10.3k��star������λ��ͼƬ�������а����λ��PhotoView��ǰ��λ��ͬ������δ�������ͼƬ��չʾ��������һ������΢�ŵ�ͷ�����Ŵ������ʵ�ֵģ��ܶ�App��ͼƬ��ʾ��Ӧ���ư�ѹ�����ʵ�ֵģ��˽�PhotoView����һ���Ὺ�ĵģ�������Ҳ���������ImageView�ĵ���Ŵ�Ч����Android��sampleҲ�У�

github  https://github.com/chrisbanes/PhotoView

���ߣ�chrisbanes

ʹ�ã�

���ƴ���
��app��Ŀ¼��build.gradle�м��룺
allprojects {
    repositories {
        maven { url "https://jitpack.io" }
    }
}
��app��moduleĿ¼��build.gralde�м��룺

dependencies {
    compile 'com.github.chrisbanes:PhotoView:latest.release.here'
}
���ƴ���
ʹ��

���ƴ���
<com.github.chrisbanes.photoview.PhotoView
    android:id="@+id/photo_view"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>


PhotoView photoView = (PhotoView) findViewById(R.id.photo_view);
photoView.setImageResource(R.drawable.image);
���ƴ���
 

16.material-dialogs
һ�仰���ܣ�һ���Զ���dialog���

�ϰ����ɣ�9.9k��star��Ҳ�Ǽ�PhotoView��SlidingMenu֮��������Զ���View��ܣ�Ҳ���㻹���Զ���View�����ˣ���Dialogʹ�õĻ��е����裬�����ͨ�����������Dilaogʹ������

github  https://github.com/afollestad/material-dialogs

���ߣ�Aidan Follestad

ʹ�ã�

dependencies {
    // ... other dependencies here
    compile 'com.afollestad.material-dialogs:core:0.9.4.5'
}
 

17.droid-async-http
 һ�仰���ܣ�һ�����HttpЭ����첽����������ܣ�

�ϰ����ɣ���Ȼ����������ʹ��retrofit+okhttp�����ɣ���9.8k��star��֤������Ȼֵ��������ѧϰ��ֵ��ע����ǣ���Ҳ�Ѿ�������û�����ˣ��㾡����ȥ������������ɣ�

github   https://github.com/loopj/android-async-http

���ߣ�James Smith

ʹ�ã�

���ƴ���
repositories {
  maven {
    url 'https://oss.sonatype.org/content/repositories/snapshots/'
  }
}
dependencies {
  compile 'com.loopj.android:android-async-http:1.5.0-SNAPSHOT'
}
���ƴ���
 

18.androidannotations
һ�仰���ܣ�һ�����ע��Ŀ��ٿ������

�ϰ����ɣ���Butterknifeһ������ע�⣬����ע��������view�ĳ�ʼ������ͬ����androidannotations�ṩ�˸�����������򵥵��߳�ģ�͵ȣ�����ֻ�Ӵ���Butterknife���޷�����һ������androidannotations�����ƣ������־�������˽�ע������ã����Գ���̽��һ�£�

������ַ http://androidannotations.org/

github https://github.com/androidannotations/androidannotations

���ߣ� WonderCsabo

 

19.fastjson
һ�仰����:һ�����json���������ɵĿ��

�ϰ����ɣ����������ֲ��ѿ��������������������ԣ�����Ͱ͵ĳ���֤�˴������������Խ��9.4k��star������Ҳ�ǰ����һ�����ֵ��й���Դ��ܣ��漰�����app�����õ�json��fastjsonֵ����Ϊ�����ѡ��

github  https://github.com/alibaba/fastjson

���ߣ�alibaba

ʹ�ã�

compile 'com.alibaba:fastjson:1.1.58.android'
 

20.Material-Animations
һ�仰���ܣ�һ���ṩ����ת�����������Ķ������

�ϰ����ɣ�Android����������а�ڶ�����9.3k��star�������붯����ܰ񵥵�һ��lottie-android��ͬ���ǣ�Material-Animations�ṩ���ǳ����л��Ķ���Ч����Android ����sample���Ѿ��ṩ�˲���Transition ��ת����������չʾ����Ϊ��ѧ�ߺ��ѿ�����չ���Լ���Ŀ�У�Material-Animations��ʾ������Ϊ������ʡȥ�˴����鷳��ֱ���հ�Ӧ�õ��Լ���App�аɡ�

 github  https://github.com/lgvalle/Material-Animations

���ߣ�Luis G. Valle

ʹ�ã�

downԴ�룬�޸�ѧϰ

 

21.tinker
һ�仰���ܣ�����΢�Ź�����Android�Ȳ����������

�ϰ����ɣ�9.1k��star��΢�����õ��Ȳ����������Ķ������ж�

������ַ  http://www.tinkerpatch.com/Docs/intro

github   https://github.com/Tencent/tinker

���ߣ�Tencent

 

 

22.ViewPagerIndicator
һ�仰���ܣ�һ�����ViewPager��ҳ��ָʾ����Դ���

�ϰ����ɣ��Ϲ������������Ѿ�����δ�����ˣ�������Ȼ�������Ա���app�п�������ʹ�ó�����8.9K��star��������㳲�����ڴ����ڰ���

������ַ http://viewpagerindicator.com/

github  https://github.com/JakeWharton/ViewPagerIndicator

���ߣ�JakeWharton 

ʹ�ã�

 ���� ��ַ https://github.com/JakeWharton/Android-ViewPagerIndicator/zipball/master

 

23.Android-CleanArchitecture
һ�仰���ܣ�һ��������ƿ�ܵ�demo

�ϰ����ɣ������ǿ�ܣ�����԰�������һ���飬�����̻��������Ƽ��ļܹ�����������һ��sample app�����ͼ�Ľ��⣬�㽫��Android�ͻ��˵ļܹ��и���һ�����ʶ��8.8k��star������֤��������һ�������顱Ӵ��

github  https://github.com/android10/Android-CleanArchitecture

���ߣ�Fernando Cejas

 

24..Android-PullToRefresh
һ�仰���ܣ�һ��Ϊ��ͨ��ͼ�ṩˢ��UI����ͼ���

�ϰ����ɣ�8.2K��star����ʹ��λ��ˢ����UI��ܰ��ף�ǿ��ļ����������ÿ��֧��ListView��GrdiView��WebViewScrollView��ViewPager���ڶ�View����ˢ�µ�������������������������أ��������ص�������Ӧ�ÿ������ˣ�

github https://github.com/chrisbanes/Android-PullToRefresh

���ߣ�Chris Banes

ʹ�ã�

github forkԴ�룬���ɵ���Ŀ��

 

25.flexbox-layout
һ�仰���ܣ�һ�����������

�ϰ����ɣ�8.1k��star��ǰ��H5������תAndroid�����ĸ�����FlexboxLayout��ΪLinearLayout��RelativeLayout������ߣ�ֵ�ø�λһ�ԣ�����һͬ�Ƴ��Ļ���ConstraintLayout��

github  https://github.com/google/flexbox-layout

���ߣ�Google

ʹ�ã�

dependencies {
    compile 'com.google.android:flexbox:0.3.0-alpha3'
}
 

26.AndroidSwipeLayout
һ�仰���ܣ��ǳ�ǿ�󻬶�ʽ����

�ϰ�����:����ɾ���ǹ���app����������Ʒ��������»���������Ϊ�����ߵ�����Ҳ����������AndroidSwipeLayout��github��ӵ��8K��star��֤��������ס�˼��飬��λֵ��һ��

github https://github.com/daimajia/AndroidSwipeLayout

���ߣ�daimajia

ʹ�ã�

dependencies {
    compile 'com.android.support:recyclerview-v7:21.0.0'
    compile 'com.android.support:support-v4:20.+'
    compile "com.daimajia.swipelayout:library:1.2.0@aar"
}
������ 

AndroidSwipeLayout-v1.1.8.jar

 

27.realm-java
һ�仰���ܣ�Realm��һ���ƶ������ݿ���

�ϰ����ɣ�������������C++���죬����ͨ��Sqlite�����ݿ��Ķࡣ���߲²�������ˣ�realm��7892��star������λ�ڴ������������ݿ���GreenDao��7877��֮ǰ

������ַ��https://realm.io/cn/

github https://github.com/realm/realm-java

���ߣ�Realm�Ŷ� 

ʹ�ã�https://realm.io/docs/java/latest/

 

28.greenDAO
һ�仰���ܣ�greenDAO��һ���Ч�����ٵ�SQLite�����ݿ�

�ϰ����ɣ�greenDAO��star������Realm�������£�����EventBusʦ��ͬ�ţ�Ҳ����greenrobot�Ŷӿ���ά���ģ�����������֤���������ʱ���Realm��greenDao���ߵ������ԣ�ֻ�ܾ��嵽ʵ��ʹ�õ��У�ģ�����ϵ�ʹ�����Σ����и�ǿ�Ȳ��Ժ�������жϣ����ڴ˲���һ������˵�꣬����ź�

������ַ��http://greenrobot.org/greendao/

github  https://github.com/greenrobot/greenDAO

ʹ�ã�

���ƴ���
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
���ƴ���
 

29.stetho
һ�仰���ܣ�һ���ṩ��Chrome�����߹����ϵ���Android app�����Ŀ�Դ���

�ϰ����ɣ��Ϲ�ʱ��Android����ԱҪ���Ա������ݿ⣬��Ҫ����Android Device Monitor�ҵ�/data/data/com.xxx.xxx/databases�����db�ļ���������PC�ˣ���PC�����ݹ��߲鿴������ʹ��stethoʡȴ����˵��鷳������Android����Ա������������������Ӧ�����еı��ĶΣ���Ҫ�������м���Log��䣬һ����Ϣһ����Ϣ��ӡ�������൱������������ʹ��stetho��ʡȴ���������鷳�ѣ�7.8K��star�������Android�����ߵ��Եĸ�������ֵ��ӵ�У�

���ߣ�FaceBook

������ַ�� http://facebook.github.io/stetho/

github   https://github.com/facebook/stetho

ʹ�ã�

compile 'com.facebook.stetho:stetho:1.5.0'
 

30.BaseRecyclerViewAdapterHelper
һ�仰���ܣ�ǿ��������Recyvlerviewͨ��������

�ϰ����ɣ��������RecyclerView��ӵ���ߣ���һ��Ҫ�������ר�ŷ����view����������7.7K��star��������һ�λ��github��Android ���������а��һ�����кܶྪϲ����ȥ̽Ѱ��

������ַ��http://www.recyclerview.org/

���ߣ��������Լ�����С���

ʹ�ã�

���ƴ���
allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}


dependencies {
        compile 'com.github.CymChad:BaseRecyclerViewAdapterHelper:VERSION_CODE'
}
���ƴ���
 

31.AndroidViewAnimations
һ�仰���ܣ�һ���ṩ�ɰ��������ϵĿ��

�ϰ����ɣ�����������˵���������˿���������������еĶ���Ч�������ɽ���������ɰ��Ķ�����ܡ�7.6K��star����֤�������ڶ�����������ս��������������λ��lottie-android��Material-Animations����������ܰ���֮�����ӵ�����

github https://github.com/daimajia/AndroidViewAnimations

���ߣ�daimajia

ʹ�ã�

dependencies {
        compile 'com.android.support:support-compat:25.1.1'
        compile 'com.daimajia.easing:library:2.0@aar'
        compile 'com.daimajia.androidanimations:library:2.2@aar'
}
sample��

YoYo.with(Techniques.Tada)
    .duration(700)
    .repeat(5)
    .playOn(findViewById(R.id.edit_area));
 

32. MaterialDrawer
һ�仰���ܣ�ǿ������Ϸ��ĳ�����

�ϰ����ɣ�7.6K��star���������ߵĳ�������״̬������㻹����ԥ����SlidingMenu����bugû�˹ܵ���������ô�������������Ϊ��ĳ��벼�� 

github  https://github.com/mikepenz/MaterialDrawer

���ߣ�Mike Penz

ʹ��:

compile('com.mikepenz:materialdrawer:5.9.2@aar') {
    transitive = true
}
 

new DrawerBuilder().withActivity(this).build();
 

 

 33.Android-ObservableScrollView
һ�仰���ܣ�һ������ͼ�����������Ӿ�Ч���Ļ���ʽ���

�ϰ����ɣ�7.5K��star������֤�����������ļ�ֵ��github���ṩ��12�ֻ���Ч��������������ֲ�������ܵĲ��㣬�������App���飡

github https://github.com/ksoichiro/Android-ObservableScrollView

���ߣ�Soichiro Kashima

ʹ�ã�

compile com.github.ksoichiro:android-observablescrollview
 

34.CircleImageView
һ�仰���ܣ�Բ��ImageView

�ϰ����ɣ�Ҳ�����Ѿ���˵��������չʾԲ��ͼƬ�ķ�����������㲻���Գ���CircleImageView����ô���֪ʶ�����Ϊ��������Ȼʧɫ���е�ʱ����������ǿ��������ȿ��ǵģ���ͬʵ�ַ���ǣ���������ܲ����ֵ��������˼�������������ͼƬ�������������ԣ���ôCircleImageView���Բ���������˶��顣�������˼ǵ�ȥ��Romain Guy�Ľ���Ӵ��

github https://github.com/hdodenhof/CircleImageView

���ߣ�Henning Dodenhof

ʹ�ã�

dependencies {
    ...
    compile 'de.hdodenhof:circleimageview:2.1.0'
}
 

���ƴ���
<de.hdodenhof.circleimageview.CircleImageView
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/profile_image"
    android:layout_width="96dp"
    android:layout_height="96dp"
    android:src="@drawable/profile"
    app:civ_border_width="2dp"
    app:civ_border_color="#FF000000"/>
���ƴ���
 

35.logger
һ�仰���ܣ�һ����log��־������ʾ�Ŀ��

�ϰ����ɣ�logger��Ϊ���Կ�ܣ���δ������ǿ������������������������ŵ����log��Ϣ������֧�ֶ��ָ�ʽ���̡߳�Json��Xml��List��Map�ȣ���������ճ���������󺣰��log��Ϣ�����԰Σ�logger�������ָ·���ƣ�6.6k��star����λ�е��Կ�ܵڶ���������facebook��stetho֮��

github https://github.com/orhanobut/logger

���ߣ�Orhan Obut

ʹ�ã�

compile 'com.orhanobut:logger:2.1.1'
 

Logger.d(MAP);
Logger.d(SET);
Logger.d(LIST);
Logger.d(ARRAY);
Logger.json(JSON_CONTENT);
Logger.xml(XML_CONTENT);
 

36.agera
һ�仰����:һ�������Androidƽ̨����Ӧʽ��̿��

�ϰ����ɣ�googleר���Ƴ�һ����Ӧʽ��̿�ܷ�����Android�����ߣ������֮��Ӧʽ��̿�ܰ��׵� RxJava RxAndroid�������������������Ĳ�ͬ������agera����push event��pull data ��VS Rxϵ�� push data����

github https://github.com/google/agera

���ߣ�Google

ʹ�ã�

  compile 'com.google.android.agera:agera:1.3.0'
��չ����

  compile 'com.google.android.agera:content:1.3.0'
  compile 'com.google.android.agera:database:1.3.0'
  compile 'com.google.android.agera:net:1.3.0'
  compile 'com.google.android.agera:rvadapter:1.3.0'
  compile 'com.google.android.agera:rvdatabinding:1.3.0'
 

37.BottmBar
һ�仰���ܣ�һ��ײ���������ͼ���

�ϰ����ɣ��ײ���������߿�ܣ�6.3K��star������֤�����������㣬��ȫ��ѭ������ƹ淶�����ַǳ����㡣���˵ȱ�㣬�޷�����icon��titile�ļ�࣬�޷��Զ�����ͼ�Ĵ�С�ȣ�����Щ������ͨ���޸�Դ�������������׳�Ҳ�޸���һ�׷��Ϲ��ڿ����ߵĵײ�������ܣ�������Դ��

github  https://github.com/roughike/BottomBar

���ߣ�Iiro Krankka

ʹ�ã�

compile 'com.roughike:bottom-bar:2.3.1'
 

38.Calligraphy
һ�仰���ܣ�һ���Զ���������

�ϰ����ɣ�����㻹��Ϊһ���޸�App������������ʽ�����գ�6.3K��star��Calligraphy��ֵ����ӵ�У�������ͬʱ�޸�����������Ŀ��Textview���壬Ҳ���Ե��� ����ĳ��Textview�����壬���ڵ�ʲô���������԰ɣ�

github  https://github.com/chrisjenx/Calligraphy

���ߣ�Christopher Jenkins

ʹ�ã�

dependencies {
    compile 'uk.co.chrisjenx:calligraphy:2.3.0'
}
 

39.AndroidSlidingUpPanel
һ�仰���ܣ����϶��Ļ��������ͼ���

�ϰ����ɣ���������Ŀ��Ҫһ������ק�Ļ���ʽ��壨չʾĳЩ������Ϣ���������֣���ͼ��Ϣ�ȣ�����ô�Ƽ���ʹ������6.3k��star�����Դ�ҵ��˾umano����Ʒ��֤�����������Ƴ��Ľ���

github https://github.com/umano/AndroidSlidingUpPanel

���ߣ�umano

ʹ�ã�

���ƴ���
dependencies {
    repositories {
        mavenCentral()
    }

    compile 'com.sothree.slidinguppanel:library:3.3.1'
}
���ƴ���
 

40.AppIntro
һ�仰���ܣ�һ���ṩ����������ӭҳ�Ŀ��

�ϰ����ɣ����ߴ�δ�Ѵ���ѻ�ӭҳ����������а��У���Ϊ���ڿ����ߣ�ViewPager����App�Ļ�ӭҳ�Ѿ����ֵ�����������Ϊ��һ����Դ�Ļ�ӭҳ��ܻ���github��ӵ��6.3k��star��Ҳ����᲻мһ�ˣ��ǵģ��������ڲ�мһ�˵�˲�䣬���������������ˡ�

github https://github.com/apl-devs/AppIntro

���ߣ�Paolo Rotolo

���ƴ���
    allprojects {
        repositories {
            ...
            maven { url 'https://jitpack.io' }
        }
    }

    dependencies {
            compile 'com.github.apl-devs:appintro:v4.2.0'
    }
���ƴ���
 

41.recyclerview-animators
һ�仰���ܣ�һ��ΪRecyclerview�ṩ��չ���������Ŀ��

�ϰ����ɣ���һ���ϻ������������ʧȥ�����������Ȥ���Ǿ�˵�������ˡ�recyclerview�Ѿ��Ƴ��������ˣ�������listview�����ǣ��Ƿ��Ѿ������Լ��������ϣ���Ҫ���ģ���Ϊ�����Ŀ����recyclerview-animators��ܰɣ�Ϊ���Լ����������ʵ�ѪҺ�������������߱�ע��6.2K��star��

github  https://github.com/wasabeef/recyclerview-animators

���ߣ�https://github.com/wasabeef

ʹ�ã�

dependencies {
  // jCenter
  compile 'jp.wasabeef:recyclerview-animators:2.2.6'
}
 

42.dagger
һ�仰���ܣ�һ��ͨ������ע�뽵�ͳ������ϵĿ������

�ϰ����ɣ�github ��dagger1�汾 ��6.2k��star �� dagger2�汾��7.3k������square��ɵ�dagger1�汾�������google�Ŷӽ��ֵ�dagger2�汾��ǿ�������Ŷӱ�֤�˴���������ϵ���Խ�ԣ��������̽��Android ��������ģʽ����Ҳ�ǲ����ѡ��

������ַ��https://google.github.io/dagger/

github ��https://github.com/google/dagger

���ߣ�google

ʹ�ã�

���ƴ���
dependencies {
  compile 'com.google.dagger:dagger:2.x'
  annotationProcessor 'com.google.dagger:dagger-compiler:2.x'
}
If you're using classes in dagger.android you'll also want to include:

compile 'com.google.dagger:dagger-android:2.x'
compile 'com.google.dagger:dagger-android-support:2.x' 
annotationProcessor 'com.google.dagger:dagger-android-processor:2.x'
���ƴ���
 

43.Android-Bootstarp
һ�仰���ܣ�һ���ṩ��AndroidӦ����ʵ��Bootstrap��web��ܣ�������Ч���Ŀ��

�ϰ����ɣ����ϵڶ�����Ӧweb������Android �˿�ܣ����ǵõ�һ����˭�𡪡�flexbox-layout����ΪAndroid�����ߣ����б�Ҫȥ�˽�Web�����ˡ�5.9k��star��֤��������С��

github https://github.com/Bearded-Hen/Android-Bootstrap

����:Bearded-Hen�Ŷ�

ʹ�ã�

dependencies {
   compile 'com.beardedhen:androidbootstrap:{X.X.X}'
}
 

44.RxBinding
һ�仰���ܣ�һ���ṩUI����¼���Ӧ�����Ŀ��

�ϰ����ɣ�����㻹δ��ʼRxAndroid ֮�ã�RxBinding������Ϊ��ĵ�һվ��ͨ��RXBinding���㽫�����Ӧʽ��̵Ŀ��֣�����Ŀ����¼����̸�������5.6K��star��RxAndroid�������Բٵ����������ðɣ�

github  https://github.com/JakeWharton/RxBinding

���ߣ�JakeWharton

���ƴ���
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
���ƴ���
 

45.ListViewAnimations
һ�仰���ܣ�һ��ΪListView�ṩ��չʾ��Ч�������Ŀ��

�ϰ����ɣ������һ���ҳ����Լ����ˣ��һ��������ҵ��ֵܡ���ListView��֤���Һ���һ��ս������ListViewAnimations�Ĵ��ھ���֤��������Щ�������ˡ���������֮�أ�Ҳ������˵�����ڵ��Ѵ����޷���ᵽRecyclerView�ﶯ���Ŀ��֣�ӵ��ListViewAnimations����һ�����Խ�����˵���ҵĺ��ӣ�ÿ��item��Ҳ���Լ��Ķ�Ч���������߱�ע 5.6K��star��

github  https://github.com/nhaarman/ListViewAnimations

���ߣ�nhaarman

ʹ�ã�

���ƴ���
repositories {
    mavenCentral()
}

dependencies {
    compile 'com.nhaarman.listviewanimations:lib-core:3.1.0@aar'
    compile 'com.nhaarman.listviewanimations:lib-manipulation:3.1.0@aar'
    compile 'com.nhaarman.listviewanimations:lib-core-slh:3.1.0@aar'
}
���ƴ���
 

46.UItimateRecyclerView
һ�仰���ܣ�һ���ṩˢ�¡����ظ��ࡢ������Ч�ȶ���������RecyclerView���

�ϰ����ɣ����ϵ����γ���RecyclerView����Ӱ������֤��RecyclerView�������ԣ�5.5K��star����������ṩ�ڶ��������������Ǹ����������ߣ���ô�˿�ܻ�Ϊ���ʡ�ܶ�ѧϰʱ�䣬��������ɶ�itemʽ���ֵĴ��������ֵ��ע����ǣ������ĿҲ����������Ŀ��˼·�϶��ο����ġ�

github  https://github.com/cymcsg/UltimateRecyclerView

���ߣ�MarshalChen

ʹ�ã�

���ƴ���
repositories {
    jcenter()
    }
dependencies {
    ...
    compile 'com.marshalchen.ultimaterecyclerview:library:0.7.2'
}
���ƴ���
 

47.uCrop
һ�仰���ܣ�һ�����ŵ�ͼƬ�ü����

�ϰ����ɣ�5.3K��star��ͼƬ�༭ģ�鵥�������Ҳ��һ�����ŵ�App��

github  https://github.com/Yalantis/uCrop

���ߣ�Yalantis

ʹ�ã�

���ƴ���
allprojects {
   repositories {
      jcenter()
      maven { url "https://jitpack.io" }
   }
}

compile 'com.github.yalantis:ucrop:2.2.1' 
���ƴ���
 

48.RxJava-Android-Samples
һ�仰���ܣ�һ�����RxJavaʹ�ó�����app

�ϰ����ɣ��񵥳��ֵĵ�һ��������Ϊ���������ʹ����һ����Ŀ���Ŀ�Դ��Ŀ��������˵��RxJava������������õ����벻����RxJava�÷����ﶼ�У������Ϊʲô����5.2k��star��������ݰ����ԭ���ź��Լ�û�д�����ôһ������׷����demo���Ͽ춯��д�������ġ�XX��Ŀ�����ɡ�

github  https://github.com/kaushikgopal/RxJava-Android-Samples

���ߣ�kaushikgopal

ʹ�ã�

clone����������̽����

 

49.AndroidAutoLayout
һ�仰���ܣ�һ���ṩ���������Ŀ��

�ϰ����ɣ�5.2K��star�������ϵܵ���Ʒ���ʺ�С��Ŀ�Ŀ����Ŷӣ��õ����MM��px������Ƹ��ǲ��Ǻ�ͷ����������һ��ʽ�㶨������⣬���кܶ�Ĳ��㣬����׷�����������·�ϣ���ֵ��̽�����˽��������߲����Ƽ�����Ӧ�õ��Ѿ��������е���Ŀ�У��Ͼ��������Ѿ���̫��������������ˣ�������������Ǹ����ӻ⣬�보һ�̺òˣ��͵ñ��ø������ϣ�����С������������Ѹ���С�����õ�¯�����ʱ��������ʳ����Ͳ�Զ�ˡ�

github https://github.com/hongyangAndroid/AndroidAutoLayout

���ߣ��ź���

ʹ�ã�

dependencies {
    compile 'com.zhy:autolayout:1.4.5'
}
 

50.EffectiveAndroidUI
һ�仰���ܣ�һ����ЧչʾUI�Ľ�ѧ��App

�ϰ����ɣ�������ֺ��Ѷ�MVC MVP,MVVM��ģʽ����̵���⣬�����һ��ʾ����app���ǶԳ�ѧ�߻��кܴ����棬������������ʱҲ���������4.8K��star��֤�����������˹�󿪷��ߵĿ��������ӣ�����Effective UI�ı��˼�������Android�ٷ��γ����Effective UI�γ̲�ı���ϣ����ң�����Ŀ��������fragment��dagger��������ʽ��Butterknife���ڶ�С֪ʶ�㣬��Ϊ��̳�ѧ�ߵ�ѧϰ�������ʺϲ�����

github  https://github.com/pedrovgs/EffectiveAndroidUI

���ߣ�Pedro Vicente 

ʹ�ã�

clone��Ŀ������

 

51.Luban
һ�仰���ܣ���ӽ�΢�ŵ�ͼƬѹ�����

�ϰ����ɣ��õ�˼·���ǿ�����������ʣ�Luban����ͼƬѹ����һ���ܣ�������4.8K��star��֤��������ͼƬѹ���ϵ����裬�����ܲ���������ģ���������������ӽ�ΰ�����Ŀ

github  https://github.com/Curzibn/Luban

���ߣ�Curzibn

ʹ�ã�

compile 'top.zibin:Luban:1.1.1'
 
52.DroidPlugin
һ�仰���ܣ�һ�����ŵĲ�����������
�ϰ����ɣ�4.8K��star���������ܰ񵥵�һ������360�Ŷӳ�Ʒ����������б�֤���гɹ���������360�ֻ����֣����ҳ���ά����
github https://github.com/DroidPluginTeam/DroidPlugin/blob/master/readme_cn.md
���ߣ�Andy Zhang
ʹ��:
clone��Ŀ������
 
53. otto
һ�仰����:һ���Ͼ���ǿ����¼����߿��
�ϰ����ɣ�4.8K��star����square�Ŷ������Ƴ����¼���Ӧ�Ϳ�ܣ��Ա�app���¼�����Ҳ�ǻ��ڴ˿�ܷ�װ�ģ����square�Ѿ����鿪���߲���RxJava RxAndroid������otto�ˡ���otto������EventBus����Աȵļ�ֵ��������˵��otto��square�Լҿ�����Rxϵ�п�ܵĲ���ͬ��ֵ�ÿ�������ȥ̽����
github https://github.com/square/otto
���ߣ�square
ʹ�ã�
repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }
}

compile 'com.michaelpardo:activeandroid:3.1.0-SNAPSHOT'
 

 
54.u2020
һ�仰���ܣ�һ���ṩDagger�ĸ߼���ѧʾ����app����������е��ƣ�
�ϰ����ɣ�4.7K��star��JakeWhartonǣͷ�����Ľ�ѧ��app������ʹ��Dagger�������߼���ܵ��÷�����չʾ��Dagger��ButterKnife��Retrofit��Moshi��Picasso��Okhttp��RxJava��Timber��Madge��LeakCanar���ڶ������ܽ�������ĸ߼��÷�����Ҳ���Խ�����Լ�����Ŀ����
github  https://github.com/JakeWharton/u2020
���ߣ�JakeWharton
 
 
55.buck
һ�仰���ܣ�buck��һ�����ٹ���ϵͳ
�ϰ����ɣ�facebook+google��������ߣ��Թ�������ĳ�ɫ��⣬���ϴ����Ŷӵ�ά�����Լ���������ʱ�Ŀ��ٸ�Ч����buck��Ϊ��΢��Android�Ŷӹ�����Ŀ����ѡ������������Ŀʱ������gradle���죬Ȼ����С��˾�����ʺϴ˿�ܣ�����Ϊ��־�ڿ�����������һ����Ϊ�����ǣ���ӭ��һ̽����
������ַ��https://buckbuild.com/
github  https://github.com/facebook/buck
���ߣ�facebook
ʹ�ã�
linux or mac system  +docs
 

 
56.PermissionsDispatcher
һ�仰���ܣ�һ�����ע����ṩ�������ʱΣ��Ȩ�޷����Ŀ��
�ϰ����ɣ���Android6.0 Google���Σ��Ȩ��һ�����û���ȫ�Ա��ᵽһ���ĸ߶ȣ�һЩ����ʱ���û���ΪΣ�յ�Ȩ�޽������Զ��������߻�ȡ����Ҫ�����û���׼�������߲ſ��Լ���ʹ�ø�Ȩ�ޣ������������Ȩ��������ץ�����������������������ܣ����㹻����������
������ַ��https://hotchemi.github.io/PermissionsDispatcher/
github https://github.com/hotchemi/PermissionsDispatcher
���ߣ�Shintaro Katafuchi
ʹ�ã�
���ƴ���
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
���ƴ���
 

57.android-gif-drawable
һ�仰����:һ���ṩչʾGIF������������ͼ���

�ϰ����ɣ����������������App����֪��ʹ����android-gif-drawable�����֤�������Ĵ��ڼ�ֵ�������ڰ񵥵�ʮһλ������lottie-androidֱ��Ӧ��AE������ʾ������AE���ʦ����ÿ����˾���䱸�ģ�GIF�Ĵ��ڣ��ͱ�Ȼ������չʾGIF����Ҫ����ֵ����ӵ�У�

github https://github.com/koral--/android-gif-drawable

���ߣ�Karol Wr��tniak

ʹ�ã�

���ƴ���
repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
}
dependencies {
    compile 'pl.droidsonroids.gif:android-gif-drawable:1.2.+'
}
���ƴ���
 

58.Apktool
һ�仰���ܣ�һ�����apk�Ĺ���

�ϰ����ɣ���Դ�ķ����빤�ߣ�����־���˽�apk�����ƽ����λ��ֵ��ӵ�У�4.5k��star�������ƽ�apk������

github  https://github.com/iBotPeaches/Apktool

������ַ��https://ibotpeaches.github.io/Apktool/

���ߣ�Connor Tumbleson

 

59.dynamic-load-apk
һ�仰���ܣ�������������

�ϰ����ɣ�4.5k��star��λ�ڲ����������ܵڶ�������һ������360�Ŷӣ���ȫ����ĵ���������ܿ�������ֲ���������������ϲ��������ֽ��⣬��ô�����Ŀһ���ʺ���

github��https://github.com/singwhatiwanna/dynamic-load-apk

���ߣ�singwhatiwanna

ʹ�ã�

github�ϵ��ĵ�������߲��͸���Ӵ

 

60.atlas
һ�仰���ܣ��Ա��Ƴ���������������

�ϰ����ɣ��Ա��Ŷ������ľ�Ʒ��atlas����ṩ�˽���������̬�Ŀ���������4.5k��star����λ�������������ܵ�һ��

github https://github.com/alibaba/atlas

���ߣ�alibaba

 

 61.volley
һ�仰���ܣ�google�Ƽ�ʹ�õ�Android������������

�ϰ����ɣ�4.4k��star�����������������㣬����ʹ��volley�Ѿ�������Ϊ��󿪷��ߵ�ϰ��

github https://github.com/google/volley���°�volley��ַ��

���ߣ�google

ʹ�ã�

cloneԴ�뵽����

 
62.androidmvp
һ�仰���ܣ�һ��չʾAndroid��Mvp��Ƶ�demo
�ϰ����ɣ�����Ϊ�����ࡢ��ƾչʾĳ�����ģʽ�ͻ��4.2K��star����Ŀ��������г���mvp�Ĵ��㣬androidmvp������Ϊ���ǰ��վ
github  https://github.com/antoniolg/androidmvp
���ߣ�Antonio Leiva
ʹ�ã�
clone������
 
63.SwipeBackLayout
һ�仰����:һ���������ͨ���������ƹر�ҳ��ĵĿ��
�ϰ����ɣ���΢�Ż����˳���ǰ��������Ч�����ṩ��activity�Ļ����ر�������ͨ������˼·��ʵ��fragment�Ļ����ر�����׾�;���߼�ֽ�����λcloneԴ�뵽����̽��һ����4.2k��star֤���ܶ��˶�ϲ����
github https://github.com/ikew0ng/SwipeBackLayout
���ߣ�ike_w0ng
 ʹ��:
compile 'me.imid.swipebacklayout.lib:library:1.0.0'
 

64.FlycoTabLayout
һ�仰���ܣ�һ��������������ֶ���ָʾ��Ч���Ŀ��

�ϰ����ɣ���������û������Ϊ�˸�app����ҳ��ָʾ�����ܾͼ���2.5M�������⣬������Ϊ�˽�viewpager��swip views��ָʾ�����ԭ��������ܣ���ֵ�ô������ԣ����߽��鵥���������Դ�룬���뵽�Լ�����Ŀ��ȥ��4.1K��star�����ο�������Ʒ����Ȼ�Ƽ���

github  https://github.com/H07000223/FlycoTabLayout

���ߣ�Flyco

 

65.android-testing
һ�仰���ܣ�һ��չʾ�Ĵ��Զ������Կ��������demo��Espresso��UiAutomator��AndroidJunitRunner��JUnit4��

�ϰ����ɣ�ѧϰ�߾����������ƶ��Ƕ��ľ��أ����������ѧϰ��Android Testing Support Library site�Ŀγ̣���ô��һ����android���Ĵ���Կ���Ȳ����������demo�ǳ��ʺ��㣬����ѧϰ���4.1k��star��������Ŀ��

github https://github.com/googlesamples/android-testing

���ߣ�googlesampes�Ŷ�

 

66.FileDownloader
һ�仰���ܣ�һ���Ч���ȶ��������õ��ļ���������

�ϰ����ɣ�4.1k֤�������ж�����ϲ�����ļ����ؿ��Ƽ򵥵ı��󰵲��˶��ٵĿӿӵ�㣬��֪�����������Լ�ʵ���ļ����ع��ܣ�������Ŀ�ܿ������������Ʊ�������������ܿ����������ʵ����

github https://github.com/lingochamp/FileDownloader

����:LingoChamp�Ŷ�

ʹ�ã�

dependencies {
    compile 'com.liulishuo.filedownloader:library:1.5.5'
}
 

 67.JieCaoVideoPlayer
һ�仰���ܣ�����MediaPlayer api����VideoView �Ķ�ý�岥�ſ��

�ϰ����ɣ�����������ý�岥�ſ�ܣ��������ɵ����˼��뱾�񵥣��������������ŵ㣬����100k��ӵ��������Ϳ��Կ��ٿ������ƽ���ͷ����������Ƶ����Ч����4k��star��֤����ֵ��һ��

github https://github.com/lipangit/JieCaoVideoPlayer

���ߣ�Nathen

ʹ�ã�
compile 'fm.jiecao:jiecaovideoplayer:5.5.4'
 

68.glide-transformations
һ�仰���ܣ�Ϊ�ڶ�����ͼƬ���ؿ���ṩͼƬ��״��������Ŀ��

�ϰ����ɣ��ڰ񵥿�ǰ�Ĳ����Ѿ����ܹ�glide��Picasso��Fresco��ͼƬ���ؿ�ܣ�glide-transformations����һ��Ϊ�����ṩͼƬ���������Ŀ�ܣ�ʹ�������ǳ��򵥣�����ܵ��˴�ҵ�ϲ����github����3.8K��star
github  https://github.com/wasabeef/glide-transformations
���ߣ�Daichi Furiya
ʹ�ã�
���ƴ���
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:glide-transformations:2.0.2'
    // If you want to use the GPU Filters
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1'
}
���ƴ���
��Glide�����ñ��Ч��

Set Glide Transform.

Glide.with(this).load(R.drawable.demo)
        .bitmapTransform(new BlurTransformation(context))
        .into((ImageView) findViewById(R.id.image));
 

69.android-gpuimage
һ�仰���ܣ�һ�����OpenGL��ͼƬ��Ⱦ����
�ϰ����ɣ�����GpuImage��IOSƽ̨��������̸��Android���android-gpuimage���ṩ���70����ͼƬ��ȾЧ�����㻹�ں�����ͼ���������ʵ��ͼƬ��õģ���������һ�ж��������⡣���������ͼ������Ĺ���ʦ���˿�ܵĽ���˼·Ҳ�����������档����Ҳ��ͨ��android-gpuimage��������ͼApp������Ů�ѷ��ĵģ��ٴ�Ϊ����ʵ�����ޡ�ios��+android��һ��19k��star���Ѿ�֤��������ʵ�������ڵ�ʲô�أ�
github��https://github.com/CyberAgent/android-gpuimage
���ߣ�CyberAgent �Ŷ�
ʹ�ã�
���ƴ���
repositories {
    jcenter()
}

dependencies {
    compile 'jp.co.cyberagent.android.gpuimage:gpuimage-library:1.4.1'
}
���ƴ���
����ĸ��췽��������Ҫ�Ķ�Ios�ı���ĵ���������������С���ǿ���Ƽ���

 
70.RxPermissions
һ�仰���ܣ�һ�����RxJava���Ȩ������Ŀ��
�ϰ����ɣ�����ڶ����ṩȨ����Ŀ�ܣ�����RxJava����ƣ��������ר��дҵ��3.7K��star�Ѿ�֤��������ʵ�ü�ֵ
github https://github.com/tbruyelle/RxPermissions
���ߣ�Thomas Bruyelle
ʹ�ã�
���ƴ���
repositories {
    jcenter() // If not already there
}

dependencies {
    compile 'com.tbruyelle.rxpermissions:rxpermissions:0.9.4@aar'
}
���ƴ���
 

���ŵ�ʹ�ã�
���ƴ���
RxPermissions rxPermissions = new RxPermissions(this); 

rxPermissions
    .request(Manifest.permission.CAMERA)
    .subscribe(granted -> {
        if (granted) { // I can control the camera now
        } else {
           // Oups permission denied
        }
    });
���ƴ���
 

71.freeline
һ�仰���ܣ�һ�̬�滻�ı��빹�����

�ϰ����ɣ���Facebook��Buck��Androdi�ٷ���InstRun֮�����Ͻ���Ƴ���Freeline�����ܣ���������Freeline��ҵ������������ʽ�����Ȼ���������ٶ�����;�������Ⱥ󣬱����ٶȲ����ڱ�������Ŀ��������У����freeline��3.7��star�����б����ܵڶ���

������ַ��https://www.freelinebuild.com/

github��https://github.com/alibaba/freeline

���ߣ�alibaba

ʹ�ã�

���ƴ���
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
File �� Settings... �� Plugins �� Browse repositories ��freeline.
���ƴ���
 

72.RxLifecycle
һ�仰���ܣ�һ���ṩ��ʹ��RxJava�����й���Activity��Fragment�������������Ŀ��

�ϰ����ɣ��ڰ񵥿�ǰ�Ĳ��֣����Ѿ��˽�RxJava��RxAndroid��ǿ��֮���������ִ��ĵĿ�������Ϊû�м�ʱȡ�����Ķ��������ص��ڴ�й©����Ҫ���ģ�RxLifecycle����Ϊ�������⣬��gtihub��ӵ��3.7K��star������֪���������֪�����Ա�Ҳ����ʹ����

github  https://github.com/trello/RxLifecycle

���ߣ�trello�Ŷ�

ʹ�ã�

cloneԴ�뵽����

 

73.classyshark
һ�仰���ܣ�һ���ִ���ļ������

�ϰ����ɣ������Apktool֮��ڶ���apk���򹤾ߣ������ϲ�����ŵ�ͼ������չʾ����ô��һ�����ܴ������classyshark���Խ��ƽ�Ľ����ͼ�λ�չʾ�û������������3.7K��star����������apk���򹤾ߵڶ�λ��

github  https://github.com/google/android-classyshark

���ߣ�google

ʹ�ã�

���� JAR 

 

74.acra
һ�仰���ܣ�һ���ṩ��¼APP������־�����Ŀ��

�ϰ����ɣ�������������ռ�APP������־��������ôacra�Ǹ������ѡ��3.7K��star����acraλ�б�����־������а��һ����acra���㹻��������¼����APP�����ҷ��ط���ˣ�acraҲ�ṩ���൱���ı�����־ͳ�Ʒ���˿��Acralyzer��cralyzer������Apache CouchDB֮�ϣ����Գ���CouchDB֮�⣬û�б�Ҫ��װ�κζ����������ƶ��˿�����Ҳ���Խ��ѧϰ����˵Ľ��裬һ�����ã�

github https://github.com/ACRA/acra

�����github  https://github.com/ACRA/acralyzer

���ߣ�acra�Ŷ�

ʹ�ã�

û��ʲô������cloneԴ�뵽���ظ�������

 

75.DiskLruCache
һ�仰���ܣ�һ���ṩ�����ļ�������������Ŀ��

�ϰ����ɣ�3.7k��star��������˵��DiskLruCache�����㣬�����Թ�������ļ����������������Ϊһ����ܣ�������Ҫ�ܴ�������������ˣ����������ˣ�����Ҳ��ΪGoogle�����ᳫ�Ļ���  ���绹�ǵ��ϴ�����һ��������桱�����鿴�����ļ���С��������ʲôʱ����DiskLruCacheһ�仰�Ϳ��Ը㶨��

github https://github.com/JakeWharton/DiskLruCache

���ߣ�JakeWharton

ʹ�ã�

 

compile 'com.jakewharton:disklrucache:2.0.2'
�������� latest .jar

 

76.dexposed
һ�仰���ܣ�һ��֧�Ű���󲿷�App�ͻ������޸������ϵ��������Ŀ��

�ϰ����ɣ������ٴγ������޸���ܵ���Ӱ��֤��App���޸������Ļ��ȣ�dexposed�ṩͼ�λ������ܼ�ء��������޸�bug©����֧��AOP���˼��ȣ�����������ҵ���޸�����������߻��Ǵ��������޸�����һ̽���������ˣ�����ܺ��ʺ��㡣3.5k��star��֤������Ϊһ�ż�����ܵĴ��ڣ��Ƕ�ô����ϲ����

github  https://github.com/alibaba/dexposed

���ߣ�alibaba

ʹ�ã�

dependencies {
        compile 'com.taobao.android:dexposed:0.1.1@aar'
    }
 

77.Litho
һ�仰���ܣ�һ���ṩ��Ч����UI�����Ŀ�� 

�ϰ����ɣ���Ϊһ��ר�Ź���UI�Ŀ�ܣ�Litho��Ч�ĵط����ڣ�����������������Ⱦ�Ͳ��ֵ��̣߳�Ȼ�󽫴����õ�������ݸ�UI�߳�ȥ������յ���Ⱦ��ʹ�ø��ٵ���ͼ�㼶������������Ĺ����ٶȣ�ֵ��ע����ǣ�����֧�ֿ������������ɸı��UI��� ,3.5K��star��֤�������ڹ���UI����ļ�ֵ�����������ڴ�������ȥ����

github  https://github.com/facebook/litho

���ߣ�facebook

 ʹ�ã�

���ƴ���
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
���ƴ���
 

78.mosby
һ�仰���ܣ�һ���ṩ����MVP��Ŀ�����Ŀ��

�ϰ����ɣ��񵥿�ǰ�Ĳ����Ѿ�������MVC,MVVM,MVP�Ŀ����Ŀ����ش�ʱ���ڹ�����ҵ��Ŀ�ܹ��ϣ�ѡ����߿���һ����ʵ�MVP�������ü�ޣ�mosby������Ϊ��ĵ�һ���ο�������Է�װ����Ҳ�����ճ�����������Σ�3.4K��star��֤�������ڿ��������ж��ܿ����ߵ�ϲ��

github https://github.com/sockeqwe/mosby

���ߣ�Hannes Dorfmann

ʹ�ã�

���ƴ���
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
���ƴ���
 

79.AndResGuard
һ�仰���ܣ�һ���ṩ��Դ�ļ�·������ �Ĺ���

�ϰ����ɣ�������Ǹ���APK��С�����е��ˣ���ôAndResGuardһ���ʺ��㣬����ԭ������Java Proguard������ֻ�����Դ�����Ὣԭ���߳�����Դ·����̣����罫res/drawable/wechat��Ϊr/d/a��3.4K��star��֤�������Ż�APK��·�ϣ��㲻��һ������ս����

github  https://github.com/shwenzhang/AndResGuard

���ߣ�wechat team

ʹ�ã�

clone��Ŀ�����أ���ʵҲ���Ǹ������仰���ĵ�

 

80.StatusBarUtil
һ�仰���ܣ�һ���ṩ���ó���ʽ״̬����ʽ�����Ŀ��

�ϰ����ɣ����ʦMM���Ǳ�Թϵͳ״̬�������ţ��Ǿ͸���һ�������ĳ���ʽ״̬����StatusBarUtil������������������״̬����ʽ��3.3K��star������˵�����ж������MM��ϲ��

github https://github.com/laobie/StatusBarUtil

���ߣ�Jaeger

ʹ�ã�

compile 'com.jaeger.statusbarutil:library:1.4.0'
 

81.robolectric
һ�仰���ܣ�һ�������Android�豸�ĵ�Ԫ���Կ�ܣ�

�ϰ����ɣ�sample���о�����ζ�Android�Ĵ�����ͳ������ܲ��Ե�������3.2K��star��ֵ�ó��������ĵ��˳���

������ַ��http://robolectric.org/

github  https://github.com/robolectric/robolectric

���ߣ�robolectric

ʹ�ã�

testCompile "org.robolectric:robolectric:3.3.2"
 

82.Fragmentation
һ�仰����:һ���ṩ����FragmenǶ��t�����Ŀ��

�ϰ����ɣ�����Activity��Fragmentʹ�ã���һ������Ӧ�֣������Ҫ��һ��ͨ�õ�Activity&FragmentǶ����ƣ�������е������޴��ˣ�Fragmentation������Ϊ�����Fragment�����ϵĵ�һ����3.2K��star��������Ϊ�е�������ʵ�ˣ���Ŀ������˵����Fragment�Ĺ�������������δ�ṩFragment&Activity�������ڡ�����ջ�Ĺ�����������˺���ֱ��Ӧ�õ���ҵ��Ŀ���У���Դ�뵱�е����˼·��ֵ�ñ�������λ�����ʰ�������������㣡

github��https://github.com/YoKeyword/Fragmentation

���ߣ�YoKey

ʹ�ã�

// appcompat v7���Ǳ����
compile 'me.yokeyword:fragmentation:0.10.7'
// �����ʹ��SwipeBack ������Ե�˳�Fragment/Activity���ܣ������������Ŀ�
// compile 'me.yokeyword:fragmentation-swipeback:0.10.4'
 

83.Small
һ�仰���ܣ����ɵĲ�������

�ϰ����ɣ���Ϊ�����ܰ񵥵��³�Ա��Small���ŵ������ɣ��ʺ���ΪС�ŶӵĲ������������3.1K��star����������˿ṷ���ֵ����������Ŷӵ�������������ǵ��Ŷ�����ʵʩ�����������Small�Ǹ������ѡ��

 ������ַ��http://code.wequick.net/Small/cn/cases

github  https://github.com/wequick/Small

���ߣ�wequick �Ŷ�

ʹ�ã�

���ƴ���
buildscript  {
    dependencies {
        classpath 'net.wequick.tools.build:gradle-small:1.2.0-alpha6'
    }
}

apply plugin: 'net.wequick.small'

small {
    aarVersion = '1.2.0-alpha6'
}
���ƴ���
 

84.JsBridge
һ�仰���ܣ�һ���ṩWebView��Javascriptͨ�������Ŀ��

�ϰ����ɣ��ÿ���ṩ��������H5ҳ�����ͨ��JS����App������������3.1K��star������ͨѶ��ʽ��ֵ��ÿһ��Web\Hybrid App�����߳���

gtihub https://github.com/lzyzsd/JsBridge

���ߣ�hi��ͷ��hi

ʹ�ã�

���ƴ���
repositories {
    // ...
    maven { url "https://jitpack.io" }
}

dependencies {
    compile 'com.github.lzyzsd:jsbridge:1.0.4'
}
���ƴ���
 

85.richeditor-android
һ�仰���ܣ�һ��ǿ��ĸ��ı��༭��� 

�ϰ����ɣ�2.8k��star�������һ��ΪTextView�ṩ��չ�����Ŀ�ܣ�����ʱ����Ҫ���������ܲ�֪����

github  https://github.com/wasabeef/richeditor-android

���ߣ�Daichi Furiya

ʹ�ã�

���ƴ���
repositories {
    jcenter()
}

dependencies {
    compile 'jp.wasabeef:richeditor-android:1.2.2'
}
���ƴ���
 

86.Transitions-Everywhere
һ�仰���ܣ�һ�������ȷʹ��Transitions API��Android ת������API���Ľ�ѧ����Ŀ

�ϰ����ɣ�����ܻ�δ���Թ�Android API��Transitions ��ܣ�������������ȴ�޷�������������Ķ�Ч�������ģ�Transitions-Everywhere������������һ������������ȫ������Transitions ��ǿ��֮��

github  https://github.com/andkulikov/Transitions-Everywhere

���ߣ�Andrey Kulikov

ʹ�ã�

dependencies {
    compile "com.andkulikov:transitionseverywhere:1.7.4"
}
 

87.android-viewbadger
һ�仰���ܣ��ܹ����ٵ�ΪAndroid ��ͼ���롰ѫ�¡������Ŀ��

�ϰ����ɣ����˵ѫ��һ��������İ������ô��ʾ�Ѷ�δ��������С�������Ϣ��һ�������һ����̫İ����������������λʵ�ʿ����о�������ΪĳЩitem����С����ǵ����󣬴����ĸ�λһ�����Ÿ���ʵ�ַ�����Ϊʲô���ܿ������ŵ�����أ�android-viewbadger���԰���ʵ�֣���Ȼ����ĳЩ����£�����Ҫ�߱��޸�Դ����������Է������MM������ֵ��ע����ǣ������Ŀ�Ѿ�����û�и����ˣ�

github https://github.com/jgilfelt/android-viewbadger

���ߣ�Jeff Gilfelt

ʹ�ã�

cloneԴ�뵽����

View target = findViewById(R.id.target_view);
BadgeView badge = new BadgeView(this, target);
badge.setText("1");
badge.show();
 

88.AndroidWiFiADB
һ�仰���ܣ�һ���������Ҳ������������ֻ��豸APP�Ĳ����Ŀ

�ϰ����ɣ����Ƿ��ڵ��Ĳ��Թ����и�ǿ�ȵİβ������߶��ֻ���غ�USB�˿�������������ֲ����𺦣����ģ���wifi��AndroidWiFiADB������������Ҳ���Ե���Ӧ���ˣ�����Ȥ���ǣ��ڲ��Թ���ʦһ�������ֻ�һ��������bug��ʱ�����Ѿ�͵͵�������ֻ����޸���bug����ع�������

github https://github.com/pedrovgs/AndroidWiFiADB

���ߣ�Pedro Vicente G��mez S��nchez

ʹ�ã�

Preferences/Settings->Plugins->Browse Repositories->serch AndroidWiFiADB
 

889.emojicon
һ�仰���ܣ�һ���ṩ��TextView��EdiTextչʾ����������Ŀ��

�ϰ����ɣ�2.7k��star��,�񵥵ڶ�����ǿTextView��ʾ�����Ŀ�ܣ����רΪ�������ƣ��������������΢�š�QQ�ı�����ʾ����������ģ������һ�������������֪����

 

90.packer-ng-plugin
һ�仰���ܣ�һ��򱬹��߲��

�ϰ����ã����߾���ά�����漰��Χ��ȫ���ԣ��������˲����Ŀ������Ŀ�ų����100��������ֻ��Ҫ10���ӣ��������ϸ��ָ�����������������Ľ��죬ѡ��һ���ʺ��Լ��Ŷӵģ���������ѡ��

github https://github.com/mcxiaoke/packer-ng-plugin

���ߣ�Xiaoke Zhang

ʹ�ã�

���ƴ���
buildscript {
    ......
    dependencies{
    // add packer-ng
        classpath 'com.mcxiaoke.gradle:packer-ng:1.0.9'
    }
} 
���ƴ���
 

���ƴ���
apply plugin: 'packer' 

dependencies {
    compile 'com.mcxiaoke.gradle:packer-helper:1.0.9'
} 

 android {
    //...
    signingConfigs {
      release {
          // ����������������ʱ��Ҫ������
          // 1. Gradle�汾 >= 2.14.1
          // 2. Android Gradle Plugin �汾 >= 2.2.0
          // ������ֻʹ�þɰ�ǩ��������V2��ǩ��ģʽ
        v2SigningEnabled false 
      }
    }
  }
���ƴ���
 

91.android-priority-jobqueue
һ�仰���ܣ�һ���ṩ��̨������������Ŀ��

�ϰ����ɣ�������Ǹ�־�������о����̲߳����Ŀ����ߣ������Ŀһ����Ҫ�����������Activity���¼��ء�Serviceʹ���̳߳�ʱ���������ȼ��Ͳ������⣬����Ҫ���ģ�Job Manage���չ����ȼ����־��ԣ�����ƽ�⣬�ӳ٣�������ƣ����飬2.4K��star������Ķ��̹߳��������������������ĵ�������ܺ��٣�ֵ����һ��

github  https://github.com/yigit/android-priority-jobqueue

���ߣ�Yigit Boyar

 

92.Android-Debug-Database
һ�仰���ܣ�һ���ṩ����App�ڲ����ݿ������Ŀ��

�ϰ����ɣ�����ڶ�����Ե������ݿ�Ŀ�ܣ�һ�д��뼯�ɣ�ֱ�����������ɾ�Ĳ�App�����ݿ⣬2.3k��star���Ķ������ж���

github  https://github.com/amitshekhariitbhu/Android-Debug-Database

���ߣ�AMIT SHEKHAR

ʹ�ã�

debugCompile 'com.amitshekhar.android:debug-db:1.0.0'
���������

 http://XXX.XXX.X.XXX:8080
 

93.conceal
һ�仰���ܣ�һ��facebook�ṩ�ļ��ܱ��ش��ļ��Ŀ��

�ϰ����ɣ�������ڵ���App�ڵ�ͼƬ����˽���⣬���facebook�ṩ���ļ����ܿ�����Խ��������⣬facebook�ͻ��˵�ͼƬ�����ݶ���ʹ��conceal���ܵ�

������ַ��http://facebook.github.io/conceal/

github https://github.com/facebook/conceal

����;facebook

ʹ�ã�

clone��Ŀ������/��������jar

 

94.ARouter
һ�仰���ܣ�һ���ṩ����ҳ����ת·�ɵĿ��

�ϰ����ɣ������������Ƶ��������ÿ���ṩ�����ⲿURLӳ�䵽�ڲ�ҳ�桢��ģ���ҳ����ת��ҳ������������ת���̵����������и��๦�ܵ���ȥ����2.1K��star��ֵ��Ϊ��ҵ���Ŀ�ܺȲ�

github  https://github.com/alibaba/ARouter

���ߣ�alibaba 

ʹ�ã�

���ƴ���
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
    // �滻�����°汾, ��Ҫע�����api
    // Ҫ��compilerƥ��ʹ�ã���ʹ�����°���Ա�֤����
    compile 'com.alibaba:arouter-api:x.x.x'
    annotationProcessor 'com.alibaba:arouter-compiler:x.x.x'
    ...
}
// �ɰ汾gradle���(< 2.2)������ʹ��apt��������÷�������ĩ'����#4'
// Kotlin���òο���ĩ'����#5'
���ƴ���
 

95.MagicaSakura
һ�仰���ܣ�һ���ṩ�������л������Ŀ��

�ϰ����ɣ�������ṩ��������һֱ�Ǳ��������صģ������bilibili�ṩ�Ķ������ܣ���Ϊ�����漰��Χ�ܲ��䣬1.9��star����лbilibili�Ŷ��������Ĺ��ף�

github https://github.com/Bilibili/MagicaSakura

����:Bilibili

ʹ�ã�

compile 'com.bilibili:magicasakura:0.1.6@aar'
 

96.CustomActivityOnCrash
һ�仰���ܣ�һ�APP crash��ʱ���Զ�����ĳ��Activity�Ŀ�ܣ���������ʾUnfortunately, X has stopped��

�ϰ����ɣ�����Ĵ����ǰ�����Ҫ�ģ�������Ӯ����1.8K��star����Ϊ������Ӧ��ӵ�п��ǵ�����Ǳ����bug�������������ǲ�����������㵽������ϵͳ�˵�ͬ��Ҳ������ɳ��������crash����ˣ�����ó������ŵ�crash->����ֵ������˼��������ܾ��ṩ����������

github  https://github.com/Ereza/CustomActivityOnCrash

���ߣ�Eduard Ereza Mart��nez

ʹ�ã�

dependencies {
    compile 'cat.ereza:customactivityoncrash:2.1.0'
}

��ӵ� Application class:
���ƴ���


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
���ƴ���
 

 

97.XhsEmoticonsKeyboard
һ�仰���ܣ���ĵĿ�Դ����������

�ϰ����ɣ�����㻹�ڷ������Ϊ���APP���Ƽ��̣���ô�˿�ܷǳ��ʺ��㣬���һ��ṩ�����չʾ������1.7��star֤�������Ķ��ء��������߻������˸߷�΢�ż��̣�QQ���̵�demo���������λ

github https://github.com/w446108264/XhsEmoticonsKeyboard

���ߣ�zhongdaxia

ʹ�ã�

���ƴ���
allprojects {
    repositories {
        jcenter()
        maven { url "https://jitpack.io" }
    }
}


dependencies { 
    compile 'com.github.w446108264:XhsEmoticonsKeyboard:2.0.4'
}
���ƴ���
 

 

��.������Ŀ
1.iosche
һ�仰���ܣ��ȸ�2016�����ߴ���չʾ��Ŀ

�ϰ����ɣ�github����13.4k��star��λ����ҵ����Ŀ���а��һλ��ţ�ƵĿ����ߣ�Ȩ�������ģʽ����׼����Ŀд����ֵ��һ�ԣ����߽����ѧ��down��Դ�룬�ҵ�app��ڣ�ÿ��ҳ����һͨ��������ģʽ�ĸ��������⡣

github https://github.com/google/iosched

���ߣ� Google

 

2.Plaid
һ�仰���ܣ��ṩ������ź���еĿ�Դapp

�ϰ����ɣ���׼��material design��ƣ�������app��github��9k��star��ֵ�������������ϲβ�������app����������о����ɣ�

github  https://github.com/nickbutcher/plaid

 ���ߣ� Nick Butcher

 

3.PocketHub
һ�仰���ܣ�Github��Android��

�ϰ����ɣ�8.7K��star������Github���������ӣ����ŵ�Դ��ֵ�ø�λһ̽����

github https://github.com/pockethub/PocketHub

����:Fadil Sutomo

ʹ�ã�

down������Դ��

 

4.Signal Android
һ�仰���ܣ�Signal��һ�ȫͨѶ�Ķ�����app��

�ϰ����ɣ�7.9K��star������������app�ı�ǩ���ԣ����������а��ж�һ�޶��������Զ���app����Ȥ����������̽��һ��

github https://github.com/WhisperSystems/Signal-Android

���ߣ�WhisperSystems

ʹ�ã�github��downԴ��

 

5.android-UniversalMusicPlayer
һ�仰���ܣ�һ����豸���еĶ�ý��app

�ϰ����ɣ�googlesamples�����Ƽ���githubӵ��7.9k��star��������Android�ֻ���������ƽ�壬�����豸��ʹ�ã����ڽ��������Android�ֻ������ĳ���Ա���᲻��������أ���ֵ��һ�ԣ�

github https://github.com/googlesamples/android-UniversalMusicPlayer

���ߣ�Google

ʹ�ã�github��downԴ��

 

6.HomeMirror
 һ�仰���ܣ�������Ǹ������ļһ���ô��һ����Ҫ���澵�ӣ�

�ϰ����ɣ�������App������github����һϯ֮�أ��������ṩ�ر�����Ĺ��ܣ�����HomeMirror��github������7599��star��������Ϊ���ṩ�˾��ӵĹ��ܡ���������Android �ֻ���pad��������Ϊ�����ξӼ�������ֵ��ӵ�У�

github  https://github.com/HannahMitt/HomeMirror

���ߣ�Hannah Mittens 

HomeMirror�����飺



 

7.ExoPlayer
һ�仰���ܣ�һ�� ���Androidԭ��MediaPlayer��ý�岥����

�ϰ����ɣ�Ҳ����Google���Լ�MediaPlayer API�������⣬���Ե�����ExoPlayer��ExoPlayer�ṩ��ǿ�����չAPI��ʹ������������ý�岥��������ݣ���������չ���Զ�ý�岥��������Ȥ��ͬ���ǿ�����������չ�����ˣ�6.9K��star��֤�����ж��ܿ�������ϲ���������ܿɹ���ǣ�google���ڸ���ά���ţ�

������ַ��https://google.github.io/ExoPlayer/

github  https://github.com/google/ExoPlayer

���ߣ�google

ʹ�ã�

���ƴ���
repositories {
    jcenter()
}
compile 'com.google.android.exoplayer:exoplayer:r2.X.X'

compile 'com.google.android.exoplayer:exoplayer-core:r2.X.X'
compile 'com.google.android.exoplayer:exoplayer-dash:r2.X.X'
compile 'com.google.android.exoplayer:exoplayer-ui:r2.X.X'
���ƴ���
 

8.cheesesquare
һ�仰���ܣ�Android ������Ƶ�չʾ����Ŀ

�ϰ�����:���߱���Ϊ��Android Support Lib��������ˣ���д����չʾ����Ŀ�����ܲ��Ƽ��ϰ񣿲�������Ѿ����˺ü����ˣ�����Ϊ��Ȩ����չʾ��Ŀ����һ����Ҫ����6.7��star֤�������Ƕ�ô���ܻ�ӭ��

github  https://github.com/chrisbanes/cheesesquare

���ߣ�Chris Banes

 

9.DanmakuFlameMaster
һ�仰���ܣ�android�˿�Դ��Ļ����

�ϰ����ɣ�bilibili��Ʒ����֤�����Ĵ���Ʒ�ʣ�����ndkԴ��Ҳһ����Դ����νҵ�����ģ��õ�Ļ����Ŀ�Դ��ʡ�˺ܶ���Ƶֱ��С���Ŀ����ɱ�������ǿ���Ƽ���

github https://github.com/Bilibili/DanmakuFlameMaster

���ߣ�bilibili

ʹ�ã�

���ƴ���
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
���ƴ���
 

10.facebook-android-sdk
 һ�仰���ܣ�һ���ṩ����facebookƽ̨�����Ŀ��

�ϰ����ɣ����������н���facebook�����󣬻�����ѧϰ����sdk�������ⶼ�Ǻܰ���;������ο���һ����ҵ��sdk���ǽ������㿪������ʦ�ı���֮·��4.1k��star��facebook�־ø���������֤����ֵ��ӵ�У�

github https://github.com/facebook/facebook-android-sdk

���ߣ�facebook

ʹ�ã�

 https://developers.facebook.com/docs/android
 

11.android-oss
һ�仰���ܣ����ⴴ������Kickstarter ��Դ��Android��ͻ���

�ϰ����ɣ����µ���ҵ��APP��ÿ��ҳ�洦��ö��ܰ��������־�ڳ�Ϊһ�����Ź���ʦ����Դ��Ŀһ���ʺ��㣬3.8k��star֤���������׵�������

github��https://github.com/kickstarter/android-oss

���ߣ�kickstarter

ʹ��;

cloneԴ�뵽����

 

12.k-9
һ�仰���ܣ�Android�˿ͻ����ʼ�App

�ϰ����ɣ����ǵ���С���ĳ���������FoxMail�����������һ���ƶ���Email App��k-9���кܺõĽ����ֵ���������Ӧ�ò�Э����Ҳ���и������ʶ

������ַ�� https://k9mail.github.io/

github  https://github.com/k9mail/k-9

ʹ�ã�

clone��Ŀ������

 

13.Timber
һ�仰���ܣ�һ�����ֲ�������App

 �ϰ����ɣ�3K��star����ȫ���ղ�����ƹ淶���ṩʮ���ֲ������ԣ����һ��ṩApp��ͨ��������������һ������ͬ�����㣬����־����������������ͬѧֵ��һ��

github https://github.com/naman14/Timber

���ߣ�Naman Dwivedi

ʹ�ã�

cloneԴ����һ����ϰ��

 

14.remusic
һ�仰���ܣ�������������Android��App

�ϰ����ɣ�ѧϰ��Timer���Ƿ񻹲�̫�������θ�ڣ�remusic�����������θ�ڡ���������������ȥֱ�ӵ�������Ŀ�ˣ�2.9K��star������Timber����ƣ����ֵ�ǰ�����ȸ㶮Timber��ֵ�����֣���һ�����⣺��������ع������������أ�

github https://github.com/aa112901/remusic

���ߣ�MW

ʹ�ã�

clone��Ŀ

 

15.Douya
һ�仰���ܣ���Դ����ͻ���

�ϰ����ɣ�һ���ȫ�桢�ܹ���Ʋ��׵Ŀ�ԴAPP�������ǶԶ���APP���˼·���������е��ع���Ŀ���ɼ����߶Բ�Ʒ�ĳ��Ժ��Ȱ���2.9K��star��֤������Ŀ������ͷ�Է���һʱ�������Ʒ�����ÿһ��idea����ʵ�֣������ǵ����罫���ô���

github  https://github.com/DreaminginCodeZH/Douya

���ߣ�Zhang Hai

ʹ�ã�

clone��Ŀ������

 

16.BookReader
һ�仰���ܣ���ԴС˵�Ķ���

�ϰ����ɣ�2.7K��star�������һ���Ķ���APP�����кܸߵ�ѧϰ��ֵ���������Ȥ���Ķ������෽��չ��ͬѧ��

github https://github.com/JustWayward/BookReader

���ߣ�JustWayward �Ŷ�

ʹ�ã�

clone������ 

 

17.bilibili-android-client
һ�仰����:�߷�bilibili��Android�ͻ���

�ϰ����ɣ�2.5K��star�������һ����Ƶֱ����ԴApp���ʺ϶���Ƶֱ����������������Ȥ��ͬѧ��bilibili-android-client��ʹ���˺ܶ���Ϳ�ܣ�����Ŀ�����ʺϻ���������ͬѧ����Ҫ���ģ�ѧϰҳ��Ĳ������Ҳ��ֵ�õģ�

github  https://github.com/HotBitmapGG/bilibili-android-client

���ߣ�Hcc

ʹ�ã�clone������

 

18.AndroidChromium
һ�仰���ܣ�Android��chrome�����

�ϰ����ɣ������������Ƶ�����:

�ȸ��������׿��Դ����Ŀ
���缶�İ�׿�ܹ�
���屾��Ŀҵ���߼���ȫ����ʤ�ι���һ�߹�˾����ʦ
��������־�������������ܵ��㣬ֵ��ӵ��

github https://github.com/JackyAndroid/AndroidChromium

���ߣ�JackYAndroid

ʹ�ã�

cloneԴ�뵽����

��.������ܣ�
���������Ⱥ�ֻ�����ͻ��֣�
1.libgdx
һ�仰���ܣ�һ���ƽ̨��android����Ϸ�������

�ϰ����ɣ�android�˿���������һ����11.7K��star������Ϸ���������ר����ǩ������Ҫ�������ǿ�ƽ̨��

������ַ  http://libgdx.badlogicgames.com/

github https://github.com/libgdx/libgdx

2.xUtils
һ�仰���ܣ�������ҵ���������

�ϰ����ɣ�4.9K��star��xUtils��Ϊ�Ϲ�ʱ�ڳ���Ա�����Ƴ�Ŀ�����ܣ�����ԭ�򡪡�ʡ�¡�xUtls�����Ĵ�ģ�飬��֮���������ṩ�Ĵ�������������ݲ�����UI������HttpЭ�������ͼƬ������xUtils��Ϊ���߳�ѧAndroid�����Ƶĵ�ʦ����Ŀ���ڱ��߶��꾭���У�����xUtils��Ϊ�ڶ���С����Android�˿�ܷ�����ѡ������֤�������ܻ�ӭ�̶ȡ��ÿ�������Ѿ����µ���xUtils3��������Android����漰��һ�����뷨�����Դ�xUtils���֣�����Ϊ��ܴ�ʦ���С���Ȼ����кܶ������Ѿ���ʱ������ģ�����������������������������xUtils��Ϊ���ڿ����ߵĽ������Ϲ�ʱ�ڵĿ�ܳ����ֵ����ӵ�У�

github  https://github.com/wyouflf/xUtils

���ߣ�wyouflf

ʹ�ã�

compile 'org.xutils:xutils:3.5.0'
3.android-common
һ�仰���ܣ� һ��android���ٿ������

�ϰ����ɣ��ε����Android����ʦ��Ʒ���������꿪���ߵļ��飬��4.3K�����ڿ��ٿ�����ܰ���������ÿ���ṩ��ͼƬ���桢Http���桢DropDownListView������ģ�顢�������ù�����ȣ���Ϊ�Ϲ�ʱ�ڳ���Ա������ܽ��Կ�����ܣ�����һ�����ǻ۵Ľᾧ��ֵ������Ϊ����Trinea���ƺȲ�

github  https://github.com/Trinea/android-common

���ߣ�Trinea

ʹ�ã�

clone���뵽����

4.Vitamio
һ�仰���ܣ�һ��֧�ֿ�ƽ̨��Android��ý�忪�����

�ϰ����ɣ����֮ǰ�ᵽ��exoplayer���������㿪����ý����������ұ�֤vitamioֵ����һ��

������ַ��https://www.vitamio.org/

github https://github.com/yixia/VitamioBundle

���ߣ�yixia�Ŷ�

ʹ�ã�

cloneԴ�뵽����

 

5.Weex
һ�仰���ܣ��ƶ��˿�ƽ̨�����Ľ������

�ϰ����ɣ�14.4K��star���г���Ӧ�ð�������ҵ����Ͽ�����ܣ�����Ͱͳ�Ʒ��Ϊʲô�������أ�

������ַ��https://weex.apache.org/cn/

github  https://github.com/alibaba/weex

���ߣ�alibaba

 

6.cordova-android��Hybrid ������ܡ�WebApp������ܣ�
һ�仰���ܣ���ƽ̨�Ŀ������

�ϰ����ɣ�cordova���㹻��������ɻ�Ͽ�����WebApp���������󣺲�������Web�����ߣ�������Native�����ߣ�ʹ��cordova������������ƽ̨��App 

������ַ��http://cordova.axuer.com/docs/zh-cn/latest/guide/overview/index.html

github https://github.com/apache/cordova-android

 

7.react-native
һ�仰���ܣ�һ����Javascript���������������ϵͳ���ԣ�Ios��Android���Ŀ��

�ϰ����ɣ����ѽ�react-native����ʲô������ʺ�ǰ�˹���ʦ�����ƶ���App��Ҳ�ʺ�Native�����߽��п�ƽ̨�Ŀ�����������Navitve��������˵���͵�ѧϰ���߻�����һ��������ܰ����ߡ���ǰ�˽���һ�����ԣ�Web������δ����Native���������ڣ������Ǵ���������δ���ĵ�·�ϣ�49K��star���ƺ���������δ������һ��

������ַ�� http://facebook.github.io/react-native/docs/getting-started.html

github  https://github.com/facebook/react-native

���ߣ�facebook 

 

��.������
1.AndroidUtilCode
һ�仰���ܣ��ṩ�������Ӵ�Ĺ�����

�ϰ����ɣ�10.8K��star����������֤�����Ƕ�ô�ܻ�ӭ����ӭ���ṩ���õĹ�����׳������

github https://github.com/Blankj/AndroidUtilCode/blob/master/README-CN.md

 

File �� Settings... �� Plugins �� Browse repositories...
and search for freeline.

 

2.kotiln
һ�仰���ܣ�Google�Ƴ���Android�������

�ϰ����ɣ�����AndroidStudioȡ��Eclipse������Goolg��kotiln��ΪAndroid�Ĺ������ԣ�Ҳ����Ϊ�˱���ͬOracle��ר�����ϣ���kotlin 100%����java���������java���������Լ�����ʽ��̵�˼����Щ���������ͬ��ֵ������ע�⣬���ǵ��ڰ�֮ǰ˵������δ����kotlin�ģ�������java�ģ������Ǵ��ڵ���ͨ��δ���ĵ�·�ϡ���ѧϰδ���ı�����ԣ������Լ��Ĺ���Ч�ʣ�����°�򶹶������ֶ���Ϊ��

������ַ��http://kotlinlang.org/

github��https://github.com/JetBrains/kotlin

 ʹ�ã�

http://kotlinlang.org/docs/reference/   �ṩ�� api-android����-�鼮����Դ

 

 

��.�鼮����Ŀ
���������Ⱥ�
1.Android developer�й�������ѵ�γ�
һ�仰���ܣ������й������Google�����߹������Ӳ�Ʒ����Android�����߹���

�ϰ����ɣ���������ѵ�γ̡�API�����γ̡�Sample��������������ܡ�AndroidStudio����...�ȵ�һϵ�й�����ѵĿγ̣����ܴ󲿷����ݻ���Ӣ�Ľ��⣬������Ͽ���Ӣ��ʵ�һƪһƪ���꣬�����ң����Android֪ʶˮƽ����ɱ���������ϴ󲿷ֵ�Android�鼮

������ַ��https://developer.android.google.cn/training/index.html

���ߣ�google

 

2.android-architecture
һ�仰���ܣ�google�ṩ��Android���¸��ֻ������

�ϰ����ɣ���������mvp��mvvm�������йϿ��ˣ����ɨ��Ҷһ��...

github https://github.com/googlesamples/android-architecture

���ߣ�google

 
3.andorid-open-project
һ�仰���ܣ�����Android�������еĿ�Դ��Ŀ�ĵ�����Ŀ¼

�ϰ����ɣ�23k��star�ĵ�����Ŀ¼������ʢ���������ǣ�����Ŀ�ĵ���������Ķ��������ķǳ��������ǲ֮���Ķ����Ƽ����ɡ����й���������ȫ��Android ��Դ��Ŀ����Ŀ¼

github https://github.com/Trinea/android-open-project

���ߣ�Trinea

 

4.awesome-android-ui
һ�仰���ܣ�Android�Ŀ�Դ��ĿĿ¼

�ϰ����ɣ������һ���Ŀ¼��23k��star

github  https://github.com/wasabeef/awesome-android-ui