## 문제
- ajax를 두번 연달아 호출하면 database connection error 발생

## 분석
- database connection 정보가 전달 안됨 
- db connection 정보는 .env 파일에 설정 되어 있고 phpdotenv library를 사용하여 $_SERVER의 서버 환경 변수값을 토대로 값을 가져옴 
- 연속 호출시 phpdotenv를 통한 $_SERVER에 변수 값이 할당 안됨
- $_SERVER 에 값을 할당되는 부분을 보니 php native getenv 함수를 통해 이미 값이 할당되어 있다고 되어 있음 

## 예상 
- 첫번째 콜을 통해 변경된 서버사이드 변수 설정이 영향을 주는것 같다. 
   apache_setenv로 설정되는 값이 설마 파일에 쓰여저 원복되는데 시간차가 있어서 그런건가 ㅡㅡ;; 설마;;;
