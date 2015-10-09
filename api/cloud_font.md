# 云字体

本接口用于获取云字体ttf文件(Beta版)

```php
接口url : http://api.yun.zitiguanjia.com:8000/index/min_ttf

请求方式: GET

参数:
    app_key : 字符串, 客户app唯一识别码, 后台可以看到
    font_id_no : 字符串, 字体识别码, 4.2中fontIdNo字段
    str : 获取云字体的字符(建议不超过140字,字数过多建议分次获取)

返回格式: ttf or json

返回: 处理成功将直接返回ttf文件，失败会返回对应的错误信息，格式为json

失败时返回示例:
{
    data: "",
    error_code: 401,
    error_msg: "字体不存在"
}
```
