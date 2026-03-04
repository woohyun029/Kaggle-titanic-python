# 🚢 Kaggle Titanic - Data Analysis & Feature Engineering

캐글(Kaggle)의 타이타닉 데이터를 활용하여 데이터 분석의 기초부터 특성 공학(Feature Engineering)까지 학습하는 과정입니다.

## 📌 학습 목표
- 데이터의 분포를 파악하는 탐색적 데이터 분석(EDA) 실습
- 다양한 시각화 라이브러리(Matplotlib, Seaborn) 활용 능력 향상
- 실제 모델 학습이 가능하도록 데이터를 정제하는 전처리 기술 습득

## 📂 주요 수행 내용

### 1. 탐색적 데이터 분석 (EDA)
- **Survived:** 생존율 분포 확인 (Pie plot, Count plot)
- **Pclass & Sex:** 객실 등급과 성별에 따른 생존율 차이 분석
- **Age:** KDE plot을 이용한 연령별 밀도 분석 및 누적 생존율 시각화
- **FamilySize:** SibSp와 Parch를 결합한 새로운 피처 생성 및 영향력 분석

### 2. 특성 공학 & 전처리 (Feature Engineering)
- **Initial 추출:** 정규표현식(`str.extract`)을 사용하여 이름에서 호칭을 분리하고, 이를 바탕으로 나이(`Age`)의 결측치를 정교하게 채움
- **Fare 로그 변환:** 데이터 왜도(Skewness)를 줄이기 위해 로그 변환(`np.log`) 적용
- **데이터 수치화:** 문자열 데이터를 `map` 함수와 `get_dummies`를 사용하여 숫자형 및 원-핫 인코딩으로 변환
- **상관관계 분석:** Pearson Correlation Heatmap을 그려 변수 간 밀접도 확인

## 🛠 사용 기술
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Missingno
- **Development Environment:** Jupyter Notebook

## 💡 배운 점
- 단순한 결측치 채우기보다, 다른 변수와의 관계(호칭별 나이 평균 등)를 활용한 정밀한 전처리의 중요성을 배움.
- 수치형 데이터의 치우침을 해결하는 로그 변환의 개념을 익힘.
- 데이터 타입(Interval, Category 등)에 따른 처리 방식의 차이를 경험함.
