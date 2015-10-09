#初始化

1. (必须)项目Application onCreate方法中初始化

    ```ruby
    FontCenter.initFontCenter(application, app_key);
    ```

2. (必须)在程序的入口activity中的onCreate方法中调用

    ```php
    FontCenter.getInstance().init();
    ```
3. (可选)设置自定义下载目录，默认路径: /sdcard/yiziyun，缓存路径: /sdcard/yiziyun/cache

    ```ruby
    FontCenter.getInstance().setFolder_font(String path)
    ```
