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
- [🛠️ 주요 기술](#🛠️-주요-기술)
- [🧱 시스템 아키텍처](#🧱-시스템-아키텍처)
- [📂 폴더 구조](#📂-폴더-구조)
- [🧪 실행 방법](#🧪-실행-방법)
- [🖼 화면 미리보기](#🖼-화면-미리보기)
- [🙋 팀원 소개](#🙋-팀원-소개)
- [📌 기타 참고](#📌-기타-참고)

---

## 🧠 프로젝트 소개

**Atelier**는 예술가와 감상자, 팬들이 자유롭게 소통하고 작품을 감상하고 소장할 수 있는  
**온라인 예술 커뮤니티 & 커머스 플랫폼**입니다.

> “작품을 넘어, 예술가의 세계와 연결되다.”

- 작가는 자신의 작품을 전시하고 굿즈를 판매하며,  
- 유저는 갤러리를 감상하고 좋아요/댓글/채팅을 통해 소통합니다.  
- 더 나아가 티켓 예매와 굿즈 구매까지 이어지는 몰입형 경험을 제공합니다.

---

## 🎯 주요 기능

| 카테고리 | 기능 설명 |
|----------|------------|
| 🖼 갤러리 | 작가/유저 전시, 좋아요, 댓글, 작품 상세 조회 |
| 🛒 커머스 | 굿즈 장바구니, 구매, 전시 티켓 예매 |
| 💬 실시간 채팅 | WebSocket 기반 채팅 (1:1 or 커뮤니티형) |
| 🔔 알림 시스템 | 댓글/작품 등록/구매 등 실시간 피드백 제공 |
| 🧑 마이페이지 | 내 전시, 좋아요한 콘텐츠, 구매 내역 관리 |
| 🧑‍💼 관리자 기능 | 유저 관리, 콘텐츠 승인/삭제, 통계/신고 처리 |
| 📍 AI 추천 | Hugging Face + Naver API 기반 장소 추천 |
| 🌤 날씨 API | 전시장 기반 날씨 정보 제공 (OpenWeather API)

---

## 🛠️ 주요 기술

### 1. Frontend
- React, Vite, React Router
- Zustand (전역 상태 관리)
- Styled-components
- Axios, WebSocket (실시간 기능)
- Visual Studio Code

### 2. Backend
- Java, Spring Boot
- Spring Security (JWT 인증)
- JPA (Hibernate)
- MySQL
- WebSocket (STOMP)
- @Scheduled (예약 태스크)
- Gradle, IntelliJ IDEA

### 3. Storage & Infra
- MySQL
- AWS EC2 & S3
- Nginx
- GitHub Actions, Jenkins

### 4. External API & AI
- Google Map API
- OpenWeather API
- Hugging Face (AI 장소 추천)
- Naver 검색 API

### 5. 협업 도구
- GitHub, Notion, Figma, ERDCloud

---

## 🧱 시스템 아키텍처

![Atelier Architecture](./docs/architecture.png)

> *프론트 → 백엔드 → DB → 외부 API 흐름을 시각적으로 표현*

---

## 📂 폴더 구조

```bash
📁 src/
├── api/
├── assets/
├── components/
├── features/
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
│   └── support/
├── routes/
├── socket/
├── styles/
├── utils/
├── App.jsx
├── main.jsx
└── routes.js
