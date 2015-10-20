# 获取分类和分类下的字体列表

本接口用于获取客户在SDK后台配置的对应国家下的字体分类和分类下的字体列表

```php
接口url : http://cdn5.xinmei365.com/cdndata/sdkapi/appAllFont?app_key=%s&country=%s&type=%s"

请求方式: GET

参数:
    app_key : 字符串，客户app唯一识别码， 后台可以看到
    country : 字符串，国家代码(参考5.2)
    type : 字符串，字体包格式，目前只支持"zip", 默认返回apk字体格式

返回格式: json

返回示例:
{
    "error_code": "0",//错误码，成功为0
    "error_msg": "success",//错误信息， 成功为success
    "data": [
        {
            "id": 120,//分类id
            "name": "列表",//分类名称
            "previewurl": "",//分类配置图片
            "fontNum": "11",//该分类下包含字体个数
            "supportCloud": true,//该分类下是否包含支持云字体功能的字体
            "fontlist": [
                {
                    "packageName": "",//包名,用于googleplay,客户配置
                    "jumpType": 0,//跳转方式,默认为0,普通下载,为2时表示跳转googleplay下载
                    "fontName": "印象",//字体名称
                    "fontPreviewUrl": "http://fonts.b0.upaiyun.com/fontPreZip/vZPdHUVb.zip",//包含字体名称小字体,zip文件,解压使用
                    "fontDownloadUrl": "http://upaicdn.xinmei365.com/fontzip/vZPdHUVb.zip",//文件下载url
                    "fontSize": 7182434,//字体大小(参考值, 实际大小请下载时获取)
                    "fontIdNo": "vZPdHUVb",//字体识别码(易字云字库中唯一识别字体)
                    "isHotFont": false,//最热(不建议使用)
                    "isNewFont": false,//最新(不建议使用)
                    "ft_sdk_support": 1,//字体支持功能,0为仅支持基本功能,1为支持云字体功能
                    "fontPreviewImg": "",//字体预览图片,易字云配置
                    "ownImg": "",//字体预览图片,客户自行配置
                    "aliases": "",//别名,客户自行配置
                    "preview_text": "",// 预览文字
                    "preview_text_ttf": ""// 包含预览文字ttf的zip压缩文件地址
                },
                {
                    "packageName": "",
                    "jumpType": 0,
                    "fontName": "淘淘体",
                    "fontPreviewUrl": "http://fonts.b0.upaiyun.com/fontPreZip/3APGuTX5.zip",
                    "fontDownloadUrl": "http://upaicdn.xinmei365.com/fontzip/3APGuTX5.zip",
                    "fontSize": 6396441,
                    "fontIdNo": "3APGuTX5",
                    "isHotFont": false,
                    "isNewFont": false,
                    "ft_sdk_support": 1,
                    "fontPreviewImg": "",
                    "ownImg": "",
                    "aliases": "",
                    "preview_text": "",
                    "preview_text_ttf": "http://upaicdn.xinmei365.com/fontPreZip/meitu_pre_zip/meitu_3APGuTX5.zip"
                },
               ...
            ]
        }
    ]
}
```
