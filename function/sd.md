# 云字体功能
1. 手动获取云字体
    ```ruby
    FontCenter.getInstance().getTypeface(Font font,String text,CloudFontCallBack callBack);
	```
2. 自动获取云字体

    1. 开始自动加载云字体
    ```ruby
    FontCenter.getInstance().startAutoCloudText(Font font,TextView textView);
	```
	2. 设置自动加载云字体的font
	 ```ruby
    FontCenter.getInstance().setAutoCloudFont(Font font)；
    ```
    3. 设置自动加载云字体的textView
	 ```ruby
	FontCenter.getInstance().setAutoCloudTextView(TextView textView)；
	```
	4. 停止自动加载云字体
	 ```ruby
    FontCenter.getInstance().stopAutoCloudText();
	```
3. 获取云字体缓存大小
    ```ruby
    FontCenter.getInstance().getCloudCacheSize();
    ```
4. 清理云字体缓存
    ```ruby
    FontCenter.getInstance().cleanCloudCache();
    ```

