# 易字云SDK开发手册

## 当前版本2.1.3

本手册只适用于易字云SDK最新版本

易字云SDK主要用于为开发者提供字体资源，通过SDK的形式，实现开发者对字体的下载管理和使用等功能

## 下载SDK

[易字云SDK (Demo+jar)][demojar_download]

[易字云SDK (jar)][jar_download]


## 更新日志

###SDK V2.1.3：

1. 恢复初始化方式
2. 增加fontKey验证
3. 解决部分bug

###SDK V2.1.2：

1. 更改初始化方式
2. 优化缓存
3. 优化统计
4. 解决部分bug

###SDK V2.1.1：

1. 新增统计
2. 解决6.0权限问题
3. 优化下载

###SDK V2.1：

1. 增加云字体功能
2. 增加字体包功能
3. 优化字体列表功能

###SDK V2.0.1：

1. 优化统计功能，提供精确数据分析报表
2. 优化下载

###SDK V2.0：

1. 获取字体列表信息接口
`getCateListFromServer(IHttpCallBack callback, String country) ` SDK现在加入对国家的支撑,提供了国家代码来支撑不同国家的字体,用于国际化.
Country：国家代号，比如说中文字体：cn，英文字体cn，日文字体 ja
Callback：获取数据回调接口
2. 新增字体包用于跳转谷歌市场下载字体 `downloadFont(Font font, Context context)`
和跳转方式，如果有需要在海外市场下载字体的话，请联系管理员。
3. 根据字体信息删除字体文件 deleteFont(Font font)


[demojar_download]:http://doc.zitiguanjia.com/public/file/sdkfile/fontsdk(jar+demo).zip
[jar_download]:http://doc.zitiguanjia.com/public/file/sdkfile/fontsdk.jar
