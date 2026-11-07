# 김서영 | AI 서비스 개발

Python과 TypeScript로 데이터를 다루고, AI 워크플로우가 실제 화면·API에서 어떻게 실행되는지 구현하고 검증하는 일을 해왔습니다.

기업 프로젝트에서는 **기존 코드의 제약을 분석해 수정하는 일**, 음성인식 결과의 **사람 검수 절차**, 제조업의 **업무 데이터 연결**을 경험했습니다. 팀 전체 성과와 개인 작업은 각 저장소에 나눠 적었습니다.

## 주요 작업

### 1. EXEM · eXemble LOOP 백엔드

[LOOP 개선 코드·기술 기록](https://github.com/Westzer00/exem-ai-workflow) · 2026.07–10 / 5인 기업연계 프로젝트

기존 LOOP가 내부 노드의 여러 결과를 다음 실행으로 구분해 넘기기 어려워 입출력 바인딩과 직전 회차 결과 참조, 종료 조건 처리를 수정했습니다.

- **직접 담당:** 사내 Python 실행 로직 변경, 관련 테스트와 PR·코드 리뷰. PHISIGHT 화면의 사용자 흐름 설계 및 상세 UI는 팀원과 공동 작업
- **GitHub 공개 범위:** 회사 원본 대신 동일한 핵심 동작을 다시 구현한 [독립 LOOP 엔진](https://github.com/Westzer00/exem-ai-workflow/tree/main/backend/loop_demo)·API·합성 데이터 예제
- **남은 검증:** 사내 제품의 신규 설정 UI 연동·운영 배포와 실제 분석 엔진 연결은 완료된 것으로 표기하지 않음

### 2. BLI · 제조업 AI 업무 플랫폼

2026.09–진행 중 / 2인 개발

발주·입고·생산·수출·회계 자료의 연결 관계를 정의하고 MES 및 업무 문서를 활용하는 화면·API와 AI 조회·문서 처리를 개발했습니다.

- **참여 범위:** 품목·거래처·발주 데이터 모델, 조회 화면·API, 문서 처리와 중복 요청 방지 로직
- **자료 범위:** 기업 내부 소스와 거래처 자료는 공개하지 않습니다. 이 GitHub의 독립 코드 테스트로 BLI 운영 성능을 증명하지 않습니다.

### 3. 보이스피싱 STT 품질 검수

[STT 검수 로직·Streamlit 예제](https://github.com/Westzer00/voice-phishing-stt-qc-pipeline) · EXEM 기업연계

Whisper 전사에서 금액·기관명, 반복 표현, 낮은 confidence 등을 단서로 **사람이 확인할 구간**을 먼저 찾고, NeMo 화자 정렬과 검수 기록을 연결했습니다.

- 전체 통화 **511건**, 읽기 가능한 **509건** 약 **2,984분** 대상으로 STT 처리·검수
- 의심 후보 **5,152개 구간** 선별 및 검수 절차 담당
- 최종 **398건 Gold 데이터셋은 팀 확정 결과**입니다.
- 공개 UI는 합성 텍스트 기반 기록 데모이며 원음 재생과 실제 음성 데이터는 포함하지 않습니다.

## 그 밖의 프로젝트

| 프로젝트 | 맡은 작업 및 확인 가능한 결과 |
|---|---|
| [화장품 신제품 Cold-Start ML](https://github.com/Westzer00/cosmetic-coldstart-risk-ml) | 성분 전처리·변수 설계, 모델 비교 참여. 4인 팀장·2026 한국데이터마이닝학회 제1저자 포스터 |
| [UniVTG 영상 구간 검색](https://github.com/Westzer00/univtg-creator-segment-retrieval) | LLM Query, Top-50 후보·Top-10 정렬 평가, 병목 분석. 원본 영상 추론은 외부 패키지 필요 |
| [로켓 비행전자](https://github.com/Westzer00/rocket-avionics-case-study) | 센서 연동·하강 판단 조건 검토·비행전자 통합 시험. 2024 GOAT 팀 공동 작업; 공개 코드는 독립 재구성 예제 |

## 사용 기술

- **백엔드·웹:** Python, TypeScript, FastAPI, React, Next.js, REST API
- **AI·데이터:** RAG, Milvus, Whisper, NeMo, LLM API, Pandas, scikit-learn
- **개발·검증:** Git, pytest, Docker, GitHub Actions, SQL, Cloudflare Workers

각 저장소의 README에는 **어떤 부분을 직접 구현했는지**, **팀 성과가 무엇인지**, **공개 코드만으로 검증되지 않는 항목이 무엇인지** 구분해 두었습니다.
