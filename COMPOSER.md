# Composer
[한글 사이트](http://xpressengine.github.io/Composer-korean-docs/doc/00-intro.md/)
## Introduction
의존성 관리 툴

### System Requirements
PHP 5.3.2+ to run. 

### Composer install
[Installation - Windows](https://getcomposer.org/doc/00-intro.md#installation-windows)

### [Basic usage](https://getcomposer.org/doc/01-basic-usage.md#basic-usage)

### [Command](https://getcomposer.org/doc/03-cli.md)
```
composer dump
php composer.phar init
php composer.phar install
php composer.phar update
php composer.phar install/update monolog/monolog
php composer.phar require
php composer.phar remove vendor/package vendor/package2
php composer.phar global require friendsofphp/php-cs-fixer
php composer.phar show monolog/*
composer show -lo
php composer.phar validate
php composer.phar status
php composer.phar self-update
composer.phar config --list
```
### [Config](https://getcomposer.org/doc/06-config.md)

### conposer.lock
의존성 패키지들을 설치한 뒤에 컴포저는 composer.lock파일에 설치한 패키지들의 정확한 버전 목록을 저장합니다.  
이 잠금설정들이 프로젝트가 필요로 하는 특정 버전들을 의미합니다.
