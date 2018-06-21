# PHPSTORM
## PHPSTORM PACKAGE 설정
### codesniffer
- [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer/blob/master/README.md)
- package 설치
```
composer global require "squizlabs/php_codesniffer=*"
```
- [phpstorm 설정](https://confluence.jetbrains.com/display/PhpStorm/PHP+Code+Sniffer+in+PhpStorm)

### php-cs-fixer
- [PHP-CS-Fixer](https://github.com/FriendsOfPHP/PHP-CS-Fixer/blob/2.12/README.rst)
- package 설치
```
composer global require friendsofphp/php-cs-fixer
```
- [phpstorm 설정](https://hackernoon.com/how-to-configure-phpstorm-to-use-php-cs-fixer-1844991e521f)

## PHPSTORM Tips!
### navigate
- navigate 찾기는 n 
```
ctrl + n : class
ctrl + shift + n : file
ctrl + shift + alt + n : method, variable, const
ctrl + shift + d : navigate database object
ctrl + alt + b : go to implementation
alt + up | down : move method
```

### new file 
```
1. 원하는 경로 이동 후(ctrl + n) 
2. project focus 상태에서 alt + insert
```