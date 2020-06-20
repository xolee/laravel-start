![Laravel Start](https://i.loli.net/2020/06/20/AwyeZW8IQi5lza1.png)

## Laravel Start

保持最新 Laravel 版本，可供在此版本直接食用。

## 食用方法

```
# install
sudo git clone https://github.com/xolee/laravel-start.git laravel-start
cd laravel-start
composer install
sudo cp .env.example .env
sudo php artisan key:generate

# 关闭站点
sudo php artisan down

# 文件夹权限
sudo chown -R www:www /home/wwwroot/laravel-start
sudo chmod -R 775 /home/wwwroot/storage

# 数据库
sudo php artisan migrate

# 各种清空缓存和重建缓存
sudo php artisan clear-compiled 
sudo php artisan cache:clear 

sudo php artisan config:cache 
sudo php artisan optimize 
sudo composer dump-autoload --optimize 

# 开启站点
sudo php artisan up
```

## Package List

### Dev 环境

Packages |  作用 | 链接 | 命令
:-: | :-: | :-: | :-:
barryvdh/laravel-debugbar | Debugbar | [链接][5] | `composer require barryvdh/laravel-debugbar --dev`
summerblue/generator | 代码生成 | [链接][6] | `composer require summerblue/generator --dev`
laravel/ui | Laravel 默认UI 包 | [链接][12] | `composer require laravel/ui --dev`

### Web 环境

Packages | 作用 | 链接 | 命令
:-:|:-:|:-:|:-:
laravelcollective/html | HTML/Form 生成 | [链接][1] | `composer require laravelcollective/html`
overtrue/laravel-lang | 多语言包 | [链接][3] | `composer require overtrue/laravel-lang`
intervention/image | 图片处理 | [链接][4] | `composer require intervention/image`

## 更新记录


[1]:https://packagist.org/packages/laravelcollective/html
[3]:https://packagist.org/packages/overtrue/laravel-lang
[4]:https://packagist.org/packages/intervention/image
[5]:https://packagist.org/packages/barryvdh/laravel-debugbar
[6]:https://packagist.org/packages/summerblue/generator
[12]:https://packagist.org/packages/laravel/ui
