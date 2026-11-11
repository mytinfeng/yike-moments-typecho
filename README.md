# yike-moments-typecho
typecho版本的朋友圈

## 环境推荐：
- Nginx
- PHP 8.2以上（低版本的没试过，建议PHP 8.4）
- Mysql 5.6及以上

## 使用教程
安装Typecho

下载插件:[朋友圈-插件包](https://github.com/mytinfeng/yike-moments-typecho/releases/download/v1.0.0/YikeMoments-plugin.zip)

下载主题:[朋友圈-主题包](https://github.com/mytinfeng/yike-moments-typecho/releases/download/v1.0.0/yike-moments-theme.zip)


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
