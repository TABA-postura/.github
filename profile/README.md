<div align="center">
  <h1>Postura</h1>
  <p>
    <strong>웹캠을 통한 실시간 자세 분석 시스템</strong><br><br>
  </p>
</div>

## 📜 목차

| 순번 | 항목 |
| :-: | :-: |
| 1 | 팀원 소개 |
| 2 | 서비스 개요 |
| 3 | 서비스 소개 |
| 4 | 기능 플로우차트 |
| 5 | 시스템 아키텍처 |
| 6 | UI / UX |
| 7 | ERD |
| 8 | 트러블슈팅 & 성능 향상 |

</br>

## 1️⃣ 팀원 소개

| _이름_ | 강동규 | 권예진 | 김도연 | 문형주 | 임수경 |
|:-----:|:----:|:-----:|:----:|:----:|:----:|
| ___역할___ | BE | AI | FE | BE | FE |
| ___Github___ | <a href="https://github.com/yswmon"><img src="https://avatars.githubusercontent.com/u/169887881?v=4" width="64" height="64"></a> | <a href="https://github.com/yejin1029"><img src="https://avatars.githubusercontent.com/u/161132495?v=4" width="64" height="64"></a> | <a href="https://github.com/doyeon112"><img src="https://avatars.githubusercontent.com/u/165985343?v=4" width="64" height="64"></a> | <a href="https://github.com/moon4528"><img src="https://avatars.githubusercontent.com/u/166115965?v=4" width="64" height="64"></a> | <a href="https://github.com/sukyungi"><img src="https://avatars.githubusercontent.com/u/165240451?v=4" width="64" height="64"></a> |

</br>

## 2️⃣ 서비스 개요

현대 사회에서 학생과 직장인은 컴퓨터 앞에서 보내는 시간이 폭발적으로 증가했습니다. 장시간의 모니터 사용은 필연적으로 **거북목 및 허리 굽힘**과 같은 잘못된 자세를 유발하며, 이는 만성적인 근골격계 질환과 집중력 저하의 주요 원인이 됩니다.

기존의 자세 교정 솔루션은 고가의 센서 장비나 웨어러블 기기를 요구하여 접근성이 낮았습니다. 또한 근골격계 질환은 스트레칭을 비롯한 관리와 적절한 치료도 중요하지만,  많은 시간과 비용이 요구됩니다. 그렇기에 예방이 무엇보다 중요하며 이를 위해서는 일상생활 속에서 가장 많이 보내는 시간과 장소에서 무심코 하고 있던 잘못된 습관을 고칠 필요가 있습니다. 특히 현대인들은 개인 노트북이나 데스크탑 앞에서 다양한 업무와 학습을 하는 경우가 많기 때문에 해당 시간대의 자세 습관을 피드백 해준다면 효과적일 것입니다. 

본 프로젝트는 **누구나 접근 가능한 노트북 내장 웹캠**과 **컴퓨터 비전 AI 기술**을 활용하여, 별도 장비 없이 실시간으로 사용자에게 정확한 자세 피드백을 제공하는 솔루션 서비스를 개발하고자 합니다.


</br>

## 3️⃣ 서비스 소개

### 🎯 배경 및 문제점
- 인지의 어려움: 대다수의 사람들은 본인이 현재 나쁜 자세를 취하고 있다는 사실을 실시간으로 인지하지 못함.
- 습관 개선의 어려움 : 대다수의 사람들이 본인이 어느정도로 바른 자세를 잘 유지하는지 모름. 
- 데이터 관리 부족: 장기적인 관점에서 나의 자세 습관이 어떻게 개선되고 있는지 확인하기 어려움
한 자기관리 
- 별도 장비 구매 없이 합리적인 솔루션

</br>

## 4️⃣ 기능 플로우차트

![image](https://github.com/user-attachments/assets/cd710cb0-fb79-4b79-9489-771db33cf1f7)

</br>

## 5️⃣ 시스템 아키텍처

![image](https://github.com/user-attachments/assets/a72f3617-b73d-44b9-881f-ade2c53599e8)

</br>

## 6️⃣ UI / UX

![image](https://github.com/user-attachments/assets/47827c9e-2afb-4fb2-be43-872ef58e88ba)
![image](https://github.com/user-attachments/assets/a75693e5-d838-4233-92fd-722a244085ad)
![image](https://github.com/user-attachments/assets/c68af118-fe74-4b5c-9774-18fffbf889c7)
![image](https://github.com/user-attachments/assets/d1ffa048-0ca6-488d-9bb7-653b5ed5f72d)
![image](https://github.com/user-attachments/assets/a1b31d34-6f68-41c2-803c-812b46678173)



</br>

## 7️⃣ ERD

![image](https://github.com/user-attachments/assets/93d33eed-f4fe-49a5-8f1a-58ac6b251a29)

</br>

## 8️⃣ 트러블슈팅 & 성능 향상

### ◽ HTTPS 적용
![image](https://github.com/user-attachments/assets/a1499090-b6fb-4425-af54-52f771dc87b5)
보안을 강화하고 사용자 신뢰를 확보하기 위해 기존 HTTP 접속을 HTTPS로 전환하였다. 기존에는 사용자가 http://jhzlo.world:8080/... 형식으로 직접 접근했으나, 이는 암호화되지 않은 평문 통신으로 보안에 취약했다. 이를 해결하기 위해 인증서를 발급받고, TLS 기반의 HTTPS를 적용하였다.

HTTPS는 데이터를 암호화하여 전송하기 때문에, 외부에서는 내부 데이터를 들여다볼 수 없다. 사용자는 이제 https://jhzlo.world/... 형식으로 443 포트에 접속하며, 이 요청은 Nginx가 수신한다. Nginx는 리버스 프록시 역할을 하며, 복호화된 요청을 내부 Spring Boot 애플리케이션의 8080 포트로 포워딩한다.

이 구조는 통신 보안을 강화할 뿐만 아니라, 추후 로드 밸런싱이나 서비스 확장에도 유리한 기반을 제공한다.

<br>

### ◽ Rest Template -> Web Flux
![image](https://github.com/user-attachments/assets/c50a0773-8700-4b27-8a7f-c867561366bd)
이미지 생성 API인 Stability API를 호출할 때, 특성상 응답을 받기까지 평균 약 8초의 시간이 소요된다. 이는 OpenAPI 호출 과정에서 대부분의 시간이 서버 응답을 기다리는 데 소비됨을 의미하며, 실제 네트워크 응답 분석에서도 Waiting 구간이 전체 시간의 대부분을 차지하고 있다.

기존에는 RestTemplate을 활용한 동기 + Blocking I/O 방식으로 API를 호출했기 때문에, 호출 중 해당 스레드는 응답을 받을 때까지 대기 상태가 되었고, 이는 리소스 낭비로 이어졌다. 특히 응답 시간이 긴 외부 API 호출이 많은 경우, 전체 시스템의 처리 성능에 영향을 주는 병목 현상이 발생할 수 있다.

이를 해결하기 위해 WebClient(WebFlux) 기반의 비동기+ Non-Blocking I/O 방식으로 구조를 전환하였다. 이 방식에서는 API를 호출한 후에도 스레드가 대기하지 않고 제어권을 즉시 반환하여 다른 작업을 계속 수행할 수 있다. 응답이 도착하면 콜백을 통해 결과를 처리하기 때문에 시스템 자원을 효율적으로 사용할 수 있다.

이와 같은 비동기 처리 방식 도입은 응답 시간이 긴 외부 API와 통신할 때 서버의 처리 효율을 높여주며 더 많은 동시 요청을 안정적으로 처리할 수 있는 기반을 마련한다.

<br>

### ◽ 오픈소스 spring-ai 기여

<table>
  <tr>
    <th>Project</th>
    <th>PR</th>
    <th>Commit</th>
    <th>Content</th>
  </tr>
  <tr>
    <td><a href="https://github.com/spring-projects/spring-ai">spring-ai</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/pull/3146">#3146</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/commit/e14e788a47f8962075fb312c62382afc6694ef1f">e14e788</a></td></td>
    <td>add @JsonProperty for response_format to ensure correct JSON map</td>
  </tr>
  <tr>
    <td><a href="https://github.com/spring-projects/spring-ai">spring-ai</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/pull/3188">#3188</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/commit/8a5f68d655608ff4adf11e659c78f61e118c9820">8a5f68d</a></td></td>
    <td>remove redundant samples() method</td>
  </tr>
  <tr>
    <td><a href="https://github.com/spring-projects/spring-ai">spring-ai</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/pull/3146">#3189</a></td>
    <td><a href="https://github.com/spring-projects/spring-ai/commit/2721c9e676572c0dbeba906385b13555936cf66b">2721c9e</a></td></td>
    <td>simplify stylePreset merge logic in StabilityAiImageOptions builder</td>
  </tr>
</table>

<br>

### ◽ 프론트
- 토큰 상태 저장 관련 location state, sessionStorage 혼용 → 상태관리 통일
- Axios Interceptor를 통한 에러 핸들링 일괄 처리
- Vercel 배포 환경 캐싱 및 Lazy 로딩 적용
- API 응답 시 loading 처리 적용 → UX 향상
