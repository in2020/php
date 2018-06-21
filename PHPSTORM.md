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
- 중복 코드 method로 만들기
```
1. 중복 코드 block 지정
2. ctrl + shfit + alt + t 
3. method 선택 
4. method 세부사항 설정
```
- 부모 class로 method 이동 하기
```
1. ctrl + shfit + alt + t 
2. pull up members 선택
```
- 변수로 추출 
```
1. ctrl + shfit + alt + t 
2. extract variable 선택 (inline은 반대)
```
