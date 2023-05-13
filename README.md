# Mac OS : 터미널에서 MongoDB 설치
<br>
Homebrew 설치 및 터미널 환경변수 설정
<br>
https://melonicedlatte.com/2022/06/27/230000.html

Homebrew를 통한 터미널에서 MongoDB 설치
<br>
https://choboit.tistory.com/95

터미널 MongoDB 명령어
<br>
https://jinshine.github.io/2018/06/10/MongoDB/%EA%B8%B0%EB%B3%B8%EC%A0%81%EC%9D%B8%20%EB%AA%85%EB%A0%B9%EC%96%B4/

MongoDB account 생성
<br>
https://rastalion.me/mongodb-4-2-admin-%EA%B3%84%EC%A0%95-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0/

Spring boot project에서 application.yml 코드(로컬 MongoDB와의 연결)
```yml
# spring
spring:
  data:
    mongodb:
      host: localhost
      database: DB Name
      username: User Name
      password: User Password
      uri: mongodb://localhost:27017/DB Name
```
