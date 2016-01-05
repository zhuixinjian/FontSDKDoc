

### 注意：FontCenter初始化从版本2.1.2开始由

```ruby
    FontCenter.getInstance();
```
### 改为

```ruby
    FontCenter.getInstance(Context context);
```

#初始化
1. (必须)项目Application onCreate方法中初始化
```ruby
    FontCenter.getInstance(Context context).initFontCenter(String app_key);
```
2. (必须)在程序的入口activity中的onCreate方法中调用
```ruby
    FontCenter.getInstance(Context context).init();
```
3. (可选)设置自定义下载目录，默认路径: /sdcard/yiziyun
```ruby
    FontCenter.getInstance(Context context).setFolder_font(String path);
```

4. (可选)设置自定义缓存目录，默认路径:/sdcard/yiziyun/cache
```ruby
    FontCenter.getInstance(Context context).setFolder_cache(String path);
```

