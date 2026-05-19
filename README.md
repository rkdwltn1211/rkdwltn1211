<div align="center">

# 강지수 · Kang Ji Soo

응용통계학을 전공하며 데이터의 원리를 배웠고,  
지금은 **LLM 기반 시스템 설계·구현·배포**에 집중하고 있습니다.  
단순히 모델을 가져다 쓰는 것을 넘어, **왜 이 기술을 골랐는지 설명할 수 있는 코드**를 지향합니다.

[![Gmail](https://img.shields.io/badge/rkdwl3264@naver.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rkdwl3264@naver.com)
[![GitHub](https://img.shields.io/badge/rkdwltn1211-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211)

</div>

---

## 🚀 Projects

### 🔐 기업 IT 보안 정책 Self-Correction RAG 에이전트
> ISMS-P 보안 문서를 기반으로 답변하되, AI가 스스로 환각 여부를 검증하는 RAG 시스템

- 일반 RAG의 한계인 **Hallucination 문제**를 해결하기 위해 이중 검증 루프 직접 설계
- **Hybrid Search** (벡터 + BM25) + **Query Rewriting**으로 검색 누락 최소화
- EMPLOYEE / SECURITY / ADMIN **3단계 권한별 문서 접근 제어** 구현 (JWT)
- ADMIN 전용 **로그 분석 대시보드** — PASS/FAIL 비율, 질문 유형 통계, 사용자별 집계
- AWS EC2 + Docker Compose로 **실서비스 배포 및 운영 중**
- **Stack**: FastAPI · LangGraph · ChromaDB · React · PostgreSQL · AWS EC2 · Docker

[![Demo](https://img.shields.io/badge/🌐_라이브_데모-3.26.94.252-1A3A5C?style=flat-square)](http://3.26.94.252/)
[![Repo](https://img.shields.io/badge/GitHub-security--rag-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211)

---

### 🚗 CarGuard — 차량 손상 탐지 시스템
> 탁송 전·후 차량 이미지를 AI로 분석해 흠집 심각도(0~4단계)를 자동 판정하는 웹 서비스

- **EfficientNet-B0** Transfer Learning으로 심각도 분류
- OpenCV 파이프라인 직접 구현: ECC 정렬 → Canny 엣지 → Morphology → ROI 패치 추출
- 소규모 데이터(126쌍) 한계를 데이터 증강으로 극복 — 634장 → **4,190장**
- 0~4단계 심각도 라벨링 기준 직접 설계
- 팀 프로젝트 이후 **FastAPI 서버 + AWS EC2 배포**로 독립 고도화
- **Stack**: PyTorch · OpenCV · FastAPI · AWS EC2

[![Team](https://img.shields.io/badge/팀_프로젝트-vehicle--delivery--ai--system-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/vehicle-delivery-ai-system)
[![Personal](https://img.shields.io/badge/개인_고도화-vehicle--damage--detection-009688?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/vehicle-damage-detection)
[![Demo](https://img.shields.io/badge/Live-Demo-009688?style=flat-square&logo=amazonaws&logoColor=white)](http://3.27.11.142:8000)
---

### 🔍 웹 트래픽 의심 행동 탐지 시스템
> 브라우저 DevTools로 수집한 행동 패턴(14개 feature)만으로 정상/의심 트래픽을 분류하는 ML 탐지 시스템

- JavaScript로 **14개 feature 추출 함수 직접 구현** (외부 라이브러리 미사용)
- Random Forest: Precision **1.000** · False Positive **0건** · Accuracy **98.0%**
- Chrome Extension과 연동한 **end-to-end 경고 흐름** 구현
- **Stack**: Python · scikit-learn · TensorFlow.js · Chrome DevTools API

[![Repo](https://img.shields.io/badge/GitHub-Suspicious--Web--Traffic--Analysis-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/Suspicious-Web-Traffic-Analysis-using-Chrome-DevTools)

---

### 🏭 설비 고장 예측 대시보드
> AI4I 2020 데이터 기반 설비 고장 사전 탐지 및 비용 절감 시뮬레이션 시스템

- 도메인 지식 기반 파생변수 3개 직접 설계 (Temp_diff / Power / Torque_Wear) — 고장 조건 일치율 **100%** 확인
- LR → RF → XGBoost → LightGBM 순차 실험, Threshold 최적화로 Recall **0.85** / ROC-AUC **0.97** 달성
- SHAP 분석으로 피처별 예측 기여도 시각화 및 고장 유형별 실무 조치 기준 도출
- **Stack**: Python · LightGBM · SHAP · Plotly · Streamlit

[![Repo](https://img.shields.io/badge/GitHub-AI4I--Predictive--Maintenance-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/AI4I-Predictive-Maintenance)
[![Demo](https://img.shields.io/badge/Streamlit-Demo-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://ai4i-predictive-maintenance-ddhrq3ekz7dvtdfwrlz4mc.streamlit.app/)

---

## 🛠 Tech Stack

**LLM / AI Backend**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-4B8BBE?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)

**ML / DL**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**Infra / DevOps**  
![AWS](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## 💼 Experience

| 기간 | 기관 | 내용 |
|------|------|------|
| 2024.07 – 2024.08 | **한국리서치** 인턴 연구원 | SPSS 활용, 전국 1,000명 설문 데이터 분석 및 주간 리포트 단독 작성 |
| 2025.11 – 2026.01 | **부트캠프** | 심화 데이터 분석 과정 |
| 2026.02 – 2026.08 | **부트캠프** | AI 영상기법 활용 자율주행·협동로봇 개발자 과정 (진행중) |

---

## 🎓 Education & Certifications

🏫 **한신대학교** 응용통계학과 학사 졸업 (2020.03 – 2025.02)

🏅 **ADsP** (데이터 분석 준전문가) · 2025.06  
🏅 **컴퓨터 활용능력 2급** · 2025.01

---

<div align="center">

**AI 시스템 설계와 LLM 활용에 대해 이야기하고 싶다면 편하게 연락주세요.**

[![Gmail](https://img.shields.io/badge/rkdwl3264@naver.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rkdwl3264@naver.com)

</div>
