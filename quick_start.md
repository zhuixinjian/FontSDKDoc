# 快速开始

[registurl]:http://www.zitiguanjia.com/signup
[demojar_download]:http://doc.zitiguanjia.com/public/file/sdkfile/fontsdk(jar+demo).zip
[jar_download]:http://doc.zitiguanjia.com/public/file/sdkfile/fontsdk.jar
[font_list]: /fontsdk/function/get_font_list.html
[download_font]: /fontsdk/function/downloadfont.html
[cloud_font]: /fontsdk/function/sd.html
[font_pack]: /fontsdk/function/ss.html
[use_font]: /fontsdk/function/use_font.html

1. 获取AppKey

    1. [注册易字云][registurl]并登录后台管理界面

    2. 创建应用

    3. 获取AppKey，测试appkey：`xIxj48w2ho-0cjiQK_yE`

2. 下载SDK

    [易字云SDK (Demo+jar)][demojar_download]

    [易字云SDK (jar)][jar_download]
3. 配置manifest

    添加下列权限到项目Mainfest文件

    ```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
<uses-permission android:name="android.permission.READ_PHONE_STATE" />
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
```
4. 初始化

    1. (必须)项目Application onCreate方法中初始化

    ```ruby
    FontCenter.initFontCenter(String appKey, Context applicationContext);
    ```

    2. (必须)在程序的入口activity中的

    ```php
    //onCreate方法中调用
    FontCenter.getInstance().init();
    ```
5. [获取字体列表][font_list]

6. 选择集成的功能

    1. [字体下载功能][download_font]

    2. [云字体功能][cloud_font]

    3. [字体包功能][font_pack]

7. [使用字体][use_font]
