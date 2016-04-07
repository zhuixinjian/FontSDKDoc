
#初始化
1. (必须)项目Application onCreate方法中初始化
```ruby
    FontCenter.initFontCenter(String appKey, Context applicationContext);
```
2. (必须)在程序的入口activity中的onCreate方法中调用
```ruby
    FontCenter.getInstance().init();
```
3. (可选)设置自定义下载目录，默认路径: /sdcard/yiziyun
```ruby
    FontCenter.getInstance().setFolder_font(String path);
```

4. (可选)设置自定义缓存目录，默认路径:/sdcard/yiziyun/cache
```ruby
    FontCenter.getInstance().setFolder_cache(String path);
```

