# Font字段解释
| 字段 | 描述 | 类型 |
| -- | -- | -- |
| fontIdNo | 字体id编号（唯一） | String |
| fontName | 字体名称 | String |
| fontSize | 字体大小 | Long |
| isHotFont | 是否是最热字体 | Boolean |
| isNewFont | 是否是最新字体 | Boolean |
| jumpType | 下载方式(1、直接下载 2、跳转谷歌市场下载) | Int |
| fontDownloadUrl | 字体下载地址 | String |
| fontPreviewUrl | 字体预览文件地址 | String |
| packageName | 字体包名(只有该字体在海外市场时才有) | String |
| fontPreviewImg | 字体预览图片地址，该图片用户配置 | String |
| downloadProgress | 字体下载进度 | Int |
| downloadDate | 字体下载日期 | String |
| fontLocalPath | 原始文件本地路径 | String |
| zhLocalPath | 中文字体本地路径 | String |
| enLocalPath | 英文字体本地路径 | String |
| thumbnailLocalPath | 预览文件本地路径 | String |
