<div align="center">

# 강지수 · Kang Ji Soo

통계학을 기반으로 데이터 분석과 AI 기술을 활용한 문제 해결에 관심이 있습니다.

데이터 분석부터 모델링, 서비스 구현 및 배포까지 경험하며 성장하고 있습니다.

[![Email](https://img.shields.io/badge/rkdwl3264@naver.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rkdwl3264@naver.com)
[![GitHub](https://img.shields.io/badge/rkdwltn1211-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211)

</div>

---

## Projects

### 🔐 기업 IT 보안 정책 Self-Correction RAG 에이전트

*개인 프로젝트 · LLM / RAG / AI Service*

공개 보안 PDF 문서를 기반으로 사용자 권한에 따른 문서 검색과 답변 검증을 수행하는 AI 질의응답 시스템

**주요 구현 및 성과**

- **PyMuPDF 및 조건부 OCR**을 활용한 PDF 데이터 처리, 메타데이터 관리 및 증분 갱신 구현
- **LangGraph 기반 Self-Correction RAG** 설계 — Hybrid Search, Query Rewriting, 관련성·근거성 평가 및 재시도
- **JWT 인증 및 DB 역할 기반 문서 검색 제어**, 질의 로그 관리와 관리자 대시보드 구현
- Chroma 스냅샷 스트리밍 복원을 통해 **최대 메모리 사용량 약 69% 감소** 기록 (Windows 로컬 모의 DB 환경)
- AWS EC2 기반 배포에서 **Cloudflare Pages·Render·Neon** 기반 분리 배포 환경으로 전환

**Tech Stack:** Python · LangChain · LangGraph · OpenAI API · ChromaDB · BM25 · FastAPI · React · PostgreSQL · Docker

**Links**

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/security-rag-chatbot)
[![Live Demo](https://img.shields.io/badge/Live-Demo-009688?style=flat-square)](https://security-rag-chatbot.pages.dev/)

---

### 🚗 CarGuard — 차량 손상 심각도 분석 시스템

*4인 팀 프로젝트 및 개인 고도화 · Computer Vision / Deep Learning*

차량 탁송 과정에서 발생하는 손상 관련 분쟁을 줄이기 위해 기획한 프로젝트로, 차량 이미지 기반 손상 심각도 분석 모델을 개발하고 웹 서비스로 구현

**주요 구현 및 성과**

- 4인 팀 프로젝트에서 차량 흠집 탐지 담당 — OpenCV 기반 변화 후보 시각화 및 전후·차이 이미지를 결합한 **9채널 ResNet18 회귀 모델** 구현
- **CLAHE, ECC 이미지 정렬 및 차이 마스크** 기반 후보 영역 추출과 학습 데이터 구성
- **EfficientNet-B0 기반 Lv.0~4 심각도 분류 모델**로 재설계하고 데이터 증강, 클래스 가중 손실 및 Early Stopping 적용
- **FastAPI 기반 이미지 업로드·추론 API**와 예측 확률 및 손상 경고 기준을 제공하는 웹 UI 구현
- AWS EC2 배포 이후 CPU 기반 PyTorch 실행 환경을 구성하고 **Render 무료 호스팅 환경**으로 재배포

**Tech Stack:** Python · OpenCV · PyTorch · ResNet18 · EfficientNet-B0 · FastAPI · HTML · CSS · JavaScript · AWS EC2 · Render

**Links**

[![Team Project](https://img.shields.io/badge/GitHub-Team%20Project-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/vehicle-delivery-ai-system)
[![Personal Project](https://img.shields.io/badge/GitHub-Personal%20Project-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/vehicle-damage-detection)
[![Live Demo](https://img.shields.io/badge/Live-Demo-009688?style=flat-square)](https://vehicle-damage-detection-sm5j.onrender.com)

---

### 🌐 Suspicious Web Traffic — 의심 웹 트래픽 분석 시스템

*Data Analysis / Machine Learning / Web Security*

Chrome DevTools에서 수집한 HTTP 응답 데이터를 기반으로 의심 패턴을 수치화하고, 머신러닝 모델을 활용한 분류 및 브라우저 경고 구조를 설계한 프로젝트

**주요 구현 및 성과**

- **Chrome DevTools API 기반 HTTP 응답 수집** 및 필터링·중복 제거를 통해 관찰 데이터 **4,046건 중 506건**의 분석 데이터 구성
- 본문 길이, 문자 구성 비율, Shannon Entropy, JavaScript 키워드 등 **14개 특징 추출 및 규칙 기반 Weak Labeling** 구현
- **Logistic Regression과 Random Forest** 모델 비교, 클래스 불균형 대응 및 변수 중요도 분석
- Random Forest의 규칙 기반 라벨 테스트 데이터 **102건** 기준 **Accuracy 98.04%, Precision 1.000, Recall 0.857, FP 0건** 기록
- **TensorFlow/Keras 모델 학습** 및 **TensorFlow.js 기반 브라우저 추론·경고 표시 구조** 설계

**Tech Stack:** Python · pandas · NumPy · scikit-learn · TensorFlow · Keras · TensorFlow.js · JavaScript · Chrome DevTools API

**Links**

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/Suspicious-Web-Traffic-Analysis-using-Chrome-DevTools)


---

### 🏭 AI4I Predictive Maintenance — 설비 고장 예측 대시보드

AI4I 2020 데이터 기반 설비 고장 사전 탐지 및 비용 절감 시뮬레이션 시스템

**주요 구현 및 성과**

- 도메인 지식 기반 파생변수 3개 직접 설계 (Temp_diff / Power / Torque_Wear) — 고장 조건 일치율 **100%** 확인
- LR → RF → XGBoost → LightGBM 순차 실험, Threshold 최적화로 Recall **0.85** / ROC-AUC **0.97** 달성
- SHAP 분석으로 피처별 예측 기여도 시각화 및 고장 유형별 실무 조치 기준 도출

**Tech Stack:** Python · LightGBM · SHAP · Plotly · Streamlit

**Links**

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/AI4I-Predictive-Maintenance)
[![Live Demo](https://img.shields.io/badge/Live-Demo-009688?style=flat-square&logo=streamlit&logoColor=white)](https://ai4i-predictive-maintenance-ddhrq3ekz7dvtdfwrlz4mc.streamlit.app/)

---

## Tech Stack

### Data Analysis & Visualization

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-475569?style=flat-square)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square)
![SPSS](https://img.shields.io/badge/SPSS-054ADA?style=flat-square)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-475569?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-475569?style=flat-square)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

### Machine Learning & Deep Learning

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-475569?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-475569?style=flat-square)
![SHAP](https://img.shields.io/badge/SHAP-475569?style=flat-square)

### LLM & RAG

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-4B8BBE?style=flat-square&logo=langgraph&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI%20API-1C3C3C?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square)
![BM25](https://img.shields.io/badge/BM25-475569?style=flat-square)

### Backend & Frontend

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-663399?style=flat-square&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)

### Deployment & Collaboration Tools

![AWS EC2](https://img.shields.io/badge/AWS%20EC2-232F3E?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Render](https://img.shields.io/badge/Render-181717?style=flat-square&logo=render&logoColor=white)
![Cloudflare Pages](https://img.shields.io/badge/Cloudflare%20Pages-F38020?style=flat-square&logo=cloudflarepages&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-475569?style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)
![Label Studio](https://img.shields.io/badge/Label%20Studio-475569?style=flat-square)

---

## Experience

**에이아이웍스 (AIWORKX) | AI 사업본부**

*2026.07 – 2026.10 | 인턴 · 일경험 프로그램*

**게임 음향 데이터 라벨링 프로젝트 · PL (Project Leader)**

- 담당 게임 2종의 라벨링 기준 수립 및 가이드라인 작성
- 음향 데이터 라벨링, 골든셋 구축 및 작업자 교육
- 약 **1,700개 Task**의 라벨링 결과 검수(QA)
- Excel 관리대장 구축 및 Notion 기반 수정·재검수 이력 관리
- 작업자 질의응답, 진행 현황 관리 및 PM과의 일정 조율

**해양 객체 탐지 데이터 라벨링 프로젝트 · 작업자**

- Black Olive를 활용한 Bounding Box 기반 이미지 데이터 라벨링

![Label Studio](https://img.shields.io/badge/Label%20Studio-475569?style=flat-square)
![Black Olive](https://img.shields.io/badge/Black%20Olive-475569?style=flat-square)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square)
![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)

---

**부트캠프 | 심화 데이터 분석 과정**

*2025.11 – 2026.01*

---

**한국리서치 | 인턴 연구원**

*2024.07 – 2024.08*

- SPSS 활용, 전국 **1,000명** 설문 데이터 분석 및 주간 리포트 단독 작성

![SPSS](https://img.shields.io/badge/SPSS-054ADA?style=flat-square)

---

---

## Education

**한신대학교** 응용통계학과 학사 졸업 (2020.03 – 2025.02)

## Certifications

- **ADsP** (데이터 분석 준전문가) · 2025.06
- **컴퓨터 활용능력 2급** · 2025.01

---

<div align="center">

**데이터 분석과 AI 기술을 활용한 문제 해결에 대해 이야기하고 싶다면 편하게 연락해 주세요.**

[![Email](https://img.shields.io/badge/rkdwl3264@naver.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rkdwl3264@naver.com)
[![GitHub](https://img.shields.io/badge/rkdwltn1211-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211)

</div>
