# Yuri | Data Engineering

**Python · SQL · Azure · Databricks**

데이터를 수집·정규화하고, 분석·ML·API에 연결하는 프로젝트를 개발했습니다.  
**Focus:** 데이터 정합성 · 재현 가능한 검증 · 데이터 파이프라인

**Background:** Majoring in Artificial Intelligence

---

## 🚀 Engineering Projects

### [CANOPY Data Platform](https://github.com/yurimakes/canopy-data-platform) — GPS 기반 친환경 이동 서비스

- **GPS 수집·원본 보존:** 이벤트 스키마와 Azure Functions 수집 기능을 구현하고, Event Hubs → ADLS 원본 저장 흐름을 검증했습니다.
- **분석 데이터 연결:** Databricks에서 개인별 이동 기준 산정, 친환경 미션·보상·랭킹을 연결하고, 보상 이력 중복 기록을 방지하는 멱등 처리 로직을 구현했습니다.

`Azure Functions` `Event Hubs` `ADLS` `Databricks` `PySpark` `MLflow`

### 잠실 교통 혼잡 예측 — 대중교통 혼잡 예측·운영 지원 (팀장·PM)

- **수집·전처리:** 버스·지하철·행사·기상 데이터의 정규화와 CSV/XLSX 기반 재실행 경로를 개발했습니다.
- **데이터 정합성·ML 검증:** **실시간 5·10·30분 관측과 과거 1시간 단위 학습 데이터의 시간 해상도 불일치** 및 지하철 호선 범위 차이를 분석하고, 입력 기준 정리와 시간순 모델 평가를 개선하고 있습니다.

`Python` `Azure` `PostgreSQL` `scikit-learn`

### 금융상품 AI Agent — 미래에셋증권 제10회 AI페스티벌 (팀장)

- **온톨로지 설계:** RDF/Turtle 온톨로지와 Semantic Registry를 구현해 금융상품의 의미·단위·허용 연산을 구조화했습니다.
- **조회 검증:** 허용된 필드·연산을 검사한 뒤 PostgreSQL 구조화 조회와 근거 기반 AI 응답을 연결했습니다.

`Python` `PostgreSQL` `SQL` `RDF/Turtle` `Ontology Modeling`

### [지원장바구니](https://github.com/yurimakes/youth-policy-llm-recommender) — 청년정책 AI 에이전트 (기획·AI·백엔드 / 개발 중)

- **정책 데이터 파이프라인 (v0):** 청년정책 API 데이터를 수집해 원본 응답·메타데이터를 보존하고, 공통 정책 모델로 정규화해 SQLite에 중복 없이 적재했습니다. 연령·지역·취업 상태·신청 기간을 규칙으로 평가해 **조건 일치·명확한 불일치·추가 확인 필요**를 구분했습니다.
- **검색·설명 AI (v0):** 규칙 평가를 통과하거나 추가 확인이 필요한 후보에 **OpenAI 임베딩·FAISS 검색**을 적용하고, 검색된 정책의 공식 필드와 판정 근거를 LLM에 전달해 추천 이유를 설명하도록 구현했습니다. AI 호출 실패 시에도 규칙 평가 결과를 유지합니다.
- **서비스·API 고도화:** FastAPI 기반 상태 전환 API에서 답변 수정·건너뛰기, 관심사 기반 후보 정렬, **남은 후보의 조건에 따른 질문 순서 선택**과 정책별 신청 기간·준비서류 안내를 구현했습니다. 회귀 테스트·GitHub Actions를 구성했으며, [공개 데모](https://jiwon-basket.vercel.app/)는 **실제 정책 API·LLM과 분리된 가상 정책 체험**입니다.

`Python` `SQLite` `FastAPI` `Streamlit` `FAISS` `OpenAI API` `GitHub Actions`

### [FinBridge](https://github.com/start-finance-ai/finbridge-backend) — 창업·금융지원 의사결정 서비스 (팀장·PM)

- **데이터·계산 API:** 지원사업 데이터 정규화·검색·조건 매칭과 재무·소득·매출 계산 API를 개발했습니다.
- **신뢰성:** 규칙 기반 판정·계산과 LLM 설명을 분리하고, AI 호출이 실패해도 확인된 결과를 제공하도록 폴백을 구현했습니다. [Frontend](https://github.com/start-finance-ai/finbridge-frontend)

`Python` `FastAPI` `Pydantic` `OpenAI API`

### CertiMakers — 소공인 KC 인증 준비도 진단·컨설팅 AI 서비스 (팀장·PM)

- **팀 리딩·기획:** 6인 팀의 서비스 방향·요구사항을 정리하고, 일정·산출물 관리와 기능 구현 검수를 총괄했습니다.
- **AI 품질 검증:** 별도 Python 평가 코드로 KC 공식 근거 검색(RAG) 방식, 문서 버전 적합성, 규칙·근거 간 정합성 및 AI 위험 문장 차단을 비교·검증했습니다.

`Python` `RAG` `Rule Engine` `AI Evaluation`

## 📊 Machine Learning & Data Analysis

### [Wind Power Forecasting](https://github.com/yurimakes/wind-forecasting-ai) — 풍력 발전량 예측

- LDAPS·GFS 기상 예보 특징을 생성하고, 학습·검증 시점을 분리해 회귀 모델과 앙상블을 비교했습니다.
- 입력·예측값 범위와 결과 파일을 검사하고 실험·재현 방법을 문서화했습니다.

`Python` `LightGBM` `XGBoost` `CatBoost`

### CUB-200-2011 Bird Classification — 200종 조류 이미지 분류

- **모델 학습·비교:** PyTorch로 학습·추론 코드를 구현하고, ResNet50·EfficientNet-B3·ConvNeXt 계열의 이미지 분류 모델을 비교했습니다.
- **파인튜닝·평가:** 이미지 증강과 학습 설정을 실험해 ConvNeXt-Base(384×384)를 최종 선택했습니다. 저장소에 기록된 최종 **리더보드 Macro-F1은 0.9098**입니다.

`Python` `PyTorch` `torchvision` `timm` `ConvNeXt`

### [Bank Marketing Classification](https://github.com/yurimakes/26-1-data-science-term-project) — 은행 마케팅 분류

- Logistic Regression·Random Forest를 비교하고, 불균형 데이터에서 F1·Recall·ROC-AUC를 평가했습니다.
- 양성 클래스 탐지의 한계를 분석하고 모델 결과를 해석했습니다.

`Python` `scikit-learn`

---

## 🛠️ Tech Stack

| Area | Tools |
| --- | --- |
| **Data Engineering & Cloud** | Python · SQL · PostgreSQL · Azure Functions · Event Hubs · ADLS · Databricks · Apache Spark / PySpark |
| **Applied AI & Backend** | FastAPI · SQLite · Pydantic · FAISS · RAG · OpenAI API · RDF/Turtle · Ontology Modeling |
| **Machine Learning** | scikit-learn · LightGBM · XGBoost · CatBoost · MLflow |
| **Development & Testing** | Git · GitHub · GitHub Actions |
| **Coursework & Experiments** | PyTorch |
