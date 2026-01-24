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
| 8 | [수상 내역](#8) |

</br>

<a id="1"></a>
## 1️⃣ 팀원 소개

| _이름_ | 강동규 | 권예진 | 김도연 | 문형주 | 임수경 |
|:-----:|:----:|:-----:|:----:|:----:|:----:|
| ___역할___ | BE | AI | FE | BE | FE |
| ___Github___ | <a href="https://github.com/yswmon"><img src="https://avatars.githubusercontent.com/u/169887881?v=4" width="64" height="64"></a> | <a href="https://github.com/yejin1029"><img src="https://avatars.githubusercontent.com/u/161132495?v=4" width="64" height="64"></a> | <a href="https://github.com/doyeon112"><img src="https://avatars.githubusercontent.com/u/165985343?v=4" width="64" height="64"></a> | <a href="https://github.com/moon4528"><img src="https://avatars.githubusercontent.com/u/166115965?v=4" width="64" height="64"></a> | <a href="https://github.com/sukyungi"><img src="https://avatars.githubusercontent.com/u/165240451?v=4" width="64" height="64"></a> |

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
## 8️⃣ 수상 내역

### 🥇 TABA 아카데미 10기 프로젝트 발표회
- **수상:** 최우수상 (1등)
- **주관:** TABA 아카데미 사업단
- **선정:** 총 5팀 중 1팀 선정

<details>
  <summary> <b><i>상장 펼쳐보기</i></b> </summary>

  <img width="300" alt="image" src="https://github.com/user-attachments/assets/ba6513c8-4952-43b0-b688-bbac99698378" />

</details>

<br/>
