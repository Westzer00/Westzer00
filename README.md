
# 김서영 포트폴리오
### AI Agent Engineer · AI 서비스 개발자

## 🎯 대표 프로젝트

<table>
  <tr>
    <td width="21%" align="center" valign="middle">
      <h2>🔁</h2>
      <strong>AI 백엔드 개발</strong><br/>
      <sub>LOOP 입·출력 구조 개선</sub>
    </td>
    <td width="79%" valign="top">
      <strong><a href="https://github.com/Westzer00/exem-ai-workflow">EXEM · AI 워크플로우 및 PHISIGHT</a></strong><br/>
      <sub>2026.07~10 · 5인 기업연계 프로젝트 · 공공기관 협업 과제</sub>
      <p>🔎 <strong>문제</strong> — LOOP 내부 여러 노드의 실행 결과를 다음 회차에 개별 전달하기 어려운 기존 구조</p>
      <p>👩‍💻 <strong>개인 구현</strong> — LOOP 입출력 바인딩, 이전 회차 결과 전달, 종료 조건 처리 등 Python 백엔드 로직 개발·테스트 및 사내 PR·코드 리뷰 반영</p>
      <p>🤝 <strong>협업</strong> — PHISIGHT 화면 구조·사용자 흐름 설계 및 상세 UI 공동 개발</p>
      <p>🎯 <strong>팀 성과</strong> — 공공기관 피싱 공동대응 지원을 위한 보이스피싱·스미싱 사례 분석, 유사사례 검색, 신규 시나리오 생성·검증 워크플로우와 운영 UI 구축</p>
      <p><a href="https://github.com/Westzer00/exem-ai-workflow/tree/main/backend">코드·테스트</a> · <a href="https://github.com/Westzer00/exem-ai-workflow/blob/main/docs/development-review.md">개발 과정</a> · <a href="https://github.com/Westzer00/exem-ai-workflow/blob/main/docs/ui-participation.md">UI 화면</a></p>
    </td>
  </tr>
  <tr>
    <td align="center" valign="middle">
      <h2>🏭</h2>
      <strong>제조업 AI</strong><br/>
      <sub>현업 데이터 통합</sub>
    </td>
    <td valign="top">
      <strong>BLI · 제조업 데이터 통합 및 AI 업무 플랫폼</strong><br/>
      <sub>2026.09~현재 · 2인 개발 · 실제 기업 업무 적용</sub>
      <p>🔎 <strong>문제</strong> — 발주·입고·생산·수출·회계 데이터의 부서별 분산 관리와 정보 불일치</p>
      <p>👩‍💻 <strong>개인 구현</strong> — 품목·거래처·발주 데이터 모델 설계, 기존 MES 연동, TypeScript 기반 API·AI 조회·문서 자동화 및 중복 처리 방지 기능 개발·운영</p>
      <p><sub>기업 내부 코드 및 거래처 자료 비공개</sub></p>
    </td>
  </tr>
  <tr>
    <td align="center" valign="middle">
      <h2>🎧</h2>
      <strong>STT 품질 검수</strong><br/>
      <sub>오류 선별·사람 검토</sub>
    </td>
    <td valign="top">
      <strong><a href="https://github.com/Westzer00/voice-phishing-stt-qc-pipeline">보이스피싱 음성인식 검수 파이프라인</a></strong><br/>
      <sub>EXEM 기업연계 프로젝트 · 개인 개발 코드 공개</sub>
      <p>🔎 <strong>문제</strong> — 음성인식 결과에서 기관명·금액 등 핵심 정보의 오인식 발생</p>
      <p>👩‍💻 <strong>개인 구현</strong> — 오류 의심 구간 선별 로직, 화자 정렬 및 원음 비교·수정용 검수 UI 개발</p>
      <p>📊 <strong>개인 수행</strong> — 통화 511건 STT 처리·검수, 오류 의심 구간 5,152개 선별, 최종 검증 데이터셋 398건 구축</p>
      <p><a href="https://github.com/Westzer00/voice-phishing-stt-qc-pipeline">코드·실행 방법</a> · <a href="https://github.com/Westzer00/voice-phishing-stt-qc-pipeline/actions">자동 테스트</a></p>
    </td>
  </tr>
</table>

## 📂 다른 프로젝트

| 프로젝트 | 구현과 검증 내용 |
|:---|:---|
| 🧴 **[화장품 신제품 위험 선별 ML](https://github.com/Westzer00/cosmetic-coldstart-risk-ml)** | 출시 전 입력 변수 설계와 데이터 누수 방지 검증. **4인 팀장·제1저자 학술발표** |
| 🎬 **[영상 관심 구간 검색·평가](https://github.com/Westzer00/univtg-creator-segment-retrieval)** | UniVTG 기반 검색, LLM 질의 설계, 상위 후보 정렬 단계의 성능 병목 분석 |
| 🚀 **[로켓 비행전자 시스템](https://github.com/Westzer00/rocket-avionics-case-study)** | 센서 처리·하강 판단·낙하산 제어 개발 참여, 실제 제작·발사 시험 및 코드·사진 |

## 🛠️ 사용 기술

**서비스·백엔드** &nbsp; `Python` · `TypeScript` · `FastAPI` · `Next.js` · `REST API`

**AI·데이터** &nbsp; `RAG` · `LLM API` · `Whisper` · `NeMo` · `Milvus` · `Pandas`

**개발·검증** &nbsp; `Git` · `Docker` · `pytest` · `GitHub Actions` · `Cloudflare Workers`

## 💡 개발 강점

<table>
  <tr>
    <td width="33%" align="center" valign="top">
      🧩 <strong>기존 시스템 분석·개선</strong><br/>
      <sub>EXEM LOOP 백엔드 로직 수정과<br/>예외 조건 테스트</sub>
    </td>
    <td width="34%" align="center" valign="top">
      🏭 <strong>현업 중심 서비스 개발</strong><br/>
      <sub>업무 흐름 분석부터 데이터 설계,<br/>API 개발·운영까지 수행</sub>
    </td>
    <td width="33%" align="center" valign="top">
      🛡️ <strong>AI 결과 검증·품질 관리</strong><br/>
      <sub>음성인식 오류 선별, 사람 검수 UI,<br/>검증 데이터셋 구축</sub>
    </td>
  </tr>
</table>
