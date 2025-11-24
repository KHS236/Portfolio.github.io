# STAY CONNECT(숙박예약웹) 프로젝트

## DEVELOPMENT MOTIVATION
> [!NOTE]
> 숙박 예약 사이트 -
> 
> 학습 및 성장: 웹 애플리케이션 개발에 필요한 기술과 도구를 실습하면서 학습하기 위함이다. Spring Boot, Spring Security, Gradle과 같은 프레임워크와 도구들을 사용하여 실제 프로젝트를 통해 기술을 익히고자 한다.
>
> 실제 프로젝트 경험: 이 프로젝트를 통해 실제 웹 애플리케이션 개발 프로세스를 경험하고, 문제 해결 능력을 향상시키며, 실무에서 발생할 수 있는 다양한 시나리오를 직접 체험할 수 있다.
>
> 포트폴리오 확장: 완성된 프로젝트를 포트폴리오에 추가함으로써, 향후 취업이나 프리랜서 기회를 모색할 때 강력한 경력 자료로 활용할 수 있다.
>
> 기술 스택 탐구: 최신 웹 개발 기술 스택을 탐구하고, 이를 실제 프로젝트에 적용함으로써, 이론과 실습의 차이를 이해하고, 보다 깊이 있는 기술적 역량을 갖추고자 한다.
 

## HISTORY
---
[강지영]() | [윤지원]() | [이재형]() | [조은파]() | 


## PLANS
---
 |LANGUAGE|PLAN|IMPLEMENT|DESCRIPTION|
 |-|-|-|-|
 |JAVA|2024/03/05 ~ 2024/04/23|-|-|
 |JSP/SERVLET|2024/04/24 ~ 2024/05/03|-|-|
 |SPRING STS3|-|-|-|
 |SPRING BOOT|-|-|-|



## MEMBERERS
--- 
|NAME|ROLE|DETAILS|DESCRIPTION| 
|---|---|---|---|
|강지영|BN| reservation - 예약삭제 / 예약수정 |---|
|윤지원|BN| reservation - 예약생성 / 예약목록 |---|
|이재형|BN| member - 로그인 / 로그아웃 / 회원탈퇴 |---|
|조은파|BN| member - 회원등록 / 회원목록 |---|


## 시작가이드
---
#### REQUIREMENTS
---
> [!IMPORTANT]
> 
> ### essential(필수)
> 1. git
> 2. git-flow
> 3. java-version21
> 4. gradle-version8.7
> 5. mysql-version8.3
> 6. docker
> 7. docker-compose

> [!NOTE]
> ### Optional(선택)
> 1. makefile-CLI

## INSTALLATION
---
>[!TIP]
> 
> 1. git clone https://github.com/CATERPILLAR-TEAM/STAY_CONNECT.git
> 2. gh repo clone CATERPILLAR-TEAM/STAY_CONNECT

## ENV FILE
---
>[!IMPORTANT]
>
>## Environment Variables

환경 변수는 애플리케이션의 설정과 비밀 정보를 관리하는 데 사용됩니다. 아래는 사용되는 환경 변수 목록입니다.

| Key                             | Value                  | Description                                              |
|----------------------------------|------------------------|----------------------------------------------------------|
| BASE_URL                         | url                    | 애플리케이션의 기본 URL                                    |
| SERVER_PORT                      | port_num               | 서버가 실행되는 포트 번호                                  |
| JSON_WEB_TOKEN_SECRET_KEY        | secret_key             | JWT 토큰을 서명하기 위한 비밀 키                           |
| JSON_WEB_TOKEN_EXPIRATION_TIME    | time                   | JWT 토큰의 만료 시간                                       |
| JSON_WEB_TOKEN_ISSUER            | issuer                 | JWT 발행자 정보                                            |
| MYSQL_SERVER_URL                 | mysql_server_url       | MySQL 데이터베이스 서버 URL                                 |
| MYSQL_SERVER_USERNAME            | username               | MySQL 서버의 사용자 이름                                   |
| MYSQL_SERVER_PASSWORD            | password               | MySQL 서버의 사용자 비밀번호                               |
| GOOGLE_CLIENT_ID                 | google_client_id       | Google OAuth2 클라이언트 ID                                |
| GOOGLE_CLIENT_SECRET             | google_client_secret   | Google OAuth2 클라이언트 시크릿 키                         |
| PORTONE_API_URL                  | portone_api_url        | PortOne API 엔드포인트 URL                                 |
| PORTONE_API_KEY                  | portone_api_key        | PortOne API를 사용하는 데 필요한 키                        |
| PORTONE_SECRET_KEY               | portone_secret_key     | PortOne API 시크릿 키                                       |
| PRODUCTION_MYSQL_URL             | production_mysql_url   | 프로덕션 환경에서의 MySQL 서버 URL                         |
| PRODUCTION_MYSQL_ROOT_PASSWORD   | password               | 프로덕션 MySQL 서버의 루트 계정 비밀번호                   |
| PRODUCTION_MYSQL_DATABASE        | database               | 프로덕션 환경에서 사용할 데이터베이스 이름                 |
| PRODUCTION_MYSQL_USERNAME        | username               | 프로덕션 MySQL 서버의 사용자 이름                           |
| PRODUCTION_MYSQL_PASSWORD        | password               | 프로덕션 MySQL 서버의 사용자 비밀번호                      |





## HOW TO USER GIT FLOW
---
> [!IMPORTANT]
> ### LOCAL REPOSITORY SETTING GUIDE
> 1. `git clone <git_addr>` or `gh repo clone <git_addr>`
> 2. `git flow init` or `git flow init -f`
> 3. ```bash
>    2번째 명령어 입력시 출력
>    Which branch should be used for bringing forth production releases?
>    - develop
>    - main
>    Branch name for production releases: [main] 
> 
>    Which branch should be used for integration of the "next release"?
>    - develop
>    Branch name for "next release" development: [develop] 
> 
>    How to name your supporting branch prefixes?
>    Feature branches? [feature/] 
>    Release branches? [release/] 
>    Hotfix branches? [hotfix/] 
>    Support branches? [support/] 
>    Version tag prefix? [ver.]
>    ```
> ### feature 추가할 때
> ```bash
> git flow feature start <feature name>
> ```
> 해당 명령어 실행시 현재 브랜치의 위치와 상관없이 develop 브랜치를 기반으로 feature/<feature name> 브랜치 생성
> 기능을 추가해야할 때 사용하면 된다. 평소에 가장 많이 사용될 것으로 기대된다.
> ### 완료한 feature 브랜치 develop 브랜치에 적용
> ```bash
> git flow feature finish <feature name>
> ```
> 해당 명령어 실행시 feature/<feature name> 브랜치를 자동으로 develop 브랜치에 병합한다. 우리는 pull request로 프로젝트를 진행할 예정이기
> 때문에 해당 명령어는 사용할 일이 없을 것 같다.
> 위 명령어 대신 feature/<feature name> 브랜치에서 `gh pr create --base develop --title "Update example feature" --body
> "This pull request updates the feature example."` 형식으로 작성하면 된다.
> 또는 github 웹 사이트에서 pull request 요청을 해도 된다.
> ### 원격 레포지토리에 있는 feature 가져오기
> ```bash
> git flow feature pull origin <feature name>
> ```

## SKILLS
---
| **Category** | **Technologies** |
| ------------ | ---------------- |
| **HTTP ASYNCHRONOUS** | ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white) |
| **WEB SERVER** | ![Apache Tomcat](https://img.shields.io/badge/Apache%20Tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=20232a) |
| **WEB FRAMEWORK** | ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=20232a) ![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=20232a) |
| **BUILD TOOLS** | ![Gradle](https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=20232a) |
| **DATABASE SERVER** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=20232a) |
| **FRONTEND** | ![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=20232a) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=20232a) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=20232a) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=20232a) |
| **CODE EDITOR** | ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=20232a) ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=20232a) |
| **OS** | ![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=20232a) ![Windows 11](https://img.shields.io/badge/Windows%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=20232a) |
| **TERMINAL EMULATOR** | ![iTerm2](https://img.shields.io/badge/iTerm2-000000?style=for-the-badge&logo=iterm2&logoColor=20232a) ![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-4D4D4D?style=for-the-badge&logo=windowsterminal&logoColor=20232a) |
| **SHELL** | ![Zsh](https://img.shields.io/badge/Zsh-428850?style=for-the-badge&logo=gnu-bash&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white) ![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white) |
| **PACKAGE MANAGER** | ![Homebrew](https://img.shields.io/badge/Homebrew-FBB040?style=for-the-badge&logo=homebrew&logoColor=20232a) ![Winget](https://img.shields.io/badge/Winget-0078D4?style=for-the-badge&logo=windows&logoColor=white) |
| **DEVOPS** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=20232a) ![Docker-Compose](https://img.shields.io/badge/Docker--Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Docker Hub](https://img.shields.io/badge/Docker%20Hub-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=20232a) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=20232a) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=20232a) ![Dependabot](https://img.shields.io/badge/Dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=20232a) |
| **MESSENGER** | ![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=20232a) |

## ARCHITECTURE DESIGN

END POINT DOC
---
|URI|REQUEST METHOD|REQUEST PARAMETER TYPE|RESPONSE VALUE TYPE|DESCRIPTION|
|---|---|---|---|---|
|/member/delete|GET/POST|id|boolean|member 탈퇴|
|/member/register|GET/POST|MemberDto|boolean|member 등록|
|/member/update|GET/POST|username, password, email, phone|boolean|member 정보 수정|
|/member/select|GET/POST|username|MemberDto|(관리자)member 상세 조회|
|/member/selectAll|POST|---|List<MemberDto>|(관리자)member 목록 조회|
|/member/login|GET/POST|username, password, session|boolean|member 로그인|
|/member/logout|GET|---|boolean|member 로그아웃|
|---|---|---|---|---|
|/reservation/add|GET/POST|ReservDto|boolean|숙소 예약|
|/reservation/list|GET/POST|userId|ReservDto|member가 예약한 숙소 목록 조회|
|/reservation/update|GET/POST|reservationDto|boolean|member가 예약한 정보 수정|
|/reservation/delete|GET/POST|user_id|boolean|member가 예약한 숙소 취소|
|---|---|---|---|---|

DEPENDENCIES LIST
---
| CAT | NAME                                                               | DESCRIPTION | LINK |
| --- | ------------------------------------------------------------------ | ----------- | ---- |
| FRONTEND | popper.min.js                                                 | Popper.js library for managing popups | [link](https://popper.js.org) |
| FRONTEND | axios                                                         | Promise based HTTP client for the browser | [link](https://axios-http.com) |
| FRONTEND | bootstrap.min.css                                             | Bootstrap CSS framework | [link](https://getbootstrap.com) |
| FRONTEND | bootstrap.min.js                                              | Bootstrap JavaScript framework | [link](https://getbootstrap.com) |
| FRONTEND | fonts.css                                                     | Google Fonts CSS | [link](https://fonts.google.com) |
| FRONTEND | jquery.min.js                                                 | jQuery library | [link](https://jquery.com) |
| FRONTEND | iamport.js                                                    | Iamport library for payment integration | [link](https://www.iamport.kr) |
| FRONTEND | swiper-bundle.min.js                                          | Swiper library for touch sliders | [link](https://swiperjs.com) |
| BACKEND | org.springframework.boot:spring-boot-starter                  | Spring Boot core starter | [link](https://spring.io/projects/spring-boot) |
| BACKEND | org.springframework.boot:spring-boot-starter-data-jpa         | Spring Boot Data JPA starter | [link](https://spring.io/projects/spring-data-jpa) |
| BACKEND | org.springframework.boot:spring-boot-starter-web              | Spring Boot Web starter | [link](https://spring.io/projects/spring-boot) |
| BACKEND | org.springframework.boot:spring-boot-starter-thymeleaf        | Spring Boot Thymeleaf starter | [link](https://spring.io/projects/spring-boot) |
| BACKEND| nz.net.ultraq.thymeleaf:thymeleaf-layout-dialect:3.3.0        | Thymeleaf Layout Dialect | [link](https://github.com/ultraq/thymeleaf-layout-dialect) |
| SECURITY | org.springframework.boot:spring-boot-starter-security         | Spring Boot Security starter | [link](https://spring.io/projects/spring-security) |
| SECURITY | org.springframework.boot:spring-boot-starter-oauth2-client    | Spring Boot OAuth2 Client starter | [link](https://spring.io/projects/spring-security-oauth) |
| SECURITY | org.thymeleaf.extras:thymeleaf-extras-springsecurity6         | Thymeleaf extras for Spring Security 6 | [link](https://www.thymeleaf.org) |
| DATABASE | com.mysql:mysql-connector-j                                   | MySQL Connector for Java | [link](https://dev.mysql.com/doc/connector-j/en/) |
| BUILD TOOLS | org.springframework.boot:spring-boot-starter-validation    | Spring Boot Validation starter | [link](https://spring.io/projects/spring-boot) |
| UTILITIES | io.jsonwebtoken:jjwt-api:0.12.5                              | JSON Web Token API | [link](https://github.com/jwtk/jjwt) |
| UTILITIES | io.jsonwebtoken:jjwt-impl:0.12.5                             | JSON Web Token Implementation | [link](https://github.com/jwtk/jjwt) |
| UTILITIES | io.jsonwebtoken:jjwt-jackson:0.12.5                          | JSON Web Token Jackson Integration | [link](https://github.com/jwtk/jjwt) |
| UTILITIES | org.projectlombok:lombok                                     | Lombok for reducing boilerplate code | [link](https://projectlombok.org) |
| DEVOPS | org.springframework.boot:spring-boot-devtools                   | Spring Boot DevTools | [link](https://spring.io/projects/spring-boot) |
| DEVOPS | org.springframework.boot:spring-boot-docker-compose             | Spring Boot Docker Compose support | [link](https://spring.io/projects/spring-boot) |
| DEVOPS | org.xmlunit:xmlunit-core:2.10.0                                 | XMLUnit core | [link](https://www.xmlunit.org) |
| TESTING | org.springframework.boot:spring-boot-starter-test              | Spring Boot Test starter | [link](https://spring.io/projects/spring-boot) |
| TESTING | org.springframework.security:spring-security-test              | Spring Security Test starter | [link](https://spring.io/projects/spring-security) |
| TESTING | com.h2database:h2                                              | H2 Database | [link](https://www.h2database.com) |
| TESTING | org.junit.platform:junit-platform-launcher                     | JUnit Platform Launcher | [link](https://junit.org/junit5/) |




주요기능
---
- 호텔 조회
- 지도로 검색
- 키워드로 검색
- 호텔 예약 결제
- 호텔 예약 결제 취소

## USECASE[StayConnect]
---
![STAY_CONNECT_USECASE](https://github.com/CATERPILLAR-TEAM/STAY_CONNECT/assets/61113961/64c6410f-7bfa-45ea-82df-8b39aade7344)


## ERD[StayConnect]
---
![image](https://github.com/CATERPILLAR-TEAM/TEST_SERVLET/assets/155939946/fbf64d7c-94e0-4700-b3b9-79e5172d0a4d)

## AWS Structure[StayConnect]
---
<img width="1440" alt="Screenshot 2024-06-25 at 03 05 18" src="https://github.com/user-attachments/assets/3217d916-c692-4299-ade4-94d82760306a">

## Architecture[StayConnect]
---

![StayConnectArchitecture 001](https://github.com/user-attachments/assets/c0e4bd82-53cd-4dc2-a96c-34120f9bea34)

FILE TREES[THYMELEAF/SPRING BOOT]
--- 
```STAY_CONNECT
├── README.md
├── SECURITY.md
├── build.gradle
├── docker
│   ├── docker-compose.mysql.yml
│   ├── docker-compose.yml
│   └── dockerfile
├── gradle
│   └── wrapper
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradlew
├── gradlew.bat
├── makefile
├── settings.gradle
└── src
    ├── main
    │   ├── java
    │   │   └── com
    │   │       └── caterpillars
    │   │           └── StayConnect
    │   │               ├── StayConnectApplication.java
    │   │               ├── component
    │   │               │   ├── entryPoint
    │   │               │   ├── filter
    │   │               │   │   └── JWTAuthenticationFilter.java
    │   │               │   ├── handler
    │   │               │   │   ├── JWTLoginSuccessHandler.java
    │   │               │   │   ├── JWTLogoutSuccessHandler.java
    │   │               │   │   └── OAuth2UserLoginFailureHandler.java
    │   │               │   ├── initializer
    │   │               │   │   ├── TestAccDataInitializer.java
    │   │               │   │   └── TestUserDataInitializer.java
    │   │               │   └── provider
    │   │               │       └── JWTokenProvider.java
    │   │               ├── configuration
    │   │               │   └── SecurityConfig.java
    │   │               ├── controller
    │   │               │   ├── AccommodationController.java
    │   │               │   ├── AdminController.java
    │   │               │   ├── AuthController.java
    │   │               │   ├── ErrorController.java
    │   │               │   ├── ReservationController.java
    │   │               │   ├── URIController.java
    │   │               │   └── UserController.java
    │   │               ├── model
    │   │               │   ├── dto
    │   │               │   │   ├── PaymentDto.java
    │   │               │   │   ├── ReviewDto.java
    │   │               │   │   ├── RoomInfoDto.java
    │   │               │   │   └── UserSignUpDto.java
    │   │               │   ├── entities
    │   │               │   │   ├── Accommodation.java
    │   │               │   │   ├── AccommodationGrade.java
    │   │               │   │   ├── Category.java
    │   │               │   │   ├── Reservation.java
    │   │               │   │   ├── Review.java
    │   │               │   │   ├── Role.java
    │   │               │   │   ├── RoomInfo.java
    │   │               │   │   └── User.java
    │   │               │   └── repository
    │   │               │       ├── AccommodationGradeRepository.java
    │   │               │       ├── AccommodationRepository.java
    │   │               │       ├── CategoryRepository.java
    │   │               │       ├── ReservationRepository.java
    │   │               │       ├── ReviewRepository.java
    │   │               │       ├── RoleRepository.java
    │   │               │       ├── RoomInfoRepository.java
    │   │               │       └── UserRepository.java
    │   │               └── service
    │   │                   ├── AuthService.java
    │   │                   ├── PortOnePaymentService.java
    │   │                   ├── ReservationService.java
    │   │                   ├── ReviewService.java
    │   │                   ├── ReviewServiceImpl.java
    │   │                   └── UserService.java
    │   └── resources
    │       ├── application.properties
    │       ├── static
    │       │   ├── css
    │       │   │   ├── common
    │       │   │   │   ├── footer.css
    │       │   │   │   └── header.css
    │       │   │   ├── layouts
    │       │   │   │   └── layout.css
    │       │   │   └── pages
    │       │   │       ├── accom_detail.css
    │       │   │       ├── admin
    │       │   │       │   ├── reviewList.css
    │       │   │       │   └── userList.css
    │       │   │       ├── auth
    │       │   │       │   ├── signIn.css
    │       │   │       │   └── signUp.css
    │       │   │       ├── index.css
    │       │   │       └── user
    │       │   │           └── myPage.css
    │       │   ├── fonts
    │       │   │   └── fonts.googleapis.woff2
    │       │   ├── img
    │       │   │   ├── StayConnect-main.jpg
    │       │   │   ├── StayConnect_main2.jpg
    │       │   │   ├── StayConnect_main3.jpg
    │       │   │   ├── chat.png
    │       │   │   ├── city
    │       │   │   │   ├── busan.jpg
    │       │   │   │   ├── daegu.jpg
    │       │   │   │   ├── daejeon.jpg
    │       │   │   │   ├── damyang.jpg
    │       │   │   │   ├── gangwon.jpg
    │       │   │   │   ├── gyeongju.jpg
    │       │   │   │   ├── jeju.jpg
    │       │   │   │   ├── jeonju.jpg
    │       │   │   │   ├── pohang.jpg
    │       │   │   │   └── seoul.jpg
    │       │   │   ├── github_logo.png
    │       │   │   ├── google_logo.png
    │       │   │   ├── kakao_logo.png
    │       │   │   ├── logo.svg
    │       │   │   ├── naver_logo.png
    │       │   │   └── notion_logo.png
    │       │   ├── js
    │       │   │   ├── index
    │       │   │   │   ├── index_scroll.js
    │       │   │   │   └── kakaoMapAPI.js
    │       │   │   └── signUp
    │       │   │       ├── checkBoxConsent.js
    │       │   │       └── formatPhoneNumber.js
    │       │   └── lib
    │       │       ├── ajax
    │       │       │   ├── popper.min.js
    │       │       │   └── popper.min.js.map
    │       │       ├── axios
    │       │       │   └── axios.min.js
    │       │       ├── bootstrap
    │       │       │   ├── bootstrap.min.css
    │       │       │   ├── bootstrap.min.css.map
    │       │       │   ├── bootstrap.min.js
    │       │       │   └── bootstrap.min.js.map
    │       │       ├── googleapis
    │       │       │   └── fonts.css
    │       │       ├── jquery
    │       │       │   └── jquery.min.js
    │       │       ├── portone
    │       │       │   └── iamport.js
    │       │       └── swiper
    │       │           ├── swiper-bundle.min.js
    │       │           └── swiper-bundle.min.js.map
    │       └── templates
    │           ├── deprecated
    │           │   ├── 403.html
    │           │   ├── 404.html
    │           │   └── default.html
    │           ├── fragments
    │           │   ├── common
    │           │   │   ├── footer_frag.html
    │           │   │   └── header_frag.html
    │           │   └── index
    │           │       ├── conditionalSection_frag.html
    │           │       └── mainSection_frag.html
    │           ├── layouts
    │           │   └── layout.html
    │           └── pages
    │               ├── admin
    │               │   ├── reviewList.html
    │               │   └── userList.html
    │               ├── auth
    │               │   ├── signIn.html
    │               │   └── signup.html
    │               ├── index.html
    │               └── user
    │                   ├── accom_detail.html
    │                   └── myPage.html
    └── test
        └── java
            └── com
                └── caterpillars
                    └── StayConnect
                        └── StayConnectApplicationTests.java
```
