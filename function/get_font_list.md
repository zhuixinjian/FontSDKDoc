# 获取字体列表
[country_code]: /fontsdk/other/country_code.html

1. 获取分类列表
    1. 分类中包含字体
```ruby
    FontCenter.getInstance().getCateListByLanguage(IHttpCallBack callback, String country)
    ```
    2. 分类中不包含字体
    ```ruby
    FontCenter.getInstance().getCateListFromServer(IHttpCallBack callback, String country)
    ```
2. 获取字体列表

    1. 获取单个分类中的字体
    ```ruby
    FontCenter.getInstance().getCateFontListFromServer(IHttpCallBack callback,String id)
    ```
    2. 获取国家下所有字体 [国家代码对应表][country_code]
    ```ruby
    FontCenter.getInstance().getAllFontListByLanguage(IHttpCallBack callback, String country)
    ```
    3. 根据字体id获取Font对象
    ```php
    FontCenter.getInstance().getFontById(String id);
    ```
4. ~~获取字体列表（下面这些方法已经过时，我们不建议使用了）~~

    1. ~~获取最新字体列表~~

    ```ruby
    FontCenter.getInstance().getNewestFontListFromServer(IHttpCallBack callback)
    ```
    2. ~~获取最热字体列表~~

    ```ruby
    FontCenter.getInstance().getHottFontListFromServer(IHttpCallBack callback)
    ```


