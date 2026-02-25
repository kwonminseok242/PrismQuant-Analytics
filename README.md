# 🧠 PrismQuant-analytics

> **AI-Driven Market Analysis & Backtesting Engine**
> 뉴스 데이터 수집, LLM 기반 인사이트 생성, 그리고 정교한 백테스팅을 담당하는 분석 엔진입니다.

---

## 🚀 Key Features

### 🤖 AI Insight Generation
- **LLM Summary:** GPT-4/Claude를 활용하여 코인니스, 뉴스 데이터를 요약 및 매매 적합성 판단.
- **Sentiment Analysis:** 시장 뉴스 및 지표에 대한 긍정/부정 점수 산출.

### 📊 Advanced Backtesting
- **Strategy Simulation:** 과거 데이터를 활용한 파인스크립트 기반 전략 수익률 시뮬레이션.
- **Performance Metrics:** Sharpe Ratio, MDD(최대 낙폭), 승률 등 핵심 지표 계산.

### 🌐 Data Crawling
- **Multi-source Scraper:** 코인니스, Investing.com, CoinGecko 등 다채널 경제 지표 수집.
- **Time-series Storage:** 수집된 데이터를 시계열 형태로 가공하여 분석용 DB 저장.

### 🚨 Anomaly Detection
- **Pattern Recognition:** 급격한 연속 거래 등 뇌동매매 패턴 감지 및 경고 알림 생성.

---

## 🛠 Tech Stack

- **Language:** Python 3.10+
- **AI Framework:** LangChain, OpenAI API
- **Data Science:** Pandas, NumPy
- **Scraping:** Selenium, BeautifulSoup4
- **Task Scheduler:** Celery + Redis

---

## 📂 Directory Structure

```text
.
├── crawlers/         # 뉴스 및 지표 수집 스크립트
├── engine/           # 백테스팅 엔진 로직
├── ai/               # LLM 프롬프트 및 분석 모듈
├── notebooks/        # 데이터 분석용 Jupyter Notebooks
├── tasks.py          # 비동기 작업 정의 (Celery)
└── main.py           # 분석 서버 진입점