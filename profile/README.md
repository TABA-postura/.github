<div align="center">
  <h1>Postura</h1>
  <p>
    <strong>웹캠을 통한 실시간 자세 분석 시스템</strong><br><br>
  </p>
</div>

## 📜 목차

| 순번 | 항목 |
| :-: | :-: |
| 1 | [팀원 소개](#1) |
| 2 | [서비스 개요](#2) |
| 3 | [서비스 소개](#3) |
| 4 | [기능 플로우차트](#4) |
| 5 | [시스템 아키텍처](#5) |
| 6 | [UI / UX](#6) |
| 7 | [ERD](#7) |
| 8 | [로컬 실행 방법](#8) |
| 9 | [수상 내역](#9) |

</br>

<a id="1"></a>
## 1️⃣ 팀원 소개

| _이름_ | 강동규 | 권예진 | 김도연 | 문형주 | 임수경 |
|:-----:|:----:|:-----:|:----:|:----:|:----:|
| ___역할___ | BE | AI | FE | BE | FE |
| ___Github___ | <a href="https://github.com/donggyu-kang"><img src="https://avatars.githubusercontent.com/u/169887881?v=4" width="64" height="64"></a> | <a href="https://github.com/yejinkw"><img src="https://avatars.githubusercontent.com/u/161132495?v=4" width="64" height="64"></a> | <a href="https://github.com/doyeon112"><img src="https://avatars.githubusercontent.com/u/165985343?v=4" width="64" height="64"></a> | <a href="https://github.com/moon4528"><img src="https://avatars.githubusercontent.com/u/166115965?v=4" width="64" height="64"></a> | <a href="https://github.com/sukyungi"><img src="https://avatars.githubusercontent.com/u/165240451?v=4" width="64" height="64"></a> |

</br>

<a id="2"></a>
## 2️⃣ 서비스 개요

현대 사회에서 학생과 직장인은 컴퓨터 앞에서 보내는 시간이 폭발적으로 증가했다. 장시간의 모니터 사용은 필연적으로 **거북목 및 허리 굽힘**과 같은 잘못된 자세를 유발하며, 이는 만성적인 근골격계 질환과 집중력 저하의 주요 원인이 된다.

근골격계 질환은 예방이 무엇보다 중요하며 이를 위해서는 일상생활 속에서 가장 많이 보내는 시간과 장소에서 무심코 하고 있던 잘못된 습관을 고칠 필요가 있다. 따라 해당 시간대의 자세 습관을 피드백 해준다면 효과적일 것이다.

본 프로젝트는 **누구나 접근 가능한 노트북 내장 웹캠**과 **컴퓨터 비전 AI 기술**을 활용하여, 별도 장비 없이 실시간으로 사용자에게 정확한 자세 피드백을 제공하는 솔루션 서비스를 개발하고자 합니다.


</br>

<a id="3"></a>
## 3️⃣ 서비스 소개

### 🎯 배경 및 문제점
- 인지의 어려움: 대다수의 사람들은 본인이 현재 나쁜 자세를 취하고 있다는 사실을 실시간으로 인지하지 못함.
- 습관 개선의 어려움 : 대다수의 사람들이 본인이 어느정도로 바른 자세를 잘 유지하는지 모름. 
- 데이터 관리 부족: 장기적인 관점에서 나의 자세 습관이 어떻게 개선되고 있는지 확인하기 어려움
한 자기관리 
- 별도 장비 구매 없이 합리적인 솔루션
  
### 👥 END USER
| 항목 | 내용 |
| :--- | :--- |
| **대상 연령대** | 장시간 앉아서 집중하는 10대 후반 ~ 60대 중반 (대학생, 수험생, 사무직 종사자) |
| **주요 활동** | 온라인 강의 수강, 프로그래밍, 문서 작업, 게임, 사무 업무 등 |
| **사용자 니즈** | **1. 거북목/허리 통증 완화:** 바른 자세를 유지하여 피로를 줄이고 싶음.<br>**2. 간편한 사용:** 복잡한 장비 사용 없이 간단하고 직관적으로 피드백을 받고 싶음.<br>**3. 데이터 기반 정보 제공:** 자신의 노력과 개선 정도, 평소 잘못된 자세 습관, 습관에 기반한 적절한 스트레칭 정보 |
| **주요 관심사** | 집중력 유지, 건강 관리, 효율적인 학습/업무 환경 구축 |

### 🧩 주요 기능
1. 회원가입 및 로그인
   - 기본적으로 로컬 회원가입 및 로그인 제공
   - 카카오톡, 구글을 통한 회원가입 및 로그인 제공
2. 실시간 AI 자세 모니터링
   - 웹캠을 통해 사용자의 신체 랜드마크 실시간 추출
   - 7가지 부정 자세(거북목, 어깨 비대칭 등)을 정밀하게 판단
3. 즉각적인 맞춤형 피드백
   - 나쁜 자세가 감지되는 즉시 알림과 코칭 메시지 전달
   - 코칭 메시지를 통해 즉각적인 수정 유도
4. 맞춤형 통계 및 리포트
   - 세션 진행 중 바른 자세 유지율과 경고 횟수를 실시간 수치로 시각화
   - 일간 분석 데이터를 가공해 자세 유형, 변화 추이, 빈도 등 통계 리포트 제공
5. 맞춤형 스트레칭 추천
   - 문제 자세와 스트레칭에 대한 정보 제공
   - 통계 리포트를 바탕으로 맞춤형 스트레칭 콘텐츠 추

### 🚀 기대 효과
- 즉각적인 자세 교정
- 지속적인 습관 개선
- 합리적인 솔루션

</br>

<a id="4"></a>
## 4️⃣ 기능 플로우차트

<img width="638" height="500" alt="image" src="https://github.com/user-attachments/assets/8ebe04b2-a317-47c3-99fe-8c4b01208a32" /></br>
<img width="638" height="500" alt="image" src="https://github.com/user-attachments/assets/d0d486d3-7327-485c-ad82-f1260e42e1ec" />

</br>

<a id="5"></a>
## 5️⃣ 시스템 아키텍처

<img width="638" height="353" alt="postura_systemArchitecture" src="https://github.com/user-attachments/assets/769cd495-79b4-4c20-b2dd-180b464f363c" />


</br>

<a id="6"></a>
## 6️⃣ UI / UX

<img width="638" height="310" alt="image" src="https://github.com/user-attachments/assets/25beef56-32a4-4bf8-9116-2cbf24b1adeb" />
<img width="638" height="297" alt="image" src="https://github.com/user-attachments/assets/4c670679-1db3-46c2-9f54-5aa33295a692" />
<img width="638" height="320" alt="image" src="https://github.com/user-attachments/assets/5f6ce612-cf5f-406f-bf35-e87b6ec8ad64" />
<img width="638" height="325" alt="image" src="https://github.com/user-attachments/assets/267d9d50-6aaa-456c-88a4-b4fc69b3f7a8" />
<img width="638" height="335" alt="image" src="https://github.com/user-attachments/assets/de8b5462-35ec-4769-8741-af44b1dd592f" />
<img width="638" height="320" alt="image" src="https://github.com/user-attachments/assets/c8470e58-c990-4185-a688-f9409389b448" />
<img width="638" height="360" alt="image" src="https://github.com/user-attachments/assets/57e57dd6-876a-4330-bf74-c1fdd91a8556" />
<img width="638" height="310" alt="image" src="https://github.com/user-attachments/assets/793a5ff7-9b4f-41ec-8dce-ba9b07ba6865" />
<img width="638" height="300" alt="image" src="https://github.com/user-attachments/assets/b49db0aa-17e5-4586-afd0-c7fa0ea2724c" />
<img width="638" height="321" alt="image" src="https://github.com/user-attachments/assets/5a3236a7-caf6-42d8-9c6e-2a915d3fafaf" />
<img width="638" height="371" alt="image" src="https://github.com/user-attachments/assets/25fb8ef8-7971-48ed-9fc3-fd846b962171" />
<img width="638" height="305" alt="image" src="https://github.com/user-attachments/assets/e007d42e-461c-4b49-b665-384d092a699c" />

</br>

<a id="7"></a>
## 7️⃣ ERD

<img width="900" height="750" alt="image" src="https://github.com/user-attachments/assets/c2049fb5-8edd-4554-bba1-7ee3d9ce93cf" />

</br>

<a id="8"></a>
## 8️⃣ 로컬 실행 방법

3개 서비스(백엔드·AI·프론트)를 로컬에서 한 번에 실행할 수 있습니다. **소셜 로그인을 제외한 모든 기능**이 동작합니다.

### 📦 사전 준비
| 프로그램 | 비고 |
| :--- | :--- |
| **Docker Desktop** | 실행(켜둔) 상태. MySQL·Redis·AI를 자동으로 띄웁니다 |
| **JDK 17** | 백엔드 빌드용 |
| **Node.js 18+** | 프론트엔드용 |

> MySQL·Redis는 **설치할 필요 없습니다.** Docker가 자동 생성합니다.

### 📁 폴더 구조
3개 레포를 아래처럼 배치합니다. (상위·백엔드·프론트 폴더 이름은 자유, **`AI` 폴더 이름만 고정**)
```
📁 postura/                (상위 폴더 - 이름 자유)
├─ docker-compose.yml      ⚠️ AI 폴더와 같은 위치
├─ AI/                     ⚠️ 폴더 이름 반드시 "AI"
├─ Backend/                (이름 자유)
└─ Frontend/               (이름 자유)
```
```bash
# 상위 폴더에서 3개 레포 클론
git clone https://github.com/TABA-postura/Backend.git Backend
git clone https://github.com/TABA-postura/Frontend.git Frontend
git clone https://github.com/TABA-postura/AI.git AI   # 폴더명 반드시 AI
```

### ⚙️ 설정 파일 (최초 1회)

**1) 상위 폴더에 `docker-compose.yml` 생성**
<details>
<summary>docker-compose.yml 내용 펼치기</summary>

```yaml
services:
  mysql:
    image: mysql:8.0
    container_name: postura-mysql
    environment:
      MYSQL_ROOT_PASSWORD: "postura"
      MYSQL_DATABASE: postura
      TZ: Asia/Seoul
    ports:
      - "3307:3306"
    command: --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci
    volumes:
      - postura-mysql-data:/var/lib/mysql
    healthcheck:
      test: ["CMD", "mysqladmin", "ping", "-h", "localhost", "-ppostura"]
      interval: 5s
      timeout: 5s
      retries: 20

  redis:
    image: redis:7-alpine
    container_name: postura-redis
    ports:
      - "6379:6379"

  ai:
    build: ./AI
    container_name: postura-ai
    ports:
      - "8000:8000"
    working_dir: /app
    command: uvicorn app.main:app --host 0.0.0.0 --port 8000 --app-dir src
    environment:
      SPRING_BASE_URL: "http://host.docker.internal:8080"
      SPRING_AI_LOG_PATH: "api/ai/log"
      LOG_LEVEL: "INFO"
    extra_hosts:
      - "host.docker.internal:host-gateway"

volumes:
  postura-mysql-data:
```
</details>

**2) 프론트엔드 `app/frontend/.env.development.local` 생성**
```
VITE_API_BASE_URL=http://localhost:8080
VITE_AI_BASE_URL=http://localhost:8000
```

> 백엔드 로컬 설정(`application-local.properties`)은 **Backend 레포에 이미 포함**되어 있어 따로 만들 필요가 없습니다.

### ▶️ 실행 (터미널 3개)
> 순서: **Docker Desktop 켜기 → ① 인프라 → ② 백엔드 → ③ 프론트**

```bash
# ① 인프라 (MySQL + Redis + AI) — 상위 폴더에서
docker compose up -d
# 최초 1회는 AI 이미지 빌드에 5~10분 소요 (TensorFlow). 이후엔 수 초.
```
```bash
# ② 백엔드 — Backend 폴더에서
./gradlew bootRun --args='--spring.profiles.active=local'
# ⚠️ --spring.profiles.active=local 꼭 붙이기
```
```bash
# ③ 프론트엔드 — Frontend 폴더에서 (새 터미널)
npm install   # 최초 1회
npm run dev
```

### 🌐 접속
브라우저에서 **http://localhost:3000** 접속
1. 이메일로 회원가입 → 로그인
2. 모니터링 시작 → 웹캠 권한 허용
3. 실시간 자세 분석 · 피드백 · 통계 확인

### ⏹️ 종료 / 초기화
```bash
docker compose down      # 인프라 종료 (데이터 유지)
docker compose down -v   # 인프라 종료 + DB 완전 초기화
```
백엔드·프론트는 각 터미널에서 `Ctrl + C`.

### 🛠️ 자주 나는 문제
| 증상 | 해결 |
| :--- | :--- |
| 백엔드가 원격(AWS) DB/Redis로 붙으려 함 | `--spring.profiles.active=local` 누락 |
| `docker compose`가 AI를 못 찾음 | AI 폴더 이름이 `AI`인지, compose와 같은 위치인지 확인 |
| 포트 충돌(3307·8080·3000) | 해당 포트를 쓰는 다른 프로세스 종료 |
| 소셜 로그인(구글/카카오) 안 됨 | 로컬에선 기본 비활성 → 이메일 로그인 사용 |

<a id="9"></a>
## 9️⃣ 수상 내역

### 🥇 2025 대학·기업 협력형 SW아카데미사업 (TABA 10기)
- **수상:** 최우수상 (1등)
- **주관:** TABA아카데미사업단
- **선정:** 총 6팀 중 1팀 선정
- **일자:** 2025-12-23
<br/>
