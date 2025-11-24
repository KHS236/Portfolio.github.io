# 구인구직웹 프로젝트

DEVELOPMENT MOTIVATION
---
> 구인구직싸이트 -
> > 구인구직을 하는 입장에서 사람인이나 잡코리아와 같은 사이트 <br> 
> > 보다 더 간편하게 정보를 수집할 수 있는 사이트 <br> 
 

HISTORY
---
[TOTAL](DOCUMENT/HISTORY/TOTAL) | [나재현](https://github.com/Najaehyun0913) | [이동환](https://github.com/donghwan12) | [박정현](https://github.com/niangsoul) | [최원준](https://github.com/piepenie) |


PLANS
---
 |LANGUAGE|PLAN|IMPLEMENT|DESCRIPTION|
 |-|-|-|-|
 |JAVA|2024/04/08 ~ 2024/04/23|-|-|
 |JSP/SERVLET|2024/04/24 ~ 2024/04/28|-|-|
 |SPRING STS3|2024/04/28 ~ 2024/05/14|-|-|
 |SPRING BOOT|2024/05/15 ~ 2024/06/30|-|-|
 
 

MEMBERERS
--- 
|NAME|ROLE|DETAILS|DESCRIPTION| 
|---|---|---|---|
|정우균|FN| FrontController / Docment 관리 / Dependencies  관리 |---|
|최원준|FN| 모든PAGE와 서버간 REQ / RESP |---|
|나재현|BN| 유저공통 - ID찾기 / PW찾기 / 회원가입 유효성검사 |---|
|이동환|BN| SEEKER 이력서 CRUD / 공지사항 CRUD |---|
|박정현|BN| OFFER 기업정보 CRUD / 기업공고 CRUD |---|

SKILLS
---

#### FN
---
<img src="https://img.shields.io/badge/HTML5-3366CC?style=for-the-badge&logo=htmlacademy&logoColor=white"> <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white"> <img src="https://img.shields.io/badge/JQUERY-0769AD?style=for-the-badge&logo=jquery&logoColor=white"> 


#### BN
---
<img src="https://img.shields.io/badge/JAVA-005571?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/JSP-1E8CBE?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SERVLET-4B4B77?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SPRING-STS3-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/SPRINGBOOT-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> 

#### DATABASE
---
<img src="https://img.shields.io/badge/MYSQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">  


#### DEVOPS
---
<img src="https://img.shields.io/badge/GIT-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github2&logoColor=white"> <img src="https://img.shields.io/badge/AWS-EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"> <img src="https://img.shields.io/badge/DOCKER-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/DOCKERHUB-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/JENKINS-D24939?style=for-the-badge&logo=jenkins&logoColor=white"> 


END POINT DOC
---
|URI|REQUEST METHOD|DESCRIPTION|
|---|---|---|
|/user/join|POST|회원가입을 합니다. 회원가입은 구직자, 채용자(기업가)로 나눠서 가입할 수 있습니다.|
|/user/confirmid|GET/POST|회원 아이디를 확인하는 서비스입니다.|
|/user/confirmpw|GET/POST|회원 비밀번호를 확인하는 서비스입니다.|
|---|---|---|
|/seeker/resume/add|GET/POST|구직자가 이력서를 작성합니다.|
|/seeker/resume/update|GET/POST|구직자가 작성된 이력서를 수정합니다.|
|/seeker/resume/read|GET|구직자가 작성된 이력서를 조회합니다.|
|/seeker/resume/list|GET|구직자가 작성된 이력서들의 목록을 조회합니다.|
|/seeker/delete|GET/POST|구직자가 작성된 이력서를 삭제합니다.|
|---|---|---
|/offer/company/add|GET/POST|채용자가 기업 정보를 추가합니다.|
|/offer/company/read|GET|채용자의 기업 정보를 조회합니다.|
|/offer/company/delete|GET/POST|채용자가 기업 정보를 삭제합니다.|
|/offer/company/update|GET/POST|채용자가 기업 정보를 수정합니다.|
|---|---|---|
|/offer/jobopening/read|GET|채용자가 채용 공고를 조회합니다.|
|/offer/jobopening/add|GET/POST|채용자가 채용 공고를 추가합니다|
|/offer/jobopening/list|GET|채용자가 채용 공고를 조회합니다.|
|/offer/jobopening/update|GET/POST|채용자가 채용 공고를 수정합니다.|
|/offer/jobopening/delete|DELETE|채용자가 채용 공고를 삭제합니다.|
|---|---|---|
|/community/add|GET/POST|커뮤니티 게시판에 게시물을 작성합니다.|
|/community/list|GET|커뮤니티 게시판의 목록을 조회합니다.|
|/community/read|GET|커뮤니티 게시글을 조회합니다.|
|/community/update|GET/POST|커뮤니티 게시글을 수정합니다.|
|/community/delete|GET/POST|커뮤니티 게시글을 삭제합니다.|
|/community/reply/add|GET|커뮤니티 게시물에 답글을 작성합니다.|


DEPENDENCIES LIST
---
|CAT|NAME|DESCRIPTION|LINK|-|-|
|-|-|-|-|-|-|
|FN|WEB| BOOT WEB|org.springframework.boot:spring-boot-starter-web|-|-|
|FN|THYMELEAF| THYMELEAF|org.springframework.boot:spring-boot-starter-thymeleaf|-|-|
|BN|LOMBOK|LOMBOK| org.projectlombok:lombok|-|-|
|BN|SPRING_SECURITY| SPRING_SECURITY|org.springframework.boot:spring-boot-starter-security|-|-|
|BN|SECURITY+THYMELEAF| SECURITY+THYMELEAF|org.thymeleaf.extras:thymeleaf-extras-springsecurity6|-|-|
|BN|ORM_JPA| ORM_JPA|org.springframework.boot:spring-boot-starter-data-jpa|-|-|
|BN|MAIL| MAIL|org.springframework.boot:spring-boot-starter-mail|-|-|
|BN|DEVTOOLS| DEVTOOLS|org.springframework.boot:spring-boot-devtools|-|-|
|BN|VALIDATOR| VALIDATOR|org.springframework.boot:spring-boot-starter-validation|-|-|
|BN|OAUTH2-Client| OAUTH2-Client|org.springframework.boot:spring-boot-starter-oauth2-client|-|-|
|BN|THUMNAILATOR| THUMNAILATOR|net.coobird:thumbnailator:0.4.20|-|-|
|BN|REST| REST|com.fasterxml.jackson.core:jackson-databind|-|-|
|DB|DBCONN BASIC| DBCONN BASIC|org.springframework.boot:spring-boot-starter-jdbc|-|-|


ERD[KoreaJobDb]
---
![ERD](https://github.com/user-attachments/assets/be538a90-4163-480e-92f8-5c61591bd31a)


FILE TREES[]
--- 
```
C:.
│  .gitignore
│  build.gradle
│  gradlew
│  gradlew.bat
│  settings.gradle
│
├─gradle
│  └─wrapper
│          gradle-wrapper.jar
│          gradle-wrapper.properties
│
└─src
    ├─main
    │  ├─java
    │  │  └─com
    │  │      └─example
    │  │          └─jobKoreaIt
    │  │              │  devJava.java
    │  │              │  JobKoreaItApplication.java
    │  │              │  test1234.java
    │  │              │
    │  │              ├─config
    │  │              │  │  DataSourceConfig.java
    │  │              │  │  MultipartConfig.java
    │  │              │  │  SecurityConfig.java
    │  │              │  │  TxConfig.java
    │  │              │  │  WebMvcConfig.java
    │  │              │  │
    │  │              │  └─auth
    │  │              │      │  PrincipalDetails.java
    │  │              │      │  PrincipalDetailsOAuth2Service.java
    │  │              │      │  PrincipalDetailsService.java
    │  │              │      │
    │  │              │      ├─exceptionHandler
    │  │              │      │      CustomAccessDeniedHandler.java
    │  │              │      │      CustomAuthenticationEntryPoint.java
    │  │              │      │
    │  │              │      ├─jwt
    │  │              │      │      JwtAuthorizationFilter.java
    │  │              │      │      JwtProperties.java
    │  │              │      │      JwtTokenProvider.java
    │  │              │      │      KeyGenerator.java
    │  │              │      │      TokenInfo.java
    │  │              │      │
    │  │              │      ├─loginHandler
    │  │              │      │      CustomAuthenticationFailureHandler.java
    │  │              │      │      CustomLoginSuccessHandler.java
    │  │              │      │
    │  │              │      ├─logoutHandler
    │  │              │      │      CustomLogoutHandler.java
    │  │              │      │      CustomLogoutSuccessHandler.java
    │  │              │      │
    │  │              │      └─provider
    │  │              │              GoogleUserInfo.java
    │  │              │              KakaoUserInfo.java
    │  │              │              NaverUserInfo.java
    │  │              │              OAuth2UserInfo.java
    │  │              │
    │  │              ├─controller
    │  │              │  │  CommunityController.java
    │  │              │  │  HomeController.java
    │  │              │  │  NotificationController.java
    │  │              │  │  RecruitController.java
    │  │              │  │  UserController.java
    │  │              │  │
    │  │              │  └─user
    │  │              │      ├─offer
    │  │              │      │      jobOpeningController.java
    │  │              │      │      OfferController.java
    │  │              │      │
    │  │              │      └─seeker
    │  │              │              ApplyController.java
    │  │              │              JobSeekerController.java
    │  │              │              JobSeekerRestController.java
    │  │              │              ResumeController.java
    │  │              │
    │  │              ├─domain
    │  │              │  ├─common
    │  │              │  │  ├─dto
    │  │              │  │  │      CommunityDto.java
    │  │              │  │  │      Criteria.java
    │  │              │  │  │      PageDto.java
    │  │              │  │  │      ReplyDto.java
    │  │              │  │  │      UserDto.java
    │  │              │  │  │
    │  │              │  │  ├─entity
    │  │              │  │  │      Community.java
    │  │              │  │  │      Reply.java
    │  │              │  │  │      Signature.java
    │  │              │  │  │      User.java
    │  │              │  │  │
    │  │              │  │  ├─repository
    │  │              │  │  │      CommunityRepository.java
    │  │              │  │  │      ReplyRepository.java
    │  │              │  │  │      UserRepository.java
    │  │              │  │  │
    │  │              │  │  └─service
    │  │              │  │          CommunityServiceImpl.java
    │  │              │  │          RecruitServiceImpl.java
    │  │              │  │          ReplyServiceImpl.java
    │  │              │  │          UserServiceImpl.java
    │  │              │  │
    │  │              │  ├─Notification
    │  │              │  │  ├─dto
    │  │              │  │  │      notificationDto.java
    │  │              │  │  │
    │  │              │  │  ├─entity
    │  │              │  │  │      NotifiEntity.java
    │  │              │  │  │
    │  │              │  │  ├─repository
    │  │              │  │  │      NotifiRepository.java
    │  │              │  │  │
    │  │              │  │  └─service
    │  │              │  │          NotifiService.java
    │  │              │  │
    │  │              │  ├─offer
    │  │              │  │  ├─dto
    │  │              │  │  │      CompanyDto.java
    │  │              │  │  │      JobOfferDto.java
    │  │              │  │  │      RecruitDto.java
    │  │              │  │  │
    │  │              │  │  ├─entity
    │  │              │  │  │      Company.java
    │  │              │  │  │      JobOffer.java
    │  │              │  │  │      Recruit.java
    │  │              │  │  │
    │  │              │  │  ├─repository
    │  │              │  │  │      CompanyRepository.java
    │  │              │  │  │      JobOfferRepository.java
    │  │              │  │  │      JobopeningRepository.java
    │  │              │  │  │      RecruitRepository.java
    │  │              │  │  │
    │  │              │  │  └─service
    │  │              │  │          JobOfferServiceImpl.java
    │  │              │  │          jobopeningServicelmpl.java
    │  │              │  │
    │  │              │  └─seeker
    │  │              │      ├─dto
    │  │              │      │      ApplyDto.java
    │  │              │      │      CarrerDto.java
    │  │              │      │      CertificationDto.java
    │  │              │      │      JobSeekerDto.java
    │  │              │      │      ResumeDto.java
    │  │              │      │      ResumeFormDto.java
    │  │              │      │
    │  │              │      ├─entity
    │  │              │      │      Apply.java
    │  │              │      │      Carrer.java
    │  │              │      │      Certification.java
    │  │              │      │      JobSeeker.java
    │  │              │      │      Resume.java
    │  │              │      │
    │  │              │      ├─repository
    │  │              │      │      ApplyRepository.java
    │  │              │      │      CareerRepository.java
    │  │              │      │      CertificationRepository.java
    │  │              │      │      JobSeekerRepository.java
    │  │              │      │      ResumeRepository.java
    │  │              │      │
    │  │              │      └─service
    │  │              │              ApplyServiceImpl.java
    │  │              │              JobSeekerServiceImpl.java
    │  │              │              ResumeServiceImpl.java
    │  │              │
    │  │              └─properties
    │  │                      AUTH.java
    │  │                      DBCONN.java
    │  │                      UPLOADPATH.java
    │  │
    │  └─resources
    │      │  application.properties
    │      │  data.sql
    │      │
    │      ├─static
    │      │  ├─assets
    │      │  │  │  check.svg
    │      │  │  │  facebookicon.png
    │      │  │  │  githublogo.png
    │      │  │  │  instraicon.png
    │      │  │  │  logo.gif
    │      │  │  │  logo.png
    │      │  │  │  logo_2.png
    │      │  │  │
    │      │  │  └─sample
    │      │  │          05_edu_img_240620_01.png
    │      │  │          05_edu_img_240620_02.png
    │      │  │          05_edu_img_240620_03.png
    │      │  │          05_edu_img_240620_04.png
    │      │  │          05_edu_img_240620_05.png
    │      │  │          05_edu_img_240620_06.png
    │      │  │          05_edu_img_240620_07.png
    │      │  │
    │      │  ├─css
    │      │  │  │  common.css
    │      │  │  │  index.css
    │      │  │  │
    │      │  │  ├─community
    │      │  │  │      add.css
    │      │  │  │      delete.css
    │      │  │  │      index.css
    │      │  │  │      list.css
    │      │  │  │      read.css
    │      │  │  │      update.css
    │      │  │  │
    │      │  │  ├─mobile
    │      │  │  │      common.css
    │      │  │  │
    │      │  │  ├─notification
    │      │  │  │      add.css
    │      │  │  │      list.css
    │      │  │  │      read.css
    │      │  │  │      update.css
    │      │  │  │
    │      │  │  ├─offer
    │      │  │  │  │  myinfo.css
    │      │  │  │  │
    │      │  │  │  └─jobopening
    │      │  │  │          add.css
    │      │  │  │          applylist.css
    │      │  │  │
    │      │  │  ├─recruit
    │      │  │  │      list.css
    │      │  │  │      req.css
    │      │  │  │
    │      │  │  ├─seeker
    │      │  │  │  │  myinfo.css
    │      │  │  │  │
    │      │  │  │  └─resume
    │      │  │  │          add.css
    │      │  │  │
    │      │  │  └─user
    │      │  │          confirm_id.css
    │      │  │          confirm_pw.css
    │      │  │          join.css
    │      │  │          login.css
    │      │  │
    │      │  └─js
    │      │      │  common.js
    │      │      │  index.js
    │      │      │
    │      │      ├─community
    │      │      │      add.js
    │      │      │      delete.js
    │      │      │      index.js
    │      │      │      list.js
    │      │      │      read.js
    │      │      │      update.js
    │      │      │
    │      │      ├─offer
    │      │      │  └─jobopening
    │      │      │          add.js
    │      │      │          applylist.js
    │      │      │
    │      │      ├─recruit
    │      │      │      req.js
    │      │      │
    │      │      ├─seeker
    │      │      │  └─resume
    │      │      │          add.js
    │      │      │
    │      │      └─user
    │      │              confirm_id.js
    │      │              confirm_pw.js
    │      │              join.js
    │      │              login.js
    │      │
    │      └─templates
    │          │  index.html
    │          │  login.html
    │          │  template_mainPage.html
    │          │  template_subPage.html
    │          │
    │          ├─community
    │          │      add.html
    │          │      delete.html
    │          │      index.html
    │          │      list.html
    │          │      read.html
    │          │      update.html
    │          │
    │          ├─fragments
    │          │      footer.html
    │          │      link.html
    │          │      nav.html
    │          │      top_header.html
    │          │
    │          ├─notification
    │          │      add.html
    │          │      list.html
    │          │      read.html
    │          │      update.html
    │          │
    │          ├─offer
    │          │  ├─company
    │          │  │      add.html
    │          │  │      delete.html
    │          │  │      read.html
    │          │  │      update.html
    │          │  │
    │          │  ├─jobopening
    │          │  │      add.html
    │          │  │      applylist.html
    │          │  │      delete.html
    │          │  │      list.html
    │          │  │      update.html
    │          │  │
    │          │  └─myinfo
    │          │          read.html
    │          │          update.html
    │          │
    │          ├─recruit
    │          │      list.html
    │          │      req.html
    │          │
    │          ├─seeker
    │          │  │  main.html
    │          │  │
    │          │  ├─myinfo
    │          │  │      read.html
    │          │  │
    │          │  └─resume
    │          │          add.html
    │          │          list.html
    │          │          read.html
    │          │          update.html
    │          │
    │          └─user
    │                  confirm_id.html
    │                  confirm_pw.html
    │                  join.html
    │                  myinfo.html
    │
    └─test
        │  schema.sql
        │
        └─java
            └─com
                └─example
                    └─jobKoreaIt
                        │  JobKoreaItApplicationTests.java
                        │
                        └─domain
                            └─common
                                └─repository
                                        CommunityRepositoryTest.java
```
---
