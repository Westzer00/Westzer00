# Seoyeong Kim | AI 서비스 개발

가천대학교 컴퓨터공학 전공 · **AI 서비스 / AI Agent / 백엔드 개발**

**사용자에게 필요한 기능을 만들고, 데이터와 AI의 결과가 실제 업무에서 맞게 작동하는지 확인하는 개발**을 해왔습니다.

- **기업 업무를 서비스로 구현:** 제조업의 MES·구매·수출·회계 데이터를 연결하는 API, AI 조회, 문서 자동화 개발·운영
- **AI 결과의 오류를 검증:** 약 49.7시간의 음성 검수 체계와 사람 검토 도구 개발, 검증 데이터 구축에 참여
- **기존 시스템의 한계를 개선:** EXEM AI 플랫폼의 LOOP 데이터 전달 문제를 발견하고 Python 백엔드 로직 및 테스트 개발

## 주요 프로젝트

### 1. BLI | 제조업 데이터 통합·AI 업무 플랫폼

**2026.09~현재 · 2인 개발 · 실제 기업 업무에 적용**

부서별로 흩어진 발주·입고·생산·수출·회계 기록을 연결하고, 경영진과 실무자가 함께 사용하는 AI 업무 플랫폼을 개발했습니다.

- **업무 데이터 설계:** 품목·거래처·발주 등을 관계로 정리하고 기존 MES·회계·수출 자료와 연동
- **AI·백엔드 구현:** TypeScript, Next.js, Cloudflare Workers, OpenAI API 기반 화면·API 및 근거 있는 데이터 조회
- **업무 적용:** 문서 추출·대조, 견적·실제 매출·미확정 자료 구분, 분할 입고와 중복 처리 방지, 배포·운영

> 고객사의 원천 데이터와 내부 소스는 공개하지 않습니다. 실제 화면은 비식별화한 별도 발표 자료로 정리합니다.

### 2. [EXEM / PHISIGHT | AI 워크플로우·LOOP 백엔드 개선](https://github.com/Westzer00/exem-ai-workflow)

**2026.07~2026.10 · 5인 팀 · 공공기관 협업 과제**

RAG 기반 검색 → 유형 분류 → 시나리오 생성 → 결과 검수로 이어지는 보이스피싱 분석 서비스를 팀과 함께 개발했습니다.

- **기존 플랫폼 개선:** 내부 노드의 여러 출력을 다음 회차로 전달하기 어려운 문제를 발견하고 LOOP 입출력 바인딩·이전 회차 참조·종료 조건을 Python으로 개발하고 테스트
- **사내 개발 과정:** 기능 기획과 하위 작업 분해, PR·코드 리뷰 피드백 반영까지 수행(회사 Git 기록은 비공개)
- **기술 검증:** 정상 동작뿐 아니라 값 누락·잘못된 참조·반복 종료 등 오류 조건을 점검

- **서비스 UI:** 입력부터 검수까지 화면 흐름을 설계하고 상세 UI를 팀원 1명과 공동 구현
- [독립 LOOP 코드·테스트·개발 과정·PHISIGHT UI 설명](https://github.com/Westzer00/exem-ai-workflow)

협업기관명과 원본 데이터는 공개하지 않으며 공공기관 현장 도입·운영 실적을 주장하지 않습니다.

### 3. [STT 검수 파이프라인](https://github.com/Westzer00/voice-phishing-stt-qc-pipeline)

**Python · Whisper · NeMo · Streamlit**

- 통화 **511건** 분석, 읽기 가능한 **509건 약 2,984분**, 최종 검증 데이터 **398건** 구축에 참여
- 금융·수사 관련 핵심 단어의 오류를 찾기 위해 **5,152개 의심 구간**과 **37건 재검토 통화** 선별
- 원음 대조와 수정이 가능한 사람 검토 UI, 화자 정렬 및 검수 계획 구현
- [핵심 코드·실행 방법·테스트](https://github.com/Westzer00/voice-phishing-stt-qc-pipeline#실행-및-테스트)

### 4. [리뷰 없는 신제품 위험 선별 머신러닝](https://github.com/Westzer00/cosmetic-coldstart-risk-ml)

**4인 팀장 · 2026 한국데이터마이닝학회 제1저자 포스터 발표**

- 리뷰가 없는 신제품에서 사용할 수 있는 성분·제품명·피부유형으로 입력 변수 구성
- 유사 처방 제품군이 학습·평가에 섞이는 데이터 누수 방지
- 독립 평가에서 **Recall 63.1%, PR-AUC 0.384**, 고위험 조합 **65개 중 41개** 탐지
- [전처리 코드·검증 방법·연구 결과](https://github.com/Westzer00/cosmetic-coldstart-risk-ml)

### 5. [영상 관심 구간 추천 및 성능 분석](https://github.com/Westzer00/univtg-creator-segment-retrieval)

- UniVTG와 영상별 LLM 질의로 후보 구간을 생성하고 YouTube 반복 재생 구간으로 평가
- Top-50 후보에는 유효 구간이 있으나 Top-10 정렬 과정에서 성능이 낮아지는 **병목 확인**
- [코드·평가 지표·한계](https://github.com/Westzer00/univtg-creator-segment-retrieval)

### 6. [로켓 비행전자·낙하산 전개 제어](https://github.com/Westzer00/rocket-avionics-case-study)

- 실제 로켓에 센서·제어 장치를 통합하고 발사 시험에 참여한 팀 프로젝트
- Raspberry Pi에서 센서값을 처리하고 고도 기반 하강 판단 → 제어 출력 흐름에 참여
- [구조·독립 실행 예제·테스트·실제 제작 사진](https://github.com/Westzer00/rocket-avionics-case-study)

## 사용할 수 있는 기술

| 분야 | 직접 적용한 기술과 작업 |
|---|---|
| **언어·서비스** | Python, TypeScript, JavaScript, FastAPI, Next.js, REST API |
| **AI·데이터** | Whisper, NeMo, Pandas, scikit-learn, Milvus, RAG, LLM, OpenAI API |
| **배포·검증** | Cloudflare Workers, Docker, Git/GitHub, pytest, Streamlit |
| **하드웨어** | Raspberry Pi, I2C, UART, GPIO/PWM |

기술 목록보다 **어디에 적용했고 어떻게 확인했는지**를 각 저장소의 README와 코드·테스트에서 확인할 수 있도록 구성했습니다.

## 연락

- **이메일:** k953609@gmail.com
- **GitHub:** [@Westzer00](https://github.com/Westzer00)

---

**기여 범위:** 기업·팀 프로젝트의 결과는 개인 담당 영역과 구분했습니다. 비공개 제품 소스, 실제 음성·고객 데이터와 인증 정보는 공개하지 않습니다.
