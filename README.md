🧘‍♂️ Taba-Postura (포스투라)

AI 기반 실시간 자세 교정 및 개인 맞춤형 리포트 서비스

🏆 2024 프로젝트 경진대회 최우수상 수상작

📌 서비스 아키텍처 (Project Architecture)

사용자의 웹캠 데이터를 실시간으로 분석하여 피드백을 제공하기 위해 저비용 고효율의 클라우드 네이티브 아키텍처를 설계했습니다.

Tip: 이 자리에 AWS 아키텍처 다이어그램 이미지를 넣어주세요.

📂 주요 레포지토리 (Repositories)

우리 프로젝트는 전문성 있는 관리를 위해 역할을 분리하여 운영됩니다.

💻 Backend

핵심 기술: Spring Boot, Spring Security, JPA, MySQL, Redis

주요 기능: 비즈니스 로직, 유저 권한 관리, 일일 통계 집계 배치, 실시간 피드백 데이터 중계

성과: Redis 기반 비동기 처리를 통해 100명 동시 접속 시에도 60ms대의 안정적인 응답 속도 확보

🎨 Frontend

핵심 기술: React, TailwindCSS, WebRTC/Canvas API

주요 기능: 사용자 UI 제공, 1fps 이미지 샘플링 및 전송, 실시간 대시보드 시각화

성과: Web Worker 활용으로 백그라운드 모니터링 최적화 및 사용자 친화적인 7일 Rolling 리포트 구현

🧠 AI-Inference

핵심 기술: FastAPI, MediaPipe, OpenCV, MobileNet v2

주요 기능: 실시간 신체 랜드마크 추출, 7가지 부정 자세 판별 알고리즘

성과: 다중 모델 파이프라인 설계로 0.1초 이내의 빠른 추론 성능 달성

🚀 기술적 의사결정 하이라이트 (Technical Decision)

폴리글랏 저장소 전략: 실시간 데이터는 Redis, 영구 통계는 MySQL로 분리하여 성능과 신뢰성을 동시에 확보했습니다.

비동기 디커플링: AI 분석과 API 조회를 분리하여 무거운 연산이 서비스 전체 성능에 영향을 주지 않도록 설계했습니다.

Stateless 인증: 확장성을 고려하여 별도 저장소 없이 검증 가능한 JWT 무상태 구조를 채택했습니다.

📈 활동 지표 (Organization Stats)

👥 팀원 소개 (Members)

[본인 성함]: 팀장, 풀스택 개발 및 시스템 아키텍처 설계

[팀원 성함]: 백엔드 개발 및 데이터베이스 모델링

[팀원 성함]: 프론트엔드 UI/UX 및 실시간 통신 최적화# .github
