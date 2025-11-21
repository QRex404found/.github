# 🦖 QREX: RAG 기반 QR코드 피싱 방지 시스템

[![팀명](https://img.shields.io/badge/Team-404%20FOUND-4C4C4C?style=flat-square)](https://www.notion.so/QRex-20e89adac92c802b9355fedbfbbcac9f?source=copy_link)
[![기술 스택](https://img.shields.io/badge/Stack-React%20%7C%20Spring%20Boot-6DB33F?style=flat-square&logo=react)](https://www.notion.so/QRex-20e89adac92c802b9355fedbfbbcac9f?source=copy_link)
[![라이선스](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)

<p align="center">
  <img src="../photo/logo.png" width="48%" style="display: inline-block;" alt="QREX 로고: 돋보기에 QR 코드가 있는 디자인">
  <img src="../photo/dino.png" width="48%" style="display: inline-block;" alt="QREX 마스코트: QR코드 알에서 깨어난 아기 공룡">
</p>

QREX는 의심스러운 QR 코드를 스캔하여 피싱 여부를 판별하는 서비스입니다. 
사용자가 카메라나 갤러리 이미지로 QR을 스캔하면, QREX는 URL을 분석하여 해당 사이트의 유해성을 **실시간으로 알려줍니다.** 검사 결과를 저장하고 커뮤니티에서 피싱 사례를 공유하며 서로 소통할 수 있도록 돕는 사용자 중심의 피싱 예방 시스템입니다.

---

## 💡 서비스 이름: QRex 선정 이유

**QREX**는 'QR' 코드와 최강의 포식자 공룡인 **T-Rex**의 결합입니다. 

T-Rex가 먹이사슬의 모든 위협을 압도했듯, QREX는 교묘하게 숨어있는 QR 피싱 링크를 강력하게 찾아내 제거합니다. 이는 사용자에게 가장 안전한 디지털 경험을 제공하겠다는 저희의 약속을 담은 이름입니다.

---

## ✨ 주요 특징 (Features)

| 카테고리 | 특징 | 설명 |
| :--- | :--- | :--- |
| **핵심 기능** | **실시간 QR 코드 분석** | 카메라나 갤러리 이미지를 통해 QR 코드를 인식하고, URL의 피싱 여부를 즉시 판별합니다. |
| **정확도** | **RAG 기반의 정확한 판별** | **RAG (Retrieval-Augmented Generation) 모델**과 최신 피싱 사례 데이터를 결합하여 분석 정확도를 높였습니다. |
| **커뮤니티** | **피싱 사례 공유** | 사용자들이 피싱 사례를 공유하는 게시판을 통해 피싱을 미연에 방지할 수 있습니다. |
| **개인화** | **기록 관리** | 사용자가 검사한 QR 코드의 기록을 저장하고 언제든지 다시 확인할 수 있습니다. |
| **접근성** | **반응형 웹 디자인** | 다양한 기기에서 최적의 사용 환경을 제공하는 반응형 웹 디자인을 채택했습니다. |

---

## 🛠️ 팀 역할 및 기술 스택

### 👥 팀명: 404 FOUND
> 겉보기에는 오류와 한계로 보이는 상황 속에서도 해결의 실마리를 찾아내고, 존재하지 않는 것처럼 보였던 가능성을 발굴하겠다는 의지를 담았습니다.

| 역할 | 주도자 | 기술 스택 |
| :--- | :--- | :--- |
| **UI** | 최수연, 심연우 | Figma |
| **Frontend** | 심연우, 최수연 | **React.js, shadcn/ui** |
| **Backend** | 김여민, 심연우 | **Spring Boot, JWT, JPA** |
| **DB** | 최수연, 김여민 | MySQL |
| **RAG** | 김여민 | **Spring AI, LangChain** |

> *본 프로젝트는 각 파트의 주도적인 역할을 명시하였으나, 모든 팀원이 기획, 개발, 디자인 등 전 과정에 함께 참여하며 협업을 통해 완성하였습니다.*

---

## ⚙️ 기술 아키텍처 및 상세 구현

QREX는 각기 다른 역할을 하는 **세 개의 주요 시스템**으로 구성되어 있으며, RESTful API를 통해 효율적으로 통신합니다.

### 시스템 구성
| 시스템 | 역할 및 상세 문서 |
| :--- | :--- |
| **프론트엔드 (Frontend)** | 프론트엔드 개발 환경, 컴포넌트 구조, 페이지 라우팅 등 상세 구현 내용 |
| **백엔드 (Backend)** | 백엔드 API 명세, 데이터베이스 모델링, 비즈니스 로직 등 서버 구조 상세 문서 |
| **RAG 모델 (LangChain)** | RAG 모델의 동작 원리, 데이터셋, 분석 로직 등 핵심 기술 상세 문서 |

---

## 📚 프로젝트 상세 자료 (Documentation)

| 자료 구분 | 내용 요약 | 링크/위치 |
| :--- | :--- | :--- |
| **시스템 정의서** | 프로젝트의 전체적인 요약, 주요 기능, 개발 기간, 팀원 정보 | [시스템 정의서](https://github.com/QRex404found/documents/blob/3df098751e2b3dc922981fa9b1210423626b738a/%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%A0%95%EC%9D%98%EC%84%9C.md) |
| **시스템 아키텍처** | 사용자, 프론트, 백, 분석 서버, db 간의 상호작용 다이어그램 | [시스템 아키텍처](https://github.com/QRex404found/documents/blob/3df098751e2b3dc922981fa9b1210423626b738a/system_architecture.png) |
| **기능적 요구사항** | 백엔드와 프론트엔드의 각 기능별 상세 요구사항 | [기능적 요구사항](https://github.com/QRex404found/documents/blob/3df098751e2b3dc922981fa9b1210423626b738a/%EA%B8%B0%EB%8A%A5%EC%A0%81%20%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD.md) |
| **데이터베이스(DB) 스키마** | USER, ANALYSIS, BOARD, COMMENT 테이블의 관계 및 컬럼 정보 | [ERD](https://github.com/QRex404found/documents/blob/6183a878df738e3bfa4420ecde270933a308fdee/db/db.png) |
| **회의록** | 팀 미팅 내용, 주요 결정 사항 및 진행 상황 기록 | [회의록 Repository](https://github.com/QRex404found/meeting_notes) |
| **Figma UI/UX 디자인** | 사용자 인터페이스의 전체적인 레이아웃 및 디자인 | [Figma URL](https://embed.figma.com/design/nLM3q74eSdsI1o1IhpKZ7L/QREX?node-id=0-1&t=aedu6NYkxjKdHAXR-1&embed-host=notion&footer=false&theme=system) |
| **Notion 페이지** | 프로젝트의 모든 상세 자료가 정리된 Notion 페이지 | [Notion URL](https://www.notion.so/QRex-20e89adac92c802b9355fedbfbbcac9f?source=copy_link) |
