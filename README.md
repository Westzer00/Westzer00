# Seoyeong Kim

Computer Engineering @ Gachon University  
**Applied AI · AI Service Development · Backend Engineering**

실제 업무에서 생성되는 데이터를 연결하고, **AI가 낸 결과를 검증하며 필요한 기능을 API와 서비스로 구현**하는 개발에 관심이 있습니다.

- 데이터 품질 검수부터 RAG·LLM 워크플로우와 기존 플랫폼 백엔드 개선까지 경험
- 제조업 현업 데이터와 MES를 연결하는 AI 조회·자동화 플랫폼 개발·운영
- 프로젝트의 문제와 설계 판단, 구현 코드, 테스트를 확인할 수 있도록 정리

## Selected Engineering Work

### 🏭 BLI — Manufacturing Data Integration & AI Platform

**2026.09 – 현재 · 2인 개발 · 실제 기업 업무에 적용**

- 제조기업의 발주·입고·생산·수출·회계 데이터를 업무 개체와 관계로 모델링하고 기존 MES와 연결
- TypeScript, React/Next.js, Cloudflare Workers 기반 웹·API 및 OpenAI API 연동
- 권한별 업무 조회, 원천 근거 확인, 문서 처리 자동화 및 중복·미확정 데이터 관리 기능 구현
- 실제 기업 내부 코드와 거래 정보는 공개하지 않음. 화면 자료는 공개 가능 범위를 구분해 별도 포트폴리오로 정리

### 🔁 EXEM — LOOP Backend & PHISIGHT Workflow

**2026.07 – 2026.10 · 5인 기업연계 프로젝트**

- RAG 검색 → 유형 분류 → LLM 생성 → 결과 검수로 이어지는 AI 워크플로우 개발 참여
- 기존 AI 플랫폼 LOOP의 내부 출력 전달 한계를 분석하고, Python 입·출력 바인딩 및 이전 회차 결과 전달 로직 개선·테스트에 참여
- PHISIGHT의 초기 화면 구조·사용자 흐름을 설계하고 상세 UI를 2인 공동 구현
- 기업 원본 플랫폼과 팀 UI·서버 코드는 비공개이며, 개인 기여를 설명하는 독립 예제를 별도로 구성

### 🛡 Voice Phishing STT QC & Human Review Pipeline
[Repository](https://github.com/Westzer00/voice-phishing-stt-qc-pipeline)

- **511건** 통화 STT (읽기 가능한 509건 총 **약 2,984분**) · **최종 검증 데이터 398건** 팀 구축
- **5,152개 오류 의심 구간 / 37건 전체 재검토 대상**을 선별하는 High-Recall QC 로직과 Human Review 흐름
- Whisper word timestamp와 NeMo 화자 구간의 시간 겹침 정렬 및 검수 계획·Streamlit UI
- 공개 프로젝트에는 실제 음성 대신 합성 샘플, 실행 코드, 테스트와 GitHub Actions를 포함

### 🧴 Cosmetic Cold-Start Risk ML
[Repository](https://github.com/Westzer00/cosmetic-coldstart-risk-ml)

- 리뷰가 없는 신제품 화장품의 **피부유형별 부정 경험 위험**을 출시 전 정보만으로 선별하는 문제 정의
- **47,487개 리뷰**는 Label 생성에만 사용하고, Prediction Input에서는 제외해 cold-start 조건을 유지
- 성분·기능군·피부유형 상호작용 중심의 Feature Engineering과 formula-group 기반 leakage-aware validation 수행
- Independent Test: **Recall 63.1%, PR-AUC 0.384**, High Risk 65건 중 41건 탐지
- 4인 팀 **팀장·제1저자**, 2026 한국데이터마이닝학회 하계학술대회 Poster P1-62

### 🎬 UniVTG Creator Segment Retrieval
[Repository](https://github.com/Westzer00/univtg-creator-segment-retrieval)

- 영상별 transcript와 title에서 LLM query를 생성하고 **UniVTG Top-50 candidate → Top-10 ranking**으로 이어지는 retrieval pipeline 구현
- YouTube Most Replayed는 retrieval 입력이 아닌 **독립적인 viewer-interest evaluation proxy**로 사용
- 대표 결과: **nDCG@10 0.3398 / Any-Hit@10(tIoU 0.3) 68.89% / Top-50 Oracle nDCG@10 0.6319**
- Candidate Generation보다 **Ranking이 주요 bottleneck**임을 실험 결과로 분리해 분석

### 🚀 Rocket Avionics Case Study
[Repository](https://github.com/Westzer00/rocket-avionics-case-study)

- GOAT 2024 전자부에서 **BMP280 · GPS · 9DOF IMU** 기반 비행 데이터 수집·처리 및 실제 발사체 통합 테스트 참여
- Raspberry Pi에서 **I2C / UART**로 센서를 연결하고, altitude baseline 및 moving average 기반 하강 판단 로직 구현에 참여
- 하강 조건 판단 결과를 **GPIO / PWM → Relay / Servo → parachute deployment**로 연결
- 개인 Case Study에는 팀 전체 코드를 복사하지 않고, 실제 기여 범위와 시스템 구조를 중심으로 정리


## Engineering Focus

- **AI Application / Backend** — RAG·LLM 워크플로우, API 연동, 반복 실행 상태 및 데이터 전달
- **Data Quality / Evaluation** — STT QC, Human Review, 검증 데이터 구축, ML validation
- **Business Data Integration** — 제조업 업무 데이터 모델링, MES 연동, 문서 자동화
- **Multimodal / Embedded** — Video-Language Retrieval, 센서 입력·상태 판단·제어

## Tech (Project Experience)

**Programming & Web**  
Python · TypeScript · JavaScript · FastAPI · React · Next.js · SQL

**AI & Data**  
Pandas · scikit-learn · Whisper · NeMo · Milvus · RAG · LLM · OpenAI API · UniVTG

**Systems & Workflow**  
Cloudflare Workers · Docker · Git / GitHub · pytest · Streamlit · Raspberry Pi · I2C / UART · GPIO / PWM

## Contact

- Email: **k953609@gmail.com**
- GitHub: **[@Westzer00](https://github.com/Westzer00)**

---

공개 저장소에는 확인 가능한 개인 기여, 실행 예제와 기술적 판단을 정리했습니다. 팀 프로젝트 성과는 개인 작업과 구분하며 비공개 데이터·기업 소스·credential은 공개하지 않습니다.
