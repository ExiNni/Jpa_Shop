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
C:. <br>
│  .classpath <br>
│  .gitignore <br>
│  .project <br>
│ <br>
├─bin<br>
│  └─com<br>
│      └─kh<br>
│          └─springdb<br>
│              │  JpaSpringProductApplication.class<br>
│              │  JpaSpringProductApplicationTests.class<br>
│              │<br>
│              ├─config<br>
│              │      SecurityConfig.class<br>
│              │      UserSecurityService.class<br>
│              │<br>
│              ├─controller<br>
│              │      ProductController.class<br>
│              │      UserController.class<br>
│              │<br>
│              ├─model<br>
│              │      Cart$CartBuilder.class<br>
│              │      Cart.class<br>
│              │      CartItem$CartItemBuilder.class<br>
│              │      CartItem.class<br>
│              │      Comment.class<br>
│              │      Order$OrderBuilder.class<br>
│              │      Order.class<br>
│              │      Product$ProductBuilder.class<br>
│              │      Product.class<br>
│              │      SiteUser$SiteUserBuilder.class<br>
│              │      SiteUser.class<br>
│              │      UserCreateForm.class<br>
│              │      UserRole.class<br>
│              │<br>
│              ├─repository<br>
│              │      CartItemRepository.class<br>
│              │      CartRepository.class<br>
│              │      CommentRepository.class<br>
│              │      OrderRepository.class<br>
│              │      ProductRepository.class<br>
│              │      UserRepository.class<br>
│              │<br>
│              └─service<br>
│                      CartService.class<br>
│                      CommentService.class<br>
│                      ProductService.class<br>
│                      UserService.class<br>
│<br>
├─main<br>
│  ├─java<br>
│  │  └─com<br>
│  │      └─kh<br>
│  │          └─springdb<br>
│  │              │  JpaSpringProductApplication.java<br>
│  │              │<br>
│  │              ├─config<br>
│  │              │      SecurityConfig.java<br>
│  │              │      UserSecurityService.java<br>
│  │              │<br>
│  │              ├─controller<br>
│  │              │      ProductController.java<br>
│  │              │      UserController.java<br>
│  │              │<br>
│  │              ├─model<br>
│  │              │      Cart.java<br>
│  │              │      CartItem.java<br>
│  │              │      Comment.java<br>
│  │              │      Order.java<br>
│  │              │      Product.java<br>
│  │              │      SiteUser.java<br>
│  │              │      UserCreateForm.java<br>
│  │              │      UserRole.java<br>
│  │              │<br>
│  │              ├─repository<br>
│  │              │      CartItemRepository.java<br>
│  │              │      CartRepository.java<br>
│  │              │      CommentRepository.java<br>
│  │              │      OrderRepository.java<br>
│  │              │      ProductRepository.java<br>
│  │              │      UserRepository.java<br>
│  │              │<br>
│  │              └─service<br>
│  │                      CartService.java<br>
│  │                      CommentService.java<br>
│  │                      ProductService.java<br>
│  │                      UserService.java<br>
│  │<br>
│  └─resources<br>
│      │  application.properties<br>
│      │<br>
│      ├─static<br>
│      │  └─img<br>
│      │          다누키코지 상점가.jpg<br>
│      │          시로이코이비토 파크.jpg<br>
│      │          오도리공원.jpg<br>
│      │          오타루운하.jpg<br>
│      │<br>
│      └─templates<br>
│              addProductForm.html<br>
│              index.html<br>
│              loginForm.html<br>
│              productDetail.html<br>
│              productList.html<br>
│              product_list.html<br>
│              signupForm.html<br>
│<br>
└─test<br>
    └─java<br>
        └─com<br>
            └─kh<br>
                └─springdb<br>
                        JpaSpringProductApplicationTests.java<br>
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

### 프레임워크
<div style="width: 200px; height: 100px;">
  <img src="https://img.shields.io/badge/Lombok-C8202F?style=for-the-badge&logo=javalogoColor=white" width="180" height="80"> 
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" width="180" height="80">
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
</div>
<br>

## 3. 구현 기능

### 기능 1. 회원 가입
<img src="">
<p align="justify">
회원 (Member)
회원가입 (사업자, 일반 회원) / 로그인 및 로그아웃
</p>
<br>

### 기능 2. 상품 등록
<img src="">
<p align="justify">
상품 (Item)
상품 등록 / 상품 관리 / 상품 수정 / 상품 조회 (메인화면) / 상품 상세 페이지 / 댓글 쓰기
</p>
<br>

### 기능 3. 장바구니
<img src="">
<p align="justify">
장바구니 (Cart)
장바구니 담기 / 장바구니 조회 / 장바구니 삭제 / 장바구니 상품 주문
</p>
<br>

### 기능 4. 검색
<img src="">
<p align="justify">
메인페이지 검색 기능
</p>
<br>

## 4. 피드백

<p align="justify">
4-1. 좋았던 점

4-2. 아쉬웠던 점

</p>

<br>
