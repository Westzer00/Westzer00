# Seoyeong Kim

Computer Engineering @ Gachon University  
**Applied AI · Robotics SW · Physical AI**

실물 **센서·제어 시스템**을 경험한 뒤 데이터·ML, Multimodal, LLM으로 확장해 왔습니다.  
모델 하나의 성능보다 **데이터 품질 → 입력/처리 → 판단 → 평가 → Human Review**까지 이어지는 전체 시스템을 어떻게 설계할지에 관심이 있습니다.

## Selected Engineering Work

### 🛡 Voice Phishing STT QC & Human Review Pipeline
[Repository](https://github.com/Westzer00/voice-phishing-stt-qc-pipeline)

- **511개 보이스피싱 통화**의 STT 결과를 대상으로 high-recall QC 및 Human Review 흐름 설계
- **5,152 suspicious segments / 37 call-level review targets**를 선별해 자동 결과를 곧바로 Gold Data로 사용하지 않도록 구성
- Whisper word timestamp와 NeMo diarization을 연결한 speaker alignment, review planning 및 Streamlit 검수 도구 구현
- 현재 Gold Data를 기반으로 **RAG → Classification → Scenario Generation → LLM Judge → Human Review** 흐름을 설계·구현 중

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

- **AI Data Quality / Human-in-the-loop** — STT QC, review routing, Gold Data 구축
- **Data / ML** — preprocessing, Feature Engineering, leakage-aware validation
- **Multimodal Retrieval** — video-language retrieval, candidate generation, ranking, evaluation
- **Physical Systems** — sensor integration, state decision, actuator connection

## Tech

**AI / Data**  
Python · Pandas · NumPy · scikit-learn · Whisper · NeMo · Milvus · RAG/LLM · UniVTG

**Embedded / Systems**  
Raspberry Pi · I2C · UART · GPIO · PWM · MySQL

**Workflow**  
Git · GitHub · Streamlit

## Contact

- Email: **k953609@gmail.com**
- GitHub: **@Westzer00**

---

Public repositories are curated for recruiting use.  
팀 프로젝트는 개인 기여 범위를 구분하고, 비공개 데이터·내부 코드·credential은 공개하지 않습니다.
