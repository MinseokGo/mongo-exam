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
# 스프링 부트 프로젝트와 DB 통신 순서

1.
```
brew services start mongodb-community@5.0
```
2.
```
mongod
```
3.
```
mongo
```
4. 이후 스프링 부트 프로젝트 어플리케이션 실행(순서 미준수 시 커넥션 거부)

# 로컬 폴더와 깃 레포 연동(모두 터미널에 입력)
1.
```
git config --global user.name "git hub 닉네임" (내 기준 MinseokGo)
```
2.
```
git config --global user.email "git hub 이메일"
```
3. 클론할 레포지토리의 링크복사(해당 레포의 코드 버튼을 클릭하면 주소 나옴)
4. 연동할 로컬 폴더로 터미널 상에서 cd를 통해 path 지정
```
cd Documents/...
```
5. 
```
git clone 복사한 주소
```
6. 클론된 레포가 로컬 저장소에 생성됨. 이때 저장할 파일들을 클론된 레포에 옮김
7. 추가, 변경된 파일 확인
```
git status
```
8.
```
git add .
또는
git add 파일/디렉토리 경로
```
9. 커밋 후 푸시
```
git commit -m "커밋메시지"
git push origin 브랜치명
```
