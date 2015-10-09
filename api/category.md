# category

本接口用于获取客户在SDK后台配置的字体分类列表

```php
接口url : http://cdn5.xinmei365.com/cdndata/sdkapi/appcategory

请求方式: GET

参数:
    app_key : 字符串，客户app唯一识别码， 后台可以看到
    country : 字符串，客户国际化配置，根据不同国家获取不同分类，参数请见附录3.2

返回格式: json

返回示例:
    {
        "error_code": "0", //错误码，成功为0
        "error_msg": "success", //错误信息， 成功为success
        "data": [
            {
                "id": 1, //分类id
                "name": "分类1", //分类名称
                "previewurl": "http://upaicdn.xinmei365.com/sdkimg/test1.png",  //分类配置图片
                "fontNum": "10",  //该分类下包含字体个数
                "supportCloud": true //该分类下是否包含支持云字体功能的字体
            },
            {
                "id": 2,
                "name": "分类2",
                "previewurl": "http://upaicdn.xinmei365.com/sdkimg/test2.png",
                "fontNum": "11",
                "supportCloud": false
            },
            ...
        ]
    }
```
