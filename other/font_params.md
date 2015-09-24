# Font字段解释
| 字段 | 描述 | 类型 |
| -- | -- | -- |
| fontIdNo | 字体id编号（唯一） | String |
| fontName | 字体名称 | String |
| fontSize | 字体大小 | long |
| isHotFont | 是否是最热字体 | boolean |
| isNewFont | 是否是最新字体 | boolean |
| jumpType| 下载方式(0和1为直接下载；2为跳转谷歌市场下载)|int |
| fontDownloadUrl| 字体下载地址 | String |
| fontPreviewUrl| 字体名称预览ttf压缩文件地址 | String |
| packageName | 字体包名(只有该字体在海外市场时才有) | String |
| fontPreviewImg | 字体预览图下载地址，该图片为字体管家客户端的预览图 | String |
| ownImg | 字体预览图下载地址，该图片为用户配置的预览图  | String |
| downloadProgress |字体下载进度 | int |
| downloadDate | 字体下载日期 | String |
| fontLocalPath | 原始文件本地路径 | String |
| zhLocalPath | 中文字体本地路径 | String |
| enLocalPath | 英文字体本地路径 | String |
| thumbnailLocalPath | 预览文件本地路径 | String |
| fontSdkSupport | 支持类型（1为支持云字体，其它为不支持云字体）| int |
| fromType | 字体来源（）  | int |
| aliases | 别名  | String |
| previewText | 预览文字  | String |
| previewTextTTFUrl | 预览文字ttf的zip压缩文件下载地址 | String |


