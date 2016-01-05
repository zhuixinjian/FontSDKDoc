# 字体使用
1. 创建Typeface

    1. 通过Font对象获取Typefaced对象，如果字体没下载，typeface为null

    **只适用于下载到本地的字体，不适用于云字体**

    ```ruby
    Typeface typeface=font.getTypeface();
    ```

    2. 通过文件路径获取Typeface对象

    获取中文Typeface对象
    ```ruby
    Typeface typeface=Typeface.createFromFile(font.getZhLocalPath());
    ```
     获取英文Typeface对象
    ```ruby
    Typeface typeface=Typeface.createFromFile(font.getEnLocalPath());
    ```

2. 使用Typeface
    ```ruby
    TextView textView=new TextView(context);
    textView.setTypeface(typeface);

    Paint paint= new Paint();
	paint.setTypeface(typeface);
	```
