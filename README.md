# JPA로 구현한 쇼핑몰

<p align="center">
  <br>
  <img src="https://github.com/ExiNni/semi_EJ/blob/master/%EB%96%A0%EB%82%98%EC%A1%B0%20%EB%A9%94%EC%9D%B8.PNG">
  <br>
</p>

## 0. 목차
1. 프로젝트 소개
2. 기술 스택
3. 구현 기능
4. 피드백

## 1. 프로젝트 소개

<p align="justify">
프로젝트를 만들게 된 개요나 동기를 작성해주세요.
</p>
<br>

<p align="justify">
C:.
│  .classpath
│  .gitignore
│  .project
│
├─bin
│  └─com
│      └─kh
│          └─springdb
│              │  JpaSpringProductApplication.class
│              │  JpaSpringProductApplicationTests.class
│              │
│              ├─config
│              │      SecurityConfig.class
│              │      UserSecurityService.class
│              │
│              ├─controller
│              │      ProductController.class
│              │      UserController.class
│              │
│              ├─model
│              │      Cart$CartBuilder.class
│              │      Cart.class
│              │      CartItem$CartItemBuilder.class
│              │      CartItem.class
│              │      Comment.class
│              │      Order$OrderBuilder.class
│              │      Order.class
│              │      Product$ProductBuilder.class
│              │      Product.class
│              │      SiteUser$SiteUserBuilder.class
│              │      SiteUser.class
│              │      UserCreateForm.class
│              │      UserRole.class
│              │
│              ├─repository
│              │      CartItemRepository.class
│              │      CartRepository.class
│              │      CommentRepository.class
│              │      OrderRepository.class
│              │      ProductRepository.class
│              │      UserRepository.class
│              │
│              └─service
│                      CartService.class
│                      CommentService.class
│                      ProductService.class
│                      UserService.class
│
├─main
│  ├─java
│  │  └─com
│  │      └─kh
│  │          └─springdb
│  │              │  JpaSpringProductApplication.java
│  │              │
│  │              ├─config
│  │              │      SecurityConfig.java
│  │              │      UserSecurityService.java
│  │              │
│  │              ├─controller
│  │              │      ProductController.java
│  │              │      UserController.java
│  │              │
│  │              ├─model
│  │              │      Cart.java
│  │              │      CartItem.java
│  │              │      Comment.java
│  │              │      Order.java
│  │              │      Product.java
│  │              │      SiteUser.java
│  │              │      UserCreateForm.java
│  │              │      UserRole.java
│  │              │
│  │              ├─repository
│  │              │      CartItemRepository.java
│  │              │      CartRepository.java
│  │              │      CommentRepository.java
│  │              │      OrderRepository.java
│  │              │      ProductRepository.java
│  │              │      UserRepository.java
│  │              │
│  │              └─service
│  │                      CartService.java
│  │                      CommentService.java
│  │                      ProductService.java
│  │                      UserService.java
│  │
│  └─resources
│      │  application.properties
│      │
│      ├─static
│      │  └─img
│      │          다누키코지 상점가.jpg
│      │          시로이코이비토 파크.jpg
│      │          오도리공원.jpg
│      │          오타루운하.jpg
│      │
│      └─templates
│              addProductForm.html
│              index.html
│              loginForm.html
│              productDetail.html
│              productList.html
│              product_list.html
│              signupForm.html
│
└─test
    └─java
        └─com
            └─kh
                └─springdb
                        JpaSpringProductApplicationTests.java
</p>


## 2. 기술 스택

### 개발언어
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white" width="180" height="80"> 
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white" width="180" height="80">
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white" width="180" height="80">
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" width="180" height="80"> 
  <img src="https://img.shields.io/badge/bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" width="180" height="80">
</div>

<br>

### 데이터베이스
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white" width="180" height="80">
</div>
<br>

### 개발 도구
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipseide&logoColor=white" width="180" height="80">
  <img src="https://img.shields.io/badge/VS_CODE-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white" width="180" height="80">
</div>
<br>

### 서버
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/apache tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=white" width="180" height="80">
</div>
<br>

### 협업 툴
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white" width="180" height="80">
  <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white" width="180" height="80">
</div>
<br>

## 3. 구현 기능

### 기능 1
<img src="">
<p align="justify">
설명란
</p>
<br>

### 기능 2
<img src="">
<p align="justify">
설명란
</p>
<br>

### 기능 3
<img src="">
<p align="justify">
설명란
</p>
<br>

### 기능 4
<img src="">
<p align="justify">
설명란
</p>
<br>

## 4. 피드백

<p align="justify">
4-1. 좋았던 점

4-2. 아쉬웠던 점

</p>

<br>
