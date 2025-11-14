# Hugg Android (Compose)
<img width="100%" alt="image" src="https://github.com/user-attachments/assets/d8398b08-6add-4110-8e3e-8ddcc123f037" />


## 목차

- [프로젝트 개요](#프로젝트-개요)
- [기술 스택](#기술-스택)
- [모듈 구조](#모듈-구조)
- [스크린샷](#스크린샷)
- [로드맵](#로드맵)

---

## 프로젝트 개요

- 기존 안드로이드 UI를 **Jetpack Compose**로 단계적 이전(migration)하기 위한 레포입니다.
- 화면(Presentation) / 도메인 / 데이터 레이어를 분리한 **멀티 모듈 아키텍처**를 채택합니다.

---

## 기술 스택

- **Kotlin**
- **Jetpack Compose**
- **Hilt (DI)**
- **Retrofit + OkHttp, Gson**
- **Kotlin Coroutines / Flow**

> 일부 기능은 별도의 키/설정 파일이 필요할 수 있습니다(예: 외부 로그인, 푸시).

---

## 모듈 구조

- `app`: 앱 실행 진입점과 전역 컴포지션 설정
- `domain`: 엔티티, 인터페이스, 유스케이스 등 핵심 로직
- `data`: `domain` 인터페이스 구현부(예: `Retrofit` 기반 API, 로컬 캐시)
- `feature/*`: 화면 단위 모듈(Compose UI, ViewModel)
- `buildSrc`: 공통 버전/플러그인 관리

## 스크린샷

|홈|캘린더|가계부|
|:-----:|:-----:|:-----:|
<img width="240" alt="Screenshot_1763096593" src="https://github.com/user-attachments/assets/166d352c-f59e-440d-ac7d-db9cd0dc1cf0" />|<img width="240" alt="Screenshot_1763096597" src="https://github.com/user-attachments/assets/38cc7a73-2303-43d7-a2ff-5f3ea7bbe462" />|<img width="240" alt="Screenshot_1763096607" src="https://github.com/user-attachments/assets/58a8a9df-f256-46af-a044-94d96353eda5" />

|데일리|챌린지|마이페이지|
|:-----:|:-----:|:-----:|
<img width="240" alt="Screenshot_1763096600" src="https://github.com/user-attachments/assets/59378ab0-008d-4490-960a-f3e6eef52e80" />|<img width="240" alt="Screenshot_1763096743" src="https://github.com/user-attachments/assets/48ccc2f0-d96c-4004-b753-3e978b3b75c4" />|<img width="240" alt="Screenshot_1763096608" src="https://github.com/user-attachments/assets/7b584aee-cf52-4576-bd60-473a987f6e4f" />





