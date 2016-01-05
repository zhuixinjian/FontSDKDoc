# 字体管家支持功能

1. 在Manifest中添加广播接收器
    ```
    <receiver android:name="com.xinmei365.fontsdk.receiver.ChangeFontBroadcastReceiver">
        <intent-filter >
            <action android:name="com.xinmei365.fontsdk.change"/>
        </intent-filter>
    </receiver>
    ```

2. 检查字体管家状态
    ```ruby
    /**
     * 返回值为0, 1, 2
     * 0 : 字体管家已安装, 且支持单应用换字体功能
     * 1 : 字体管家已安装, 不支持支持单应用换字体功能
     * 2 : 字体管家未安装
     */
    FontCenter.getInstance(Context context).checkFontManager();
    ```

3. 下载字体管家
    ```ruby
    FontCenter.getInstance(Context context).downloadFontmanager(FileDownloadCallBack callback)
    ```
