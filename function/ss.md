# 主题包功能(根据客户需求提供服务)

1. 获取分类列表
    ```
    FontCenter.getInstance().getCateListFromServer(IHttpCallBack callback, String country)
    ```
2. 获取单个分类详细数据列表
    ```
    FontCenter.getInstance().getCateFontListFromServer(IHttpCallBack callback,String id)
    ```
3. 根据字体id获取Font对象
    ```
    //可通过Font.getTypeface()获取Typefaced对象，如果字体没下载，typeface为null
    FontCenter.getInstance().getFontById(String id);
    ```
4. 如何获取字体包

