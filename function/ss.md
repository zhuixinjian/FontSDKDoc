# 字体包功能
1. AndroidManifest.xml中添加
    ```xml
    <application ...>
        <!-- FontPack换字体 12345替换为appkey -->
        <receiver android:name="com.xinmei365.fontsdk.receiver.FontPackChangeFontBroadcasrReceiver" >
            <intent-filter>
            <action android:name="CHANGE_FONT_12345" />
            </intent-filter>
        </receiver>
    </application>
    ```
2. 项目Application onCreate或入口Activity onCreate方法中初始化
    ```ruby
	FontCenter.getInstance().setFontPackChangeFontCallBack(
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
	    });
	```

