# Kang Ji Soo



응용통계학을 전공하며 Python 기반 데이터 분석과 머신러닝 프로젝트를 직접 설계·구현해왔습니다.  
인턴 경험을 통해 실무 데이터 분석 역량을 키웠으며, 데이터 기반 의사결정에 기여하는 분석가를 목표로 합니다.

<br>

## 🛠 Tech Stack

**Language**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SPSS](https://img.shields.io/badge/SPSS-052FAD?style=flat-square&logo=ibm&logoColor=white)

**Data Analysis & ML**  
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**Visualization**  
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-4C8CBF?style=flat-square)

**Tools & Infra**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

<br>

## 🚀 Projects

### 🔍 Web Traffic Suspicious Behavior Detection
> 브라우저 DevTools로 수집한 웹 트래픽의 행동 패턴(14개 feature)만으로 정상/의심 트래픽을 분류하는 ML 탐지 시스템

- **개인 프로젝트**
- JavaScript로 14개 feature 추출 함수 직접 구현
- Random Forest: Precision **1.000**, False Positive **0건**, Accuracy **98.0%**
- Chrome Extension과 연동한 end-to-end 경고 흐름 구현
- **Stack**: Python · scikit-learn · TensorFlow.js · Chrome DevTools API

[![Repo](https://img.shields.io/badge/GitHub-Suspicious--Web--Traffic--Analysis-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/Suspicious-Web-Traffic-Analysis-using-Chrome-DevTools)

---

### 🚗 CarGuard — Vehicle Damage Detection System
> 탁송 전·후 차량 이미지를 AI로 분석하여 흠집 심각도(0~4단계)를 자동 판정하는 웹 서비스

- **팀 프로젝트 (4인)** · 담당: 차량 흠집 탐지 파트
- **EfficientNet-B0** Transfer Learning으로 심각도 분류 (val accuracy 64%)
- OpenCV 파이프라인: ECC 정렬 → Canny 엣지 → Morphology → ROI 패치 추출
- 소규모 데이터(126쌍) 한계를 데이터 증강으로 극복 (634개 → 4,190장)
- 0~4단계 심각도 라벨링 기준 직접 설계
- 팀 프로젝트 이후 **FastAPI 서버 · AWS EC2 배포**까지 독립 서비스로 고도화
- **Stack**: Python · PyTorch · OpenCV · FastAPI · AWS EC2

[![Team](https://img.shields.io/badge/팀_프로젝트-vehicle--delivery--ai--system-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/vehicle-delivery-ai-system)
[![Personal](https://img.shields.io/badge/개인_고도화-vehicle--damage--detection-009688?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211/vehicle-damage-detection)

---

### 🏭 설비 고장 예측 대시보드 (Predictive Maintenance)
> AI4I 2020 데이터 기반 설비 고장 사전 탐지 및 비용 절감 시뮬레이션 시스템

- **개인 프로젝트**
- 도메인 지식 기반 파생변수 3개 직접 설계 (Temp_diff / Power / Torque_Wear) — 고장 조건 일치율 **100%** 확인
- LR → RF → XGBoost → LightGBM 순차 실험, Threshold 최적화로 Recall **0.85** / ROC-AUC **0.97** 달성
- SHAP 분석으로 피처별 예측 기여도 시각화 및 고장 유형별 실무 조치 기준 도출
- Streamlit 인터랙티브 대시보드 구현 (실시간 예측 · SHAP · 비용 ROI 계산기)
- **Stack**: Python · LightGBM · SHAP · Plotly · Streamlit

[![Repo](https://img.shields.io/badge/GitHub-AI4I--Predictive--Maintenance-181717?style=flat-square&logo=github)](https://github.com/rkdwltn1211/AI4I-Predictive-Maintenance)
[![Demo](https://img.shields.io/badge/Streamlit-Demo-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://ai4i-predictive-maintenance-ddhrq3ekz7dvtdfwrlz4mc.streamlit.app/)

<br>

## 💼 Experience

| 기간 | 기관 | 내용 |
|------|------|------|
| 2024.07 – 2024.08 | **한국리서치** 인턴 연구원 | SPSS 활용, 전국 1,000명 설문 데이터 분석 및 주간 리포트 단독 작성 |
| 2025.11 – 2026.01 | **부트캠프** | 심화 데이터 분석 과정 |
| 2026.02 – 2026.08 | **부트캠프** | AI 영상기법 활용 자율주행·협동로봇 개발자 과정 (진행중) |

<br>

## 🎓 Education & Certifications

🏫 **한신대학교** 응용통계학과 학사 졸업 (2020.03 – 2025.02)

🏅 **ADsP** (데이터 분석 준전문가) · 2025.06  
🏅 **컴퓨터 활용능력 2급** · 2025.01

<br>

## 🎯 Currently

- 🌱 AI 영상기법 및 자율주행 과정 학습 중
- 🔭 데이터 분석가로 취업 준비 중
- 💬 데이터 분석 / 머신러닝 / 이미지 처리에 대해 이야기하고 싶다면 편하게 연락주세요!

<br>

## 📫 Contact

[![Gmail](https://img.shields.io/badge/rkdwl3264@naver.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rkdwl3264@naver.com)
[![GitHub](https://img.shields.io/badge/rkdwltn1211-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/rkdwltn1211)
