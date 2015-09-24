# 字体下载

1. **下载字体**

    1. 直接下载
     ```
    FontCenter.getInstance().downloadFont(FontDownloadCallBack callback, Font font, Context ctx);
    ```
    2. 跳转谷歌市场下载字体包（字体包功能专用）
    ```
    FontCenter.getInstance().downloadFonPack(Font font, Context context);
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

3. **获取本地已经下载字体列表**
    ```
    FontCenter.getInstance().getDownloadedFonts();
    ```
4. **删除字体**
    ```
    FontCenter.getInstance().deleteFont(Font font);
    ```
5. 获取字体预览文件接口
    ```
    FontCenter.getInstance().getThumbnail(humbnailCallBack callback,Font font);
    ```

