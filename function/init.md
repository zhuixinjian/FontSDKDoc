#初始化

1. (必须)项目Application onCreate方法中初始化

    ```ruby
    FontCenter.initFontCenter(application, app_key, parameter);
    ```

2. (可选)设置自定义下载目录，默认在字体管家路径下：/sdcard/font，缓存路径：
/sdcard/font/cache

    ```ruby
    FontCenter.getInstance().setFolder_font(String path)
    ```

3. 在程序的入口activity中的

    ```php
    //onCreate方法中调用
    FontCenter.getInstance().init();

    //onDestroy中调用
    FontCenter.getInstance().recovery();
    ```

