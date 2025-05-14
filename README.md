<div align="center">
  <h1>🎨 Atelier</h1>
  <p>작가와 감상자가 연결되는, 예술 기반 전시 & 커머스 플랫폼</p>

  <!-- 🎖 배지 라인 삽입 -->
  <p align="center">
    <img src="https://img.shields.io/badge/React-2025-blue?style=flat-square&logo=react" />
    <img src="https://img.shields.io/badge/Zustand-State&nbsp;Management-yellow?style=flat-square" />
    <img src="https://img.shields.io/badge/Styled--components-CSS--in--JS-ff69b4?style=flat-square" />
    <img src="https://img.shields.io/badge/WebSocket-RealTime-red?style=flat-square" />
    <img src="https://img.shields.io/badge/SpringBoot-API-green?style=flat-square&logo=springboot" />
    <img src="https://img.shields.io/badge/JWT-Authentication-orange?style=flat-square" />
    <img src="https://img.shields.io/badge/MySQL-Relational&nbsp;DB-blue?style=flat-square&logo=mysql" />
    <img src="https://img.shields.io/badge/AWS-EC2/S3-orange?style=flat-square&logo=amazonaws" />
    <img src="https://img.shields.io/badge/Nginx-ReverseProxy-darkgreen?style=flat-square&logo=nginx" />
    <img src="https://img.shields.io/badge/GitHubActions-CI/CD-blue?style=flat-square&logo=githubactions" />
    <img src="https://img.shields.io/badge/HuggingFace-AI&nbsp;추천-yellow?style=flat-square&logo=huggingface" />
    <img src="https://img.shields.io/badge/OpenWeather-API-4db8ff?style=flat-square" />
  </p>
</div>

---

## 📑 목차

- [🧠 프로젝트 소개](#🧠-프로젝트-소개)
- [🎯 주요 기능](#🎯-주요-기능)
- [🛠️ 주요 기술](#🛠️-주요-기술)
- [📂 폴더 구조](#📂-폴더-구조)
- [🧪 실행 방법](#🧪-실행-방법)
- [🖼 화면 미리보기](#🖼-화면-미리보기)
- [🙋 팀원 소개](#🙋-팀원-소개)
- [📌 기타 참고](#📌-기타-참고)

---

## 🧠 프로젝트 소개

**Atelier**는 예술가와 감상자, 팬들이 자유롭게 소통하고 작품을 감상하고 소장할 수 있는  
**온라인 예술 커뮤니티 & 커머스 플랫폼**입니다.

> "작품을 넘어, 예술가의 세계와 연결되다."

- 작가는 온라인 갤러리를 통해 작품을 전시하고 판매하며,  
- 사용자는 다양한 전시를 감상하고 작가와 소통하며, 굿즈 및 티켓을 구매할 수 있습니다.

---

## 🎯 주요 기능

| 기능 | 설명 |
|------|------|
| 🖼 갤러리 | 작가 및 유저의 갤러리 감상, 좋아요/댓글 기능 |
| 🛒 커머스 | 굿즈 구매, 티켓 예매, 장바구니 기능 |
| 💬 실시간 채팅 | 작가와 1:1 또는 커뮤니티 기반 소통 기능 |
| 🔔 실시간 알림 | 작품 등록, 댓글, 구매 등 주요 이벤트 알림 |
| 🧑 마이페이지 | 내가 등록한 작품, 좋아요, 구매 내역 확인 |
| 🧑‍💼 관리자 페이지 | 유저 관리, 콘텐츠 승인/삭제, 통계, 신고 처리 |
| 📍 AI 기반 장소 추천 | Hugging Face + Naver 검색 API로 감성 장소 추천 |
| 🌤 날씨 API 연동 | OpenWeather API 기반 실시간 지역 날씨 표시 |

---

## 🛠️ 주요 기술

### 1. Frontend
- **React**  
- **JavaScript (ES6+)**  
- **Zustand** – 전역 상태 관리  
- **Styled-components** – CSS-in-JS  
- **React Router** – SPA 라우팅  
- **Axios** – RESTful API 연동  
- **WebSocket** – 실시간 알림/채팅 처리  
- **Visual Studio Code**

### 2. Backend
- **Java**, **Spring Boot**  
- **Spring Security + JWT** – 인증/인가  
- **JPA (Hibernate)** – ORM 기반 DB 연동  
- **MySQL** – 관계형 DB  
- **WebSocket (STOMP)** – 실시간 통신  
- **@Scheduled** – 예약 태스크  
- **Gradle**, **IntelliJ IDEA**

### 3. Storage & Infra
- **MySQL**  
- **AWS EC2** – 배포 서버  
- **Nginx** – 리버스 프록시 및 정적 자원 처리  
- **GitHub Actions**, **Jenkins** – CI/CD 자동화

### 4. External API & AI
- **Google Map API** – 지도 표시  
- **OpenWeather API** – 날씨 정보  
- **Hugging Face** – 감성 분석 기반 장소 추천 모델  
- **Naver 검색 API** – 장소 키워드 확장

### 5. 협업 & 개발 도구
- **GitHub** – 코드 버전 관리 및 협업  
- **Notion** – 회의록 및 기획 공유  
- **Figma** – UI 디자인 및 프로토타이핑  
- **ERDCloud** – ERD 설계 시각화

---

## 📂 폴더 구조

```bash
📁 src/
├── api/                    # API 요청 함수 모음
├── assets/                 # 이미지, 폰트 등 정적 파일
├── components/             # 공통 UI 컴포넌트
├── features/               # 기능 단위 컴포넌트 및 비즈니스 로직
│   ├── Artist/
│   ├── ArtistGallery/
│   ├── ArtistGalleryDetail/
│   ├── Drawing/
│   ├── Gallery/
│   ├── Goods/
│   ├── Notification/
│   ├── TicketPage/
│   ├── UserGallery/
│   ├── UserGalleryDetail/
│   ├── adminpage/
│   ├── cart/
│   ├── chatting/
│   ├── community/
│   ├── home/
│   ├── mypage/
│   ├── support/
│   │   ├── Footer.jsx
│   │   ├── Header.jsx
│   │   ├── Logolcon.jsx
│   │   ├── PurchaseCompleted.jsx
│   │   └── TopButton.jsx
├── routes/                 # 라우터 설정
├── socket/                 # WebSocket 모듈
├── styles/                 # 전역 스타일 및 테마 정의
├── utils/                  # 공통 유틸리티 함수
├── App.jsx                 # 루트 컴포넌트
├── main.jsx                # 진입점
└── routes.js               # 라우팅 테이블
