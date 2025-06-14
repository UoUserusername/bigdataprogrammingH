# 데이터 기반 여행 콘텐츠 추천 시스템 (빅데이터프로그래밍 H팀)

### Python 버전

- **Python 3.11.13**

### 주요 사용 라이브러리

| 라이브러리        | 버전     | 설명                             |
|------------------|----------|----------------------------------|
| `pandas`         | 2.2.2    | 데이터 처리 및 CSV 로딩          |
| `numpy`          | 2.0.2    | 수치 계산 및 배열 연산           |
| `scikit-learn`   | 1.6.1    | 협업 필터링 및 유사도 계산       |
| `matplotlib`     | 3.10.0   | 데이터 시각화 (그래프 등)        |
| `seaborn`        | 0.13.2   | 통계적 시각화 보조               |
## 📝 파일 설명

### 📦 공통 사용 데이터  
|  | 파일/폴더명 | 설명 |
|--------|--------------|------|
| 📂 | `TL_csv` | 원본 데이터 중 Train용 CSV 파일이 저장된 폴더 |
| 📂 | `VL_csv` | 원본 데이터 중 Validation용 CSV 파일이 저장된 폴더 |


### 📍 관광지 혼잡도 분류 기능  
|  | 파일명 | 설명 |
|--------|--------|------|
| 🛠️ | `congestion_level_labeling.ipynb` | 혼잡도 분류를 위한 최종 데이터를 생성합니다. 혼잡도 라벨링과 특성 엔지니어링 등 데이터 전처리 및 가공 작업을 포함합니다. |
| 🧾 | `activity_consume_final_data.csv` | `congestion_level_labeling.ipynb`에서 생성된 혼잡도 분류용 최종 CSV 데이터 파일입니다. |
| 📊 | `congestion_classification.ipynb` | 3가지 머신러닝 모델을 활용해 혼잡도 분류 학습을 수행합니다. Accuracy, Precision, Recall, F1 Score 비교 및 Feature Importance, SHAP 분석을 포함합니다. |


### 📍 여행지 추천 기능
|  | 파일명 | 설명 |
|--------|--------|------|
|🏕️| `trip_recommendation_system.ipynb` | 협업 필터링을 기반으로 사용자 간 취향 유사도를 계산해 비슷한 사용자가 좋아한 여행지를 추천합니다. |
|  |  |  |
|  |  |  |

---
## 🗂️ 사용 데이터

### AI Hub, '국내 여행로그 데이터(서부권) (2023)'
https://aihub.or.kr/aihubdata/data/view.do?searchKeyword=%EA%B4%80%EA%B4%91%EC%A7%80&aihubDataSe=data&dataSetSn=71779
