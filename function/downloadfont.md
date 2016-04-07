# 字体下载

1. **下载字体**

    1. 直接下载
     ```ruby
    FontCenter.getInstance().downloadFont(FontDownloadCallBack callback, Font font);
    ```
    2. 跳转谷歌市场下载字体包（字体包功能专用）
    ```ruby
    FontCenter.getInstance().downloadFonPack(Font font);
    ```

2. **下载任务控制**

    1. 暂停下载任务
    ```ruby
    FontCenter.getInstance().stopDownloadFont(Font font);
    ```
    2. 暂停所有下载任务
    ```ruby
    FontCenter.getInstance().stopAllDownloadFont();
    ```
    3. 取消下载任务
    ```ruby
    FontCenter.getInstance(Context context).cancelDownloadFont(Font font);
    ```
    4. 取消所有下载任务
    ```ruby
    FontCenter.getInstance().cancelDownloadFontAll();
    ```

3. **获取本地已经下载字体列表**
    ```ruby
    FontCenter.getInstance().getDownloadedFonts();
    ```
4. **删除字体**
    ```ruby
    FontCenter.getInstance().deleteFont(Font font);
    ```
5. 获取字体预览文件接口
    ```ruby
    FontCenter.getInstance().getThumbnail(ThumbnailCallBack callback,Font font);
    ```

