# 字体下载

1. **下载路径**

    1. 无下载地址的下载接口（跳转到字体管家下载，Activity中重写onActivityResult
接口，并在接口中调用以下方法，当在字体管家下载完成返回到当前应用时，
会回调OnResult接口）
    ```
    FontCenter.getInstance().getFontFromFontManager(String fontid,Activity activity,
                                                        OnResult result);
    ```

    2. 有下载地址的下载接口

        a) 直接下载apk
        ```
        FontCenter.getInstance().downloadFont(FontDownloadCallBack callback, Font font, Context ctx);
        ```

        b) 跳转谷歌市场下载字体
        ```
        FontCenter.getInstance().downloadFont(Font font, Context context);
        ```

2. **下载任务控制**
    1. 暂停下载任务
    ```
    FontCenter.getInstance().stopDownloadFont(Font font);
    ```
    2. 暂停所有下载任务
    ```
    FontCenter.getInstance().stopAllDownloadFont();
    ```
    3. 取消下载任务
    ```
    FontCenter.getInstance().cancelDownloadFont(Font font);
    ```
    4. 取消所有下载任务
    ```
    FontCenter.getInstance().cancelDownloadFontAll();
    ```

3. 获取字体预览文件接口
    ```
    FontCenter.getInstance().getThumbnail(humbnailCallBack callback,Font font);
    ```
4. 获取本地已经下载字体列表
    ```
    //此列表中的字体如果已下载, 字体对象中的isDownloaded字段为true, 需传入一个在线字体的集合)
    FontCenter.getInstance().getDownloadedFonts();
    ```

6. 判断字体是否在下载中
    ```
    FontCenter.getInstance().isDownloading(Font font);
    ```
