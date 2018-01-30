# phalapi2-apk -- APK文件解包处理

![](http://webtools.qiniudn.com/master-LOGO-20150410_50.jpg)

## 前言

PhalApi 2.x 扩展类库 - Apk 提供对APK文件解析功能

附上:

官网地址:[http://www.phalapi.net/](http://www.phalapi.net/ "PhalApi官网")

开源中国Git地址:[http://git.oschina.net/dogstar/PhalApi/tree/release](http://git.oschina.net/dogstar/PhalApi/tree/release "开源中国Git地址")

开源中国拓展Git地址:[http://git.oschina.net/dogstar/PhalApi-Library](http://git.oschina.net/dogstar/PhalApi-Library "开源中国Git地址")


## 1. 安装使用

此扩展只需要简单的把文件放到Library目录下即可使用使用方法如下:
```
// 在index.php中注册
\PhalApi\DI()->apk = function () {
     return new \PhalApi\Apk\Lite();
};
 
// 例子:
$targetFile = a.apk;//apk所在的路径地址
$res   = \PhalApi\DI()->apk->open($targetFile);
  
\PhalApi\DI()->apk->getAppName();     // 应用名称
\PhalApi\DI()->apk->getPackage();    // 应用包名
\PhalApi\DI()->apk->getVersionName();  // 版本名称
\PhalApi\DI()->apk->getVersionCode();  // 版本代码
```

## 2. 总结

希望此拓展能够给大家带来方便以及实用,拓展支持绝大部分APK文件处理!

注:笔者能力有限有说的不对的地方希望大家能够指出,也希望多多交流!

**官网QQ交流群:421032344  欢迎大家的加入!**
