<div align="center">
  <img src="https://img.icons8.com/external-flaticons-flat-flat-icons/64/000000/external-painting-art-and-design-flaticons-flat-flat-icons.png" width="80"/>
  <h1>🎨 Atelier</h1>
  <p>작가와 감상자가 연결되는, 예술 기반 전시 & 커머스 플랫폼</p>

  <p>
    <img src="https://img.shields.io/badge/React-2025-blue?style=flat-square&logo=react" />
    <img src="https://img.shields.io/badge/Zustand-State&nbsp;Management-yellow?style=flat-square" />
    <img src="https://img.shields.io/badge/Styled--components-CSS--in--JS-ff69b4?style=flat-square" />
    <img src="https://img.shields.io/badge/WebSocket-RealTime-red?style=flat-square" />
    <img src="https://img.shields.io/badge/SpringBoot-API-green?style=flat-square&logo=springboot" />
    <img src="https://img.shields.io/badge/JWT-Authentication-orange?style=flat-square" />
    <img src="https://img.shields.io/badge/AWS-EC2/S3-orange?style=flat-square&logo=amazonaws" />
    <img src="https://img.shields.io/badge/MySQL-Relational&nbsp;DB-blue?style=flat-square&logo=mysql" />
    <img src="https://img.shields.io/badge/HuggingFace-AI&nbsp;추천-yellow?style=flat-square&logo=huggingface" />
    <img src="https://img.shields.io/badge/OpenWeather-API-4db8ff?style=flat-square" />
  </p>
</div>

---

## 📑 목차

- [🧠 프로젝트 소개](#🧠-프로젝트-소개)
- [🎯 주요 기능](#🎯-주요-기능)
- [🛠 주요 기술](#🛠-주요-기술)
- [🧱 시스템 아키텍처](#🧱-시스템-아키텍처)
- [📂 폴더 구조](#📂-폴더-구조)
  - [📁 프론트엔드 구조](#📁-프론트엔드-구조)
  - [📁 백엔드 구조](#📁-백엔드-구조)
- [🧪 실행 방법](#🧪-실행-방법)
- [🖼 화면 미리보기](#🖼-화면-미리보기)
- [🙋 팀원 소개](#🙋-팀원-소개)
- [📌 기타 참고](#📌-기타-참고)

---

## 🧠 프로젝트 소개

**Atelier**는 예술가와 감상자, 팬들이 자유롭게 소통하고 작품을 감상하고 소장할 수 있는  
**온라인 예술 커뮤니티 & 커머스 플랫폼**입니다.

> “작품을 넘어, 예술가의 세계와 연결되다.”

- 작가: 작품 전시, 굿즈 판매, 유저와 실시간 소통  
- 유저: 전시 감상, 댓글, 좋아요, 티켓 구매 및 굿즈 소장  
- 관리자: 콘텐츠 승인, 유저 관리, 통계 확인 등

---

## 🎯 주요 기능

| 기능 | 설명 |
|------|------|
| 🖼 갤러리 | 작가 및 유저의 갤러리 감상, 좋아요/댓글 기능 |
| 🛒 커머스 | 굿즈 구매, 티켓 예매, 장바구니 기능 |
| 💬 실시간 채팅 | WebSocket 기반 실시간 소통 기능 |
| 🔔 실시간 알림 | 댓글/작품 등록/구매 등 실시간 피드백 |
| 🧑 마이페이지 | 내 전시, 좋아요, 구매내역, 프로필 설정 |
| 🧑‍💼 관리자 기능 | 유저/작품 관리, 콘텐츠 승인, 신고 처리 |
| 🧠 AI 추천 기능 | HuggingFace + Naver API로 감성 장소 추천 |
| 🌤 날씨 연동 | 전시 장소 기준 날씨 제공 (OpenWeather API)

---

## 🛠 주요 기술

### ✅ Frontend
- React, Vite, Zustand, Styled-components
- React Router, Axios, WebSocket
- Visual Studio Code

### ✅ Backend
- Java, Spring Boot, Spring Security (JWT)
- JPA (Hibernate), MySQL
- STOMP WebSocket, Scheduler
- Gradle, IntelliJ IDEA

### ✅ Infra & DevOps
- AWS EC2, S3, Nginx
- GitHub Actions, Jenkins

### ✅ External API
- HuggingFace (AI 감성 추천)
- OpenWeather API
- Google Maps
- Naver 검색 API

### ✅ 협업 도구
- GitHub, Notion, Figma, ERDCloud

---

## 🧱 시스템 아키텍처

![Atelier Architecture](./docs/architecture.png)

> *프론트 <-> 백엔드 <-> DB <-> 외부 API 흐름을 명확히 시각화*

---

## 📂 폴더 구조

### 📁 프론트엔드 구조

```bash
📁 src/
├── api/
├── assets/
├── components/
├── features/
│   ├── Artist/
│   ├── ArtistGallery/
│   ├── Drawing/
│   ├── Goods/
│   ├── Notification/
│   ├── TicketPage/
│   ├── chatting/
│   ├── community/
│   ├── mypage/
│   ├── adminpage/
│   └── support/
├── routes/
├── socket/
├── styles/
├── utils/
├── App.jsx
├── main.jsx
└── routes.js

### 📁 백엔드 구조

```bash
📁 artgallery/
├── src/
│   ├── main/
│   │   ├── java/com/dw/artgallery/
│   │   │   ├── config/        # WebSecurity, JWT 필터 설정
│   │   │   ├── controller/    # API 요청 처리
│   │   │   ├── service/       # 비즈니스 로직
│   │   │   ├── repository/    # DB 접근 레이어
│   │   │   ├── model/         # JPA Entity 정의
│   │   │   ├── DTO/           # 요청/응답 객체 정의
│   │   │   ├── jwt/           # JWT 인증 모듈
│   │   │   ├── exception/     # 전역 예외 처리 핸들러
│   │   │   ├── enums/         # Enum 타입 정의
│   │   │   └── ArtgalleryApplication.java  # 메인 실행 진입점
│   │   └── resources/
│   │       ├── application.properties      # 환경변수 설정
│   │       └── data.sql                    # 초기 데이터
│   └── test/java/com/dw/artgallery/       # JUnit 테스트 코드
├── uploads/                # 각 Entity별 업로드 관리 모듈
├── pom.xml                 # Maven 빌드 파일
