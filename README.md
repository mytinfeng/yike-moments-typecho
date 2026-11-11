# yike-moments-typecho
typecho版本的朋友圈

## 使用教程
安装Typecho
下载插件:[](https://github.com/mytinfeng/yike-moments-typecho/releases/download/v1.0.0/YikeMoments-plugin.zip)
下载主题:[](https://github.com/mytinfeng/yike-moments-typecho/releases/download/v1.0.0/yike-moments-theme.zip)

先：启动插件
后：启动主题
然：伪静态添加
```
if (-f $request_filename/index.html){
    rewrite (.*) $1/index.html break;
}
if (-f $request_filename/index.php){
    rewrite (.*) $1/index.php;
}
if (!-f $request_filename){
    rewrite (.*) /index.php;
}
```

同款Vue版本：[朋友圈Vue版](https://github.com/mytinfeng/yike-moments)

完成~
