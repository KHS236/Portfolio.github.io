# RANKINGSYSTEM_BN

### HISTORY
---
[바로가기](./HISTORY.md)

### TEAM
---
|NAME|ROLE|GITHUB_LINK|
|------|---|---|
|홍길동|조장-BACKEND/CONTROLLER | -
|강지영|조원-FRONTEND|-|
|조은파|조원-FRONTEND|-|

### PLAN
---
|DATE|CATEGORY|PATH|METHOD|CONTENT|LEVEL|IS_SUCCEED|
|-|-|-|-|-|-|-|
|2024-04-01|BE_INIT|/user/join|GET|회원가입|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/user/join|POST|회원가입|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/login<br>/logout|GET|로그인/로그아웃|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/login<br>/logout|POST|로그인/로그아웃|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|-|-|REMEMBER_ME|OPTIONAL| **TRUE**
|2024-04-01|BE_INIT|/user/reid<br>/user/repassword|-|아이디/패스워드 복구|OPTIONAL| FASLE
|2024-04-01|BE_INIT|/user/album/add|-|이미지 파일 업로드|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/user/album/main|-|내 앨범 전체 조회|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/user/album/main|-|내 앨범 키워드 조회(좋아요순/조회순)|**IMPORTANT**| FALSE
|2024-04-01|BE_INIT|/imageranking/list|-|이미지 랭킹 전체 조회|**IMPORTANT**| **TRUE**
|2024-04-01|BE_INIT|/user/album/main?keyfield=?&keyword=?|-|이미지 키워드(좋아요/조회순) 조회|**IMPORTANT**| FASLE




### USE SKILLS
---
 
<img src="https://img.shields.io/badge/HTML5-3366CC?style=for-the-badge&logo=htmlacademy&logoColor=white"> <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white"> 
<img src="https://img.shields.io/badge/JAVA-005571?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SPRINGBOOT-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> 
<img src="https://img.shields.io/badge/MYSQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">  
<img src="https://img.shields.io/badge/GIT-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github2&logoColor=white"> 
<img src="https://img.shields.io/badge/AWS-EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"> 
### DEPENDENCIES
---

#### CSS CDN
  - 01
  - 01
  - 01
  
#### JS CDN
  - 01
  - 01
  - 01

#### SPRING BOOT DEPENDENCIES
  - 01
  - 01
  - 01
  

### FILE TREE [tree /F | clip]
---

#### BACKEND TREE
![20240321004200](https://github.com/ALL-MY-PROJECTS-2024/99_RANKINGSYSTEM_DEPLOY/assets/84259104/1f123421-69b8-4915-a0e0-16681d03fa38)
![20240321004210](https://github.com/ALL-MY-PROJECTS-2024/99_RANKINGSYSTEM_DEPLOY/assets/84259104/49f04154-0701-43f9-afc8-e45d607677fe)

#### FRONTEND TREE
![20240321004218](https://github.com/ALL-MY-PROJECTS-2024/99_RANKINGSYSTEM_DEPLOY/assets/84259104/28c998ec-e648-4888-8164-0429d01682a2)
![20240321004222](https://github.com/ALL-MY-PROJECTS-2024/99_RANKINGSYSTEM_DEPLOY/assets/84259104/54f77b7b-eef9-4fa2-a4e6-20ca5c8832ce)

### AWS EC2 ISSUE[지울예정]
---
 -
 - Jenkins 배포시 사용할 /tmp 공간확보하기 (https://velog.io/@springkim/ubuntu-tmp-%EB%94%94%EB%A0%89%ED%84%B0%EB%A6%AC-%EC%9A%A9%EB%9F%89-%EB%8A%98%EB%A6%AC%EA%B8%B0)
 - /upload 폴더에 jenkins 계정으로 w 권한 주기


### RULE
---
- GITHUB COMMIT MESSAGE
  - git commit -m "[VERSION] [NAME] [DESCRIPTION]"
    - EX ] git commit -m "V1.2.3 JUNGWOOGYUN ADDED STYLE" 
      - 1 : Major Version(ex.페이지 추가/구조/기본스타일링) 
      - 2 : Miner Version(ex.기능추가)
      - 3 : Patch(ex.기존기능/스타일 수정

