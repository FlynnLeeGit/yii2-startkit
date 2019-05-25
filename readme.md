##

composer 切换国内源

容器内运行

```bash
composer config -g repo.packagist composer https://packagist.laravel-china.org

cd /usr/local/etc/php/conf.d

nano base.ini

# 修改memory_limit=-1

```
composer global require fxp/composer-asset-plugin:1.4.5

```

```

项目目录中
修改 composer.json 中使用 fxp-asset 管理前端的 bower 资源

```json
{
  "config": {
    "process-timeout": 1800,
    "fxp-asset": {
      "enabled": true // false -> true
    }
  }
}
```
安装依赖
```
composer install -vvv
```


github token 地址 https://github.com/settings/tokens