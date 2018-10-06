# PHPSTORM
### [xdebug 설정](https://www.jetbrains.com/help/phpstorm/configuring-xdebug.html)
- docker 설정 내용도 위 페이지에 있음
- xdebug.remote_enable=1
- xdebug.remote_port=9000
- xdebug.remote_host=host.docker.internal
```
you can set xdebug.remote_host to host.docker.internal, which automatically resolves to the internal address of the host, letting you easily connect to it from the container.
```
## PHPSTORM PACKAGE 설정
### laravel-ide-helper
- [laravel-ide-helper](https://github.com/barryvdh/laravel-ide-helper)
- package 설치
- 라라벨 code tracking helper
```
composer require --dev barryvdh/laravel-ide-helper
```
### codesniffer
- [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer/blob/master/README.md)
- package 설치
- code rule 위반 표시 
```
composer global require "squizlabs/php_codesniffer=*"
```
- [phpstorm 설정](https://confluence.jetbrains.com/display/PhpStorm/PHP+Code+Sniffer+in+PhpStorm)

### php-cs-fixer
- [PHP-CS-Fixer](https://github.com/FriendsOfPHP/PHP-CS-Fixer/blob/2.12/README.rst)
- package 설치
- code standard에 맡게 수정
```
composer global require friendsofphp/php-cs-fixer
```
- [phpstorm 설정](https://hackernoon.com/how-to-configure-phpstorm-to-use-php-cs-fixer-1844991e521f)

  

## PHPSTORM Tips!
- [laracasts 동영상](https://laracasts.com/series/how-to-be-awesome-in-phpstorm)
### Navigate
- navigate 찾기는 n 
```
ctrl + n : class
ctrl + shift + n : file
ctrl + shift + alt + n : method, variable, const
ctrl + shift + d : navigate database object
ctrl + alt + b : go to implementation
alt + up | down : move method
```

### New file 
```
1. 원하는 경로 이동 후(ctrl + n) 
2. project focus 상태에서 alt + insert
```

### Debug
```
ctrl + F8 : break point 
디버깅 flow는 chrome과 단축키를 맞춤. F10 : step over,F11 : step into
```

### Live template
```
1. Snippet 만들기 원하는 부분 block 지정 
2. ctrl + shift + a 
3. type : save as live template
4. live template 저장 화면에서 약어 및 설명 작성
5. edit variables에서 변수 설정을 세부적으로 가능하다.
```

### Refactor
- extract : variable, constant, field, parameter, method, interface
```
1. block 지정 or 커서 위치 
2. ctrl + shfit + alt + t 
3. extract 메뉴 선택 
4. 세부사항 설정
```
- 부모 class로 method 이동 하기
```
1. ctrl + shfit + alt + t 
2. pull up members 선택
```

### Generate
```
alt + Insert : overide, implement, construct, setter, getter
```

### Multiple cursors
```
alt + j : add selection for next occurrence
ctrl + alt + shift + j : select all occurrences 
```

### DB Navigator
- data source를 설정 하면 php 코드에 담겨있는 쿼리를 바로 실행할 수 있다.(ctrl + enter)
- php 코드에 injected 되어있는 sql을 변수 설정과 함께 수행 하는 방법 Settings > Tools > Databse > User Parameters에서 parameter patterns을 php 변수 형식으로 추가하면 가능 하다.
