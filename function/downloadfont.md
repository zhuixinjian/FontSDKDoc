# 字体下载

1. **下载字体**

    1. 直接下载
     ```ruby
    FontCenter.getInstance(Context context).downloadFont(FontDownloadCallBack callback, Font font, Context ctx);
    ```
    2. 跳转谷歌市场下载字体包（字体包功能专用）
    ```ruby
    FontCenter.getInstance(Context context).downloadFonPack(Font font, Context context);
    ```

2. **下载任务控制**

    1. 暂停下载任务
    ```ruby
    FontCenter.getInstance(Context context).stopDownloadFont(Font font);
    ```
    2. 暂停所有下载任务
    ```ruby
    FontCenter.getInstance(Context context).stopAllDownloadFont();
    ```
    3. 取消下载任务
    ```ruby
    FontCenter.getInstance(Context context).cancelDownloadFont(Font font);
    ```
    4. 取消所有下载任务
    ```ruby
    FontCenter.getInstance(Context context).cancelDownloadFontAll();
    ```

3. **获取本地已经下载字体列表**
    ```ruby
    FontCenter.getInstance(Context context).getDownloadedFonts();
    ```
4. **删除字体**
    ```ruby
    FontCenter.getInstance(Context context).deleteFont(Font font);
    ```
5. 获取字体预览文件接口
    ```ruby
    FontCenter.getInstance(Context context).getThumbnail(ThumbnailCallBack callback,Font font);
    ```

