# 字体列表功能

1. 获取分类列表
    ```
    FontCenter.getInstance().getCateListFromServer(IHttpCallBack callback, String country)
    ```
2. 获取单个分类详细数据列表
    ```
    FontCenter.getInstance().getCateFontListFromServer(IHttpCallBack callback,String id)
    ```
5. 根据字体id获取Font对象
    ```
    //可通过Font.getTypeface()获取Typefaced对象，如果字体没下载，typeface为null
    FontCenter.getInstance().getFontById(String id);
    ```

3. ~~获取字体列表（下面这些方法已经过时，我们不建议使用了）~~

    1. ~~获取最新字体列表~~
    ```
    FontCenter.getInstance().getNewestFontListFromServer(IHttpCallBack callback)
    ```
    2. ~~获取最热字体列表~~
    ```
    FontCenter.getInstance().getHottFontListFromServer(IHttpCallBack callback)
    ```
