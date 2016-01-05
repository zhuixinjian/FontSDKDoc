# 字体包功能
1. 初始化

    AndroidManifest.xml中添加
    ```xml
    <application ...>
        <!-- FontPack换字体 12345替换为appkey -->
        <receiver android:name="com.xinmei365.fontsdk.receiver.FontPackChangeFontBroadcasrReceiver" >
            <intent-filter>
            <action android:name="CHANGE_FONT_12345" />
            </intent-filter>
        </receiver>
    </application>```
    项目Application onCreate或入口Activity onCreate方法中初始化
    ```ruby
	FontCenter.getInstance(Context context).setFontPackChangeFontCallBack(
	    new FontPackChangeFontCallBack() {
			@Override
			public void changeFont(String fontPath, String packageName) {
				if (fontPath != null && !"".equals(fontPath)) {
					try {
						Typeface typeface = Typeface.createFromFile(fontPath);
						textView.setTypeface(typeface);
				    }catch (Exception e) {
				    }
				} else {
                }
		    }
	    });```

2. 获取分类列表
    ```ruby
    FontCenter.getInstance(Context context).getCateListFromServer(IHttpCallBack callback, String country)
    ```
3. 获取单个分类详细数据列表

    ```ruby
    FontCenter.getInstance(Context context).getCateFontListFromServer(IHttpCallBack callback,String id)
    ```

4. 根据字体id获取Font对象

    ```ruby
    //可通过Font.getTypeface()获取Typefaced对象，如果字体没下载，typeface为null
    FontCenter.getInstance(Context context).getFontById(String id);
    ```

