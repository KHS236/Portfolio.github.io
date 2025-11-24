# SAMSUNGLIONS 통합 예매 웹 프로젝트

DEVELOPMENT MOTIVATION
---
> 삼성라이온즈 홈페이지
> > 기존의 삼성라이온즈 홈페이지에는 팬들과의 소통창구도 없고 티켓 예매를 하려면 티켓링크라는 사이트에 따로 들어가서 예매를 해야하는 불편함이 있습니다. 그래서 이를 하나의 플랫폼에서 예매하고 팬들과 소통할 수 있는 서비스를 개발하고 싶었습니다.
> > 이런 서비스는 사용자가 다양한 서비스를 즐기는데 도움을 줄 것입니다.
> > 또, 사용자들의 편의를 위해 티켓 예매 과정을 간편하고 효율적으로 만들고, 다양한 옵션과 혜택을 제공하여 사용자들에게 더 나은 서비스를 제공할 것입니다.<br>
 

BRANCH
---
[이종일](http://github.com/jong12mm/SAMSUNGLIONS/tree/이종일) | [정대민](http://github.com/jong12mm/SAMSUNGLIONS/tree/daemin) | [강현우](http://github.com/jong12mm/SAMSUNGLIONS/tree/강현우) | [이건무](http://github.com/jong12mm/SAMSUNGLIONS/tree/이건무) | 


PLANS
---
 |LANGUAGE|PLAN|IMPLEMENT|DESCRIPTION|
 |-|-|-|-|
 |JAVA|-|-|-|
 |JSP/SERVLET|2024/04/24 - 2024/04/28|-|-|
 |SPRING STS3|2024/04/29 ~ 2024/05/03|-|-|
 |SPRING BOOT|2024/06/01 - 2024/06/30|-|-|
 

MEMBERERS
--- 
|NAME|ROLE|DETAILS|DESCRIPTION| 
|---|---|---|---|
|Together|---| FrontController / Document 관리 / Dependencies  관리 |---|
|이종일|조장| 예매 C.R.U.D., 갤러리 C.R.U.D., 전반적인 프론트엔드|---|
|정대민|조원| LOGIN/LOGOUT관련, 토큰 및 쿠키|---|
|강현우|조원| 결제 C.R.U.D., 메인 페이지 제작|---|
|이건무|조원| 게시판 총괄(프론트엔드 포함), 웹 크롤링|---|

SKILLS
---

#### FN
---
<img src="https://img.shields.io/badge/HTML5-3366CC?style=for-the-badge&logo=htmlacademy&logoColor=white"> <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white"> <img src="https://img.shields.io/badge/JQUERY-0769AD?style=for-the-badge&logo=jquery&logoColor=white"> 


#### BN
---
<img src="https://img.shields.io/badge/JAVA-005571?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/JSP-1E8CBE?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SPRING-STS3-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/SPRINGBOOT-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img
src="https://img.shields.io/badge/IntelliJ_IDEA-Ultimate-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">

#### DATABASE
---
<img src="https://img.shields.io/badge/MYSQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">  


#### DEVOPS
---
<img src="https://img.shields.io/badge/GIT-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github2&logoColor=white"> <img src="https://img.shields.io/badge/AWS-EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white">


END POINT DOC
---
|URI|REQUEST METHOD|REQUEST PARAMETER TYPE|RESPONSE VALUE TYPE|DESCRIPTION|
|---|---|---|---|---|
|/book/add|POST|bookid : Long<br>seatid : String<br>name : String<br>gameinfoId : LocalDateTime<br>date : String<br>bookstatus : String<br>payid : String|JSON|예매 추가|
|/book/list|GET|type : String<br>keyword : String<br>pageNo : String|JSON|예매 목록 조회|
|/book/read|GET|---|JSON|예매 상세 정보 조회|
|/book/update|POST|updateIdStr :  Long<br>bookid : Long<br>seatid : String<br>name : String<br>gameinfoId : LocalDateTime<br>date : String<br>bookstatus : String<br>payid : String|JSON|예매 정보 업데이트|
|/book/delete|POST|type : String<br>keyword : String<br>pageNo : String<br>deleteIdStr : String|JSON|예매 삭제|
|/payment/make|POST|paymentId : Long<br>amount : BigDecimal<br>paymentDateTime : LocalDateTime<br>paymentMethod : String<br>paymentStatus : String<br>impUid : String<br>merchantUid : String|JSON|결제 시작|
|/payment/cancel/{impUid}|POST|paymentId : Long<br>amount : BigDecimal<br>cancelAmount : BigDecimal<br>paymentMethod : String<br>paymentStatus : String<br>impUid : String<br>merchantUid : String|JSON|결제 취소|
|/image/add|POST|id : Long<br>name : String<br>title : String<br>data : byte[]<br>extension : String|JSON|갤러리 이미지 추가|
|/image/search|GET|---|JSON|이미지 검색|
|/image/download/{id}|GET|id : Long|JSON|이미지 다운로드|
|/user/add|POST|role : String<br>islocked : boolean<br>addr : String<br>adultphone : String<br>childphone : String<br>birth : LocalDate<br>email : String<br>gender : char<br>membership : String<br>realname : String<br>provider : String<br>providerId : String|JSON|새로운 사용자 추가|
|/user/read|GET|---|JSON|사용자 상세 정보 조회|
|/user/update|POST|---|JSON|사용자 정보 업데이트|
|/user/delete|POST|---|JSON|사용자 삭제|
|/login|POST|username : String<br>password : String|JSON|사용자 로그인|
|/logout|POST|None|JSON|사용자 로그아웃|

DEPENDENCIES LIST
---
### Spring Boot 기본 의존성
- `org.springframework.boot:spring-boot-starter-web`
- `org.springframework.boot:spring-boot-starter-security`
- `org.springframework.boot:spring-boot-starter-oauth2-client`

### JWT (JSON Web Token) 관련 의존성
- `io.jsonwebtoken:jjwt-api:0.11.2`
- `io.jsonwebtoken:jjwt-impl:0.11.2` (runtimeOnly)
- `io.jsonwebtoken:jjwt-jackson:0.11.2` (runtimeOnly)

### Lombok (코드 자동 생성) 관련 의존성
- `org.projectlombok:lombok` (compileOnly)
- `org.projectlombok:lombok` (annotationProcessor)

### Thymeleaf 템플릿 엔진 관련 의존성
- `org.springframework.boot:spring-boot-starter-thymeleaf`
- `org.thymeleaf.extras:thymeleaf-extras-springsecurity6`

### 데이터베이스 및 커넥션 풀 관련 의존성
- `org.springframework.boot:spring-boot-starter-data-jpa`
- `mysql:mysql-connector-java:8.0.33`
- `hikari-cp:hikari-cp:3.0.1`

### 웹 및 서블릿 관련 의존성
- `javax.servlet:jstl:1.2`

### 테스트 관련 의존성
- `org.springframework.boot:spring-boot-starter-test`
- `org.junit.platform:junit-platform-launcher` (testRuntimeOnly)

### XML 및 HTML 파싱 관련 의존성
- `javax.xml.bind:jaxb-api:2.3.1`
- `org.jsoup:jsoup:1.14.3`

### 아임포트 결제 모듈 관련 의존성
- `com.github.iamport:iamport-rest-client-java:0.2.21`



ERD[samsungdb]
---
![20240425155554](https://github.com/jong12mm/SAMSUNGLIONS/blob/%EC%9D%B4%EC%A2%85%EC%9D%BC/sql%ED%8C%8C%EC%9D%BC.png?raw=true)



FILE TREES[SPRING BOOT]
--- 
```
C:.
│  .gitignore
│  build.gradle
│  gradlew
│  gradlew.bat
│  settings.gradle
│
├─.gradle
│
├─.idea
│
├─gradle
│
└─src
    ├─main
    │  ├─generated
    │  ├─java
    │  │  └─com
    │  │      └─example
    │  │          └─sl
    │  │              │  SlApplication.java
    │  │              │
    │  │              ├─config
    │  │              │  │  IamportClientConfig.java
    │  │              │  │  PrincipalDetails.java
    │  │              │  │  PrincipalDetailsOauth2Service.java
    │  │              │  │  PrincipalDetailsService.java
    │  │              │  │  SecurityConfig.java
    │  │              │  │  TxConfig.java
    │  │              │  │  WebMvcConfig.java
    │  │              │  │
    │  │              │  └─auth
    │  │              │      ├─exceptionHandler
    │  │              │      │      AppException.java
    │  │              │      │      CustomAccessDeniedHandler.java
    │  │              │      │      CustomAuthenticationEntryPoint.java
    │  │              │      │      ErrorCode.java
    │  │              │      │      ExceptionManager.java
    │  │              │      │
    │  │              │      ├─jwt
    │  │              │      │      JwtAuthenticationFilter.java
    │  │              │      │      JwtAuthorizationFilter.java
    │  │              │      │      JwtProperties.java
    │  │              │      │      JwtTokenProvider.java
    │  │              │      │      KeyGenerator.java
    │  │              │      │      TokenInfo.java
    │  │              │      │
    │  │              │      ├─loginHandler
    │  │              │      │      CustomAuthenticationFailureHandler.java
    │  │              │      │      CustomLoginSuccessHandler.java
    │  │              │      │      OAuth2JwtLoginSuccessHandler.java
    │  │              │      │
    │  │              │      ├─logoutHandler
    │  │              │      │      CustomLogoutHandler.java
    │  │              │      │      CustomLogoutSuccessHandler.java
    │  │              │      │      SessionCookieClearingLogoutHandler.java
    │  │              │      │
    │  │              │      └─provider
    │  │              │              GoogleUserInfo.java
    │  │              │              KakaoUserInfo.java
    │  │              │              NaverUserInfo.java
    │  │              │              OAuth2UserInfo.java
    │  │              │
    │  │              ├─controller
    │  │              │  │  BookController.java
    │  │              │  │  ClubController.java
    │  │              │  │  FanBoardController.java
    │  │              │  │  FanController.java
    │  │              │  │  HomeController.java
    │  │              │  │  ImageController.java
    │  │              │  │  PasswordController.java
    │  │              │  │  PaymentController.java
    │  │              │  │  PlayerController.java
    │  │              │  │  ProfileController.java
    │  │              │  │  RecordController.java
    │  │              │  │  UserController.java
    │  │              │  │
    │  │              │  ├─detail
    │  │              │  │  │  CheerDetailController.java
    │  │              │  │  │  PitcherDetailController.java
    │  │              │  │  │  StaffDetailController.java
    │  │              │  │  │
    │  │              │  │  └─hitter
    │  │              │  │          CatcherController.java
    │  │              │  │          InfielderController.java
    │  │              │  │          OutfielderController.java
    │  │              │  │
    │  │              │  └─exception
    │  │              │          FileUploadExceptionAdvice.java
    │  │              │          ResourceNotFoundException.java
    │  │              │
    │  │              ├─domain
    │  │              │  ├─dao
    │  │              │  │  └─common
    │  │              │  │          CommonDao.java
    │  │              │  │          ConnectionPool.java
    │  │              │  │          ConnectionPool_ByHikari.java
    │  │              │  │
    │  │              │  ├─dto
    │  │              │  │      BoardDTO.java
    │  │              │  │      BookDto.java
    │  │              │  │      ClubNewsDTO.java
    │  │              │  │      FanBoardDTO.java
    │  │              │  │      FanCommentDTO.java
    │  │              │  │      FaqBoardDTO.java
    │  │              │  │      GameInfoDto.java
    │  │              │  │      ImageDto.java
    │  │              │  │      LoginRequest.java
    │  │              │  │      OAuthUserDto.java
    │  │              │  │      PaymentDto.java
    │  │              │  │      SeatDto.java
    │  │              │  │      UserAdultJoinRequest.java
    │  │              │  │      UserChildJoinRequest.java
    │  │              │  │      UserProfileUpdateRequest.java
    │  │              │  │
    │  │              │  └─service
    │  │              │          BoardService.java
    │  │              │          BookService.java
    │  │              │          BookServiceImpl.java
    │  │              │          ClubNewsService.java
    │  │              │          EmailService.java
    │  │              │          EmailServiceImpl.java
    │  │              │          FanBoardService.java
    │  │              │          FanCommentService.java
    │  │              │          FaqBoardService.java
    │  │              │          ImageService.java
    │  │              │          PaymentService.java
    │  │              │          PaymentServiceImpl.java
    │  │              │          StoryService.java
    │  │              │          UserService.java
    │  │              │
    │  │              ├─entity
    │  │              │      BaseEntity.java
    │  │              │      BoardEntity.java
    │  │              │      BookEntity.java
    │  │              │      ClubNewsEntity.java
    │  │              │      FanBaseEntity.java
    │  │              │      FanBoardEntity.java
    │  │              │      FanCommentEntity.java
    │  │              │      FaqBoardEntity.java
    │  │              │      GameInfoEntity.java
    │  │              │      ImageEntity.java
    │  │              │      LoginedUser.java
    │  │              │      PaymentEntity.java
    │  │              │      SeatEntity.java
    │  │              │      Signature.java
    │  │              │      StoryEntity.java
    │  │              │      User.java
    │  │              │
    │  │              └─repository
    │  │                      BoardRepository.java
    │  │                      BookRepository.java
    │  │                      ClubNewsRepository.java
    │  │                      FanBoardRepository.java
    │  │                      FanCommentRepository.java
    │  │                      FaqBoardRepository.java
    │  │                      GameInfoRepository.java
    │  │                      ImageRepository.java
    │  │                      LoginedUserRepository.java
    │  │                      PaymentRepository.java
    │  │                      SeatRepository.java
    │  │                      SignatureRepository.java
    │  │                      StoryRepository.java
    │  │                      UserRepository.java
    │  │
    │  └─resources
    │      │  application.properties
    │      │
    │      ├─static
    │      │  ├─css
    │      │  ├─data
    │      │  ├─font
    │      │  ├─img
    │      │  └─js
    │      │
    │      └─templates
    │          │  samsung.html
    │          │
    │          ├─book
    │          │      booklist.html
    │          │      book_finish.html
    │          │      book_game_info.html
    │          │      book_real_start.html
    │          │      book_start.html
    │          │      seats_modal.html
    │          │
    │          ├─club
    │          │  │  lionsPark.html
    │          │  │  slhistory.html
    │          │  │  slintro.html
    │          │  │
    │          │  ├─board
    │          │  │      detail.html
    │          │  │      paging.html
    │          │  │      save.html
    │          │  │      update.html
    │          │  │
    │          │  └─clubnews
    │          │          detail.html
    │          │          paging.html
    │          │          save.html
    │          │          update.html
    │          │
    │          ├─detail
    │          │  ├─cheer
    │          │  │      ChaHyomin.html
    │          │  │      JeongYumi.html
    │          │  │      KimGahyun.html
    │          │  │      KimHayeon.html
    │          │  │      KimMiso.html
    │          │  │      KimSangheon.html
    │          │  │      KimYujung.html
    │          │  │      KwonGayoung.html
    │          │  │      LeeSohyeon.html
    │          │  │      LeeSujin.html
    │          │  │      SongYeeun.html
    │          │  │      SungHyoryun.html
    │          │  │
    │          │  ├─hitter
    │          │  │  ├─catcher
    │          │  │  │      KangMinho.html
    │          │  │  │      KimDohwan.html
    │          │  │  │      KimJaeseong.html
    │          │  │  │      LeeByungheon.html
    │          │  │  │
    │          │  │  ├─infielder
    │          │  │  │      AhnJoohyung.html
    │          │  │  │      DavidMacKinnon.html
    │          │  │  │      JeonByeongwoo.html
    │          │  │  │      KimDongjin.html
    │          │  │  │      KimYoungwoong.html
    │          │  │  │      LeeChangyong.html
    │          │  │  │      LeeJaehyeon.html
    │          │  │  │      ParkByungho.html
    │          │  │  │      RyuJihyuk.html
    │          │  │  │
    │          │  │  └─outfielder
    │          │  │          KimDongyub.html
    │          │  │          KimHeongon.html
    │          │  │          KimHyeonjoon.html
    │          │  │          KimJichan.html
    │          │  │          KimSeongyoon.html
    │          │  │          KimTaehoon.html
    │          │  │          KooJawook.html
    │          │  │          LeeSunggyu.html
    │          │  │          YoonJeongbin.html
    │          │  │
    │          │  ├─pitcher
    │          │  │      BaekJunghyun.html
    │          │  │      ChoiHaneul.html
    │          │  │      ChoiJigwang.html
    │          │  │      ChoiSunghoon.html
    │          │  │      ConnorSeabold.html
    │          │  │      DenyiReyes.html
    │          │  │      KimDaewoo.html
    │          │  │      KimJaeyun.html
    │          │  │      KimTaehun.html
    │          │  │      LeeHoseong.html
    │          │  │      LeeSeungmin.html
    │          │  │      LeftSeunghyun.html
    │          │  │      LimChangmin.html
    │          │  │      OhSeunghwan.html
    │          │  │      RightSeunghyun.html
    │          │  │      WonTaein.html
    │          │  │      YookSunyeop.html
    │          │  │
    │          │  └─staff
    │          │          BaeYeongseop.html
    │          │          ChoDongchan.html
    │          │          ChongTaehyon.html
    │          │          ChungMintae.html
    │          │          JongHyunwook.html
    │          │          KangMyunggu.html
    │          │          KwonOhjun.html
    │          │          LeeByungkyu.html
    │          │          LeeJinyoung.html
    │          │          ParkChando.html
    │          │          ParkHanyi.html
    │          │          ParkJinman.html
    │          │          SonJooin.html
    │          │
    │          ├─fan
    │          │  │  fan_cheerdetails.html
    │          │  │  fan_cheermain.html
    │          │  │  fan_gallery.html
    │          │  │  fan_main.html
    │          │  │  fan_story.html
    │          │  │
    │          │  ├─board
    │          │  │      fandetail.html
    │          │  │      fanpaging.html
    │          │  │      fansave.html
    │          │  │      fanupdate.html
    │          │  │
    │          │  └─faqboard
    │          │          detail.html
    │          │          paging.html
    │          │          save.html
    │          │          update.html
    │          │
    │          ├─fragments
    │          │      catcher_detail_slider.html
    │          │      cheer_detail_slider.html
    │          │      footer.html
    │          │      infielder_detail_slider.html
    │          │      nav.html
    │          │      outfielder_detail_slider.html
    │          │      pitcher_detail_slider.html
    │          │      staff_detail_slider.html
    │          │
    │          ├─player
    │          │      hitter.html
    │          │      pitcher.html
    │          │      player_main.html
    │          │      staff.html
    │          │
    │          ├─record
    │          │      teamrank.html
    │          │
    │          └─user
    │                  adult_join.html
    │                  children_join.html
    │                  find_username.html
    │                  find_username_result.html
    │                  forgot-password.html
    │                  join_finish.html
    │                  join_start.html
    │                  login.html
    │                  profile.html
    │                  update-password.html
    │                  update-profile.html
    │
    └─test
        └─java
            └─com
                └─example
                    └─sl
                            SlApplicationTests.java
