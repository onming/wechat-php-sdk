# wechat-php-sdk
微信sdk插件
将会陆续更新

## 环境准备
*   PHP 7.0+
    您可以通过`php -v`命令查看当前的 PHP 版本。
*   curl 扩展
    您可以通过`php -m`命令查看 curl 扩展是否已经安装好。

## 安装方式 
### Composer 方式
```
composer require onming/wechat-php-sdk ~1.0
```

### 使用方法
```
use Onming\WechatPhpSdk\Jssdk;
$jssdk = new Jssdk(app_id, app_secret, 'thinkphp'); // 第三参数如果为thinkphp则采用tp自带缓存，默认空使用文件缓存需设置temp目录读写权限
$signPackage = $jssdk->GetSignPackage();
var_dump($signPackage);
```
