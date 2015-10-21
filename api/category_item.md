# 获取分类下字体列表

本接口用于获取客户在SDK后台配置的字体分类下所有字体列表

```php
接口url : http://cdn5.xinmei365.com/cdndata/sdkapi/categoryFont

请求方式: GET

参数:
    app_key : 字符串，客户app唯一识别码， 后台可以看到
    cate_id : 字符串，用户配置分类id(参考4.1)
    type : 字符串，字体包格式，目前只支持"zip", 默认返回apk字体格式

返回格式: json

返回示例:
    {
        "error_code": "0", //错误码，成功为0
        "error_msg": "success", //错误信息， 成功为success
        "data": [
            {
                "packageName": "", //包名,用于googleplay,客户配置
                "jumpType": 0, //跳转方式,默认为0,普通下载,为2时表示跳转googleplay下载
                "fontName": "桃心下午茶", //字体名称
                "fontPreviewUrl": "", //包含字体名称小字体,zip文件,解压使用
                "fontDownloadUrl": "", //文件下载url
                "fontSize": 11109085, //字体大小(参考值, 实际大小请下载时获取)
                "fontIdNo": "DnPUvr5z", //字体识别码(易字云字库中唯一识别字体)
                "isHotFont": false, //最热(不建议使用)
                "isNewFont": false, //最新(不建议使用)
                "ft_sdk_support": 0, //字体支持功能,0为仅支持基本功能,1为支持云字体功能
                "fontPreviewImg": null, //字体预览图片,易字云配置
                "ownImg": "" //字体预览图片,客户自行配置
            },
            {
                "packageName": "",
                "jumpType": 0,
                "fontName": "绵忆",
                "fontPreviewUrl": "http://upaicdn.xinmei365.com/wfs/2014-01/525d86ca9ee1437fad81d86cce0754bd.zip",
                "fontDownloadUrl": "http://upaicdn.xinmei365.com/wfs/2014-01/87c9a4a001344ebf8c39bddfc403d601.apk",
                "fontSize": 13887828,
                "fontIdNo": "8p4gS6Is",
                "isHotFont": false,
                "isNewFont": false,
                "ft_sdk_support": 0,
                "fontPreviewImg": null,
                "ownImg": ""
            },
            ...
        ]
    }
```
