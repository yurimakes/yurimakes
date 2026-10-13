# Yuri | Data Engineering

**Python · SQL · Azure · Databricks**

**Focus:** 데이터 파이프라인 · 데이터 정합성 · 재현 가능한 검증 · ML/API 연계  
**Background:** Majoring in Artificial Intelligence

---

## 🚀 Engineering Projects

| Project | Key Contributions & Tech Stack |
| --- | --- |
| **[CANOPY Data Platform](https://github.com/yurimakes/canopy-data-platform)**<br>GPS 기반 친환경 이동 서비스 | • **데이터 수집:** GPS 이벤트 스키마·Azure Functions 수집 기능 구현, Event Hubs → ADLS 원본 저장 검증<br>• **데이터 처리:** Databricks 기반 개인별 이동 기준·미션·보상·랭킹 연결, 보상 이력 중복 방지(멱등 처리) 구현<br>**Stack:** `Azure Functions` · `Event Hubs` · `ADLS` · `Databricks` · `PySpark` · `MLflow` |
| **잠실 교통 혼잡 예측**<br>대중교통 혼잡 예측·운영 지원<br>**팀장 · PM** | • **수집·전처리:** 버스·지하철·행사·기상 데이터 정규화, CSV/XLSX 재실행 경로 개발<br>• **데이터·ML 검증:** 실시간 5·10·30분 관측과 과거 1시간 단위 학습 데이터의 **시간 해상도 불일치**·호선 범위 차이 분석, 입력 정합성·시간순 평가 개선 중<br>**Stack:** `Python` · `Azure` · `PostgreSQL` · `scikit-learn` |
| **금융상품 AI Agent**<br>미래에셋증권 제10회 AI페스티벌<br>**팀장** | • **온톨로지:** RDF/Turtle·Semantic Registry 설계·구현, 금융상품 필드의 의미·단위·허용 연산 구조화<br>• **근거 기반 조회:** 허용된 필드·연산 검증 후 PostgreSQL 조회 및 AI 설명 연계<br>**Stack:** `Python` · `PostgreSQL` · `SQL` · `RDF/Turtle` · `Ontology Modeling` |
| **[지원장바구니](https://github.com/yurimakes/youth-policy-llm-recommender)**<br>청년정책 AI 에이전트 | • **서비스 기획:** 상황 카드 → 필요한 질문 → 정책 후보·조건 확인 → 신청 준비·상담 흐름 설계<br>• **데이터 파이프라인(v0):** 청년정책 API 수집·원본 보존·정규화·SQLite 중복 방지 적재, 연령·지역·취업·기간 규칙 판정<br>• **검색·설명 AI(v0):** OpenAI 임베딩·FAISS 검색, 공식 정책정보·판정 근거 기반 LLM 설명, AI 실패 시 규칙 결과 유지<br>• **API 고도화:** FastAPI 상태 전환·답변 수정, 관심사 정렬·조건별 질문 순서·신청 준비 정보, GitHub Actions 회귀검증<br>**Stack:** `Python` · `SQLite` · `FastAPI` · `Streamlit` · `FAISS` · `OpenAI API` · `GitHub Actions`<br>[공개 데모](https://jiwon-basket.vercel.app/) — 실제 정책 API·LLM과 분리된 가상 정책 체험 |
| **[FinBridge](https://github.com/start-finance-ai/finbridge-backend)**<br>창업·금융지원 의사결정 서비스<br> | • **데이터·계산 API:** 지원사업 정규화·검색·조건 매칭, 재무·소득·매출 계산<br>• **신뢰성:** 규칙 기반 판정·계산과 LLM 설명 분리, AI 장애 시 검증된 결과를 유지하는 폴백 구현<br>**Stack:** `Python` · `FastAPI` · `Pydantic` · `OpenAI API`<br>[Frontend](https://github.com/start-finance-ai/finbridge-frontend) |
| **CertiMakers**<br>소공인 KC 인증 준비도 진단·컨설팅 AI 서비스<br>**6인 팀 · 팀장 · PM** | • **기획·리딩:** 서비스 방향·요구사항 정의, 일정·산출물 관리, 기능 구현 검수<br>• **AI 품질 평가:** Python 평가 코드 기반 공식 근거 검색(RAG) 방식 비교, 문서 버전·규칙/근거 정합성·AI 위험 문장 차단 검증<br>**Stack:** `Python` · `RAG` · `Rule Engine` · `AI Evaluation` |

## 📊 Machine Learning & Data Analysis

| Project | Key Contributions & Tech Stack |
| --- | --- |
| **[Wind Power Forecasting](https://github.com/yurimakes/wind-forecasting-ai)**<br>풍력 발전량 예측 | • LDAPS·GFS 기상 예보 특징 생성, 시점 분리 검증 및 회귀 모델·앙상블 비교<br>• 입력·예측값·결과 파일 검증, 실험·재현 절차 문서화<br>**Stack:** `Python` · `LightGBM` · `XGBoost` · `CatBoost` |
| **CUB-200-2011 Bird Classification**<br>200종 조류 이미지 분류 | • PyTorch 학습·추론 구현, ResNet50·EfficientNet-B3·ConvNeXt 비교<br>• 이미지 증강·파인튜닝 실험, 최종 ConvNeXt-Base(384×384) 선정 — **리더보드 Macro-F1 0.9098**(저장소 기록)<br>**Stack:** `Python` · `PyTorch` · `torchvision` · `timm` · `ConvNeXt` |
| **[Bank Marketing Classification](https://github.com/yurimakes/26-1-data-science-term-project)**<br>은행 마케팅 분류 | • Logistic Regression·Random Forest 비교, 불균형 타깃의 F1·Recall·ROC-AUC 평가<br>• 양성 클래스 탐지 한계 분석·결과 해석<br>**Stack:** `Python` · `scikit-learn` |

---

## 🛠️ Tech Stack

| Area | Tools |
| --- | --- |
| **Data Engineering & Cloud** | Python · SQL · PostgreSQL · Azure Functions · Event Hubs · ADLS · Databricks · Apache Spark / PySpark |
| **Applied AI & Backend** | FastAPI · SQLite · Pydantic · FAISS · RAG · OpenAI API · RDF/Turtle · Ontology Modeling |
| **Machine Learning** | scikit-learn · LightGBM · XGBoost · CatBoost · MLflow |
| **Development & Testing** | Git · GitHub · GitHub Actions |
| **Coursework & Experiments** | PyTorch |
