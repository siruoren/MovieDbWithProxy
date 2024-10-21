### MovieDB with proxy plugin for Emby media server

# Emby-MovieDbProxy-Plugins
Emby TMDB 刮削器的代理插件

## 安装插件

### 插件放到群晖里，右键插件文件，点击属性，复制插件位置

通常都是

/Volume1/@appdata/EmbyServer/plugins

如果没有显示默认存储空间，默认就是存储空间1

根据存储空间后面的数字，比如存储空间2，对应

/Volume2/@appdata/EmbyServer/plugins

### 新增


```
mv /volume1/Test/MovieDbWithProxy.dll /volume1/@appdata/EmbyServer/plugins
chown emby:emby /volume1/@appdata/EmbyServer/plugins/MovieDbWithProxy.dll
chmod 644 /volume1/@appdata/EmbyServer/plugins/MovieDbWithProxy.dll
```



## 查看插件是否安装

### 重启EMBY

### 进入EMBY设置，点击插件
找到MovieDbWithProxy，点击配置，输入代理地址信息，点击保存


### 使用插件

媒体文件夹里的刮削器勾选TheMovieDbProxy，保存后，刷新元数据


