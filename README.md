<div align="center">
  <img src="https://img.icons8.com/external-flaticons-flat-flat-icons/64/000000/external-painting-art-and-design-flaticons-flat-flat-icons.png" width="80"/>
  <h1>🎨 Atelier</h1>
  <p>작가와 감상자가 연결되는, 예술 기반 전시 & 커뮤니티 & 커머스 플랫폼</p>

  <p>
    <img src="https://img.shields.io/badge/React-2025-blue?style=flat-square&logo=react" />
    <img src="https://img.shields.io/badge/SpringBoot-Java-green?style=flat-square&logo=springboot" />
    <img src="https://img.shields.io/badge/MySQL-DB-blue?style=flat-square&logo=mysql" />
    <img src="https://img.shields.io/badge/WebSocket-Realtime-ff69b4?style=flat-square" />
    <img src="https://img.shields.io/badge/Zustand-State&nbsp;Management-yellow?style=flat-square" />
    <img src="https://img.shields.io/badge/HuggingFace-AI&nbsp;추천-yellow?style=flat-square&logo=huggingface" />
    <img src="https://img.shields.io/badge/OpenWeather-API-4db8ff?style=flat-square" />
    <img src="https://img.shields.io/badge/AWS-Infra-orange?style=flat-square&logo=amazonaws" />
  </p>
</div>

---

## 📑 목차

- [🧠 프로젝트 소개](#🧠-프로젝트-소개)
- [🎯 주요 기능](#🎯-주요-기능)
- [🛠 주요 기술](#🛠-주요-기술)
- [🧱 시스템 아키텍처](#🧱-시스템-아키텍처)
- [🔗 ERD 설계](#🔗-erd-설계)
- [📂 폴더 구조](#📂-폴더-구조)
- [🧪 실행 방법](#🧪-실행-방법)
- [🖼 화면 설계](#🖼-화면-설계)
- [🙋 팀원 소개](#🙋-팀원-소개)
- [📌 기타 참고](#📌-기타-참고)

---

## 🧠 프로젝트 소개

**Atelier**는 작가와 감상자, 팬들이 예술을 매개로 소통하고 감상하며,  
작품을 구매하고 공유할 수 있는 **온라인 예술 전시 플랫폼**입니다.

> “작품을 넘어, 예술가의 세계와 연결되다.”

- 🧑‍🎨 작가는 전시를 만들고, 팬들과 채팅하며 수익화  
- 🖼 유저는 작품 감상, 좋아요, 구매, 리뷰, 전시회 예약  
- 🛠 관리자는 콘텐츠 관리와 통계 모니터링

---

## 🎯 주요 기능

| 기능 | 설명 |
|------|------|
| 🎨 작품 등록/전시 구성 | 작가 및 유저가 전시를 생성하고 공개 |
| 🛒 굿즈 커머스 | 장바구니, 구매, 리뷰 작성 |
| 💬 실시간 채팅 | WebSocket 기반 작가와 유저의 1:1 소통 |
| 🧾 티켓 예매 | 전시 티켓 예약 및 관리 |
| 📍 AI 추천 | Hugging Face + Naver API로 감성 기반 장소 추천 |
| 🌤 날씨 제공 | 전시 위치 기반 OpenWeather 날씨 정보 |
| 📊 관리자 페이지 | 콘텐츠 승인/삭제, 유저 통계, 신고 관리 |

---

## 🛠 주요 기술

### ✅ Frontend
- React, Zustand, Styled-components, React Router
- WebSocket, Axios
- Visual Studio Code

### ✅ Backend
- Spring Boot, JPA, Spring Security (JWT)
- MySQL, WebSocket(STOMP)
- Scheduler, Gradle, IntelliJ

### ✅ Infra & 외부 API
- AWS EC2, S3, Nginx
- Hugging Face, OpenWeather, Naver API, Google Map

### ✅ 협업 & 문서화
- GitHub, Figma, Notion, ERDCloud

---

## 🧱 시스템 아키텍처

> 📍 프론트부터 백엔드까지 전체 흐름

![Architecture](./docs/architecture.png)

- React + Zustand → Axios → Nginx → Tomcat(Spring Boot) → MySQL  
- WebSocket, JWT 인증, Reverse Proxy, REST API 연동 포함

---

## 🔗 ERD 설계

> 데이터베이스 전체 테이블 및 관계 설계

![ERD](./docs/ERD.png)

- 유저, 작가, 전시, 티켓, 굿즈, 커뮤니티, 알림, 리뷰 등 복합 도메인 구조

---

## 📂 폴더 구조

### 📁 Backend

```bash
📁 artgallery/
├── src/
│   ├── main/
│   │   ├── java/com/dw/artgallery/
│   │   │   ├── config/       # 시큐리티, JWT 등 설정
│   │   │   ├── controller/   # API 컨트롤러
│   │   │   ├── DTO/          # 요청/응답 데이터 전송 객체
│   │   │   ├── enums/        # 열거형 상수
│   │   │   ├── exception/    # 예외 처리
│   │   │   ├── jwt/          # JWT 토큰 처리
│   │   │   ├── model/        # JPA Entity
│   │   │   ├── repository/   # DB 접근 레이어
│   │   │   ├── service/      # 비즈니스 로직
│   │   │   └── ArtgalleryApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── data.sql
│   └── test/...
├── uploads/

```
### 📁 Frontend

```bash
📁 src/
├── api/              # Axios API 모듈
├── assets/           # 정적 이미지 및 폰트
├── components/       # 공통 UI 컴포넌트
├── features/         # 도메인 단위 기능별 컴포넌트
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
├── routes/           # 라우팅 테이블
├── socket/           # WebSocket 관련 모듈
├── styles/           # 전역 스타일, 테마
├── utils/            # 공통 유틸리티
├── App.jsx           # 루트 컴포넌트
├── main.jsx          # 진입점
└── routes.js



