🚢 Kaggle Titanic: End-to-End Data Analysis
데이터 가공부터 통계적 가설 검정, 모델링, SQL 쿼리까지 단계별 데이터 분석 프로세스 수행
캐글(Kaggle)의 타이타닉 데이터를 활용하여 단순한 시각화를 넘어, 통계적 유의성을 검증하고 예측 모델을 구축하며 데이터 추출 능력을 배양하는 과정을 기록한 저장소입니다.

📌 프로젝트 목표
- 데이터 기반 의사결정: 시각적 패턴을 통계적 수치(p-value)로 증명하는 분석 역량 강화
- 통계적 추론: 변수 간 상관관계를 가설 검정을 통해 논리적으로 해석
- 예측 모델링: 로지스틱 회귀를 통한 생존 확률 예측 및 모델 성능 지표 이해
- 데이터 추출: SQL을 활용하여 실무 환경에서의 데이터 조회 및 집계 능력 확보

📂 주요 수행 내용 및 파일 구성
1️⃣ EDA & Feature Engineering
결측치 정밀 전처리: 이름(Name)에서 호칭(Initial)을 정규표현식으로 추출하여 연령대(Age) 결측치를 논리적으로 보정
왜도(Skewness) 해결: 요금(Fare) 데이터의 치우침을 해결하기 위해 로그 변환(Log Transform) 적용
특성 생성: 가족 규모(FamilySize) 등 파생 변수 생성을 통한 생존 요인 다각화
2️⃣ Inferential Statistics Test
범주형 변수 검정: 성별(Sex), 객실 등급(Pclass)과 생존 여부 간의 관계를 **카이제곱 검정(Chi-square Test)**으로 유의성 확인
수치형 변수 검정: 연령(Age), 요금(Fare)에 따른 생존 차이를 T-test 및 ANOVA를 통해 통계적으로 증명
결과 해석: 시각적으로 보이는 차이가 우연인지, 통계적으로 유의미한지 판단하는 리터러시 함양
3️⃣ Logistic Regression & Inference
분류 모델 구현: Scikit-learn을 활용한 로지스틱 회귀(Logistic Regression) 모델 구축
모델 평가: Accuracy뿐만 아니라 Precision, Recall, F1-score를 통해 모델의 다각적 성능 검증
계수 해석: 각 변수의 계수(Coefficient)와 Odds Ratio를 통해 특정 요인이 생존 확률에 미치는 영향력 정량화
4️⃣ SQL Queries for Data Analysis
데이터 조회 역량: Pandas-SQL 연동을 통해 실제 DB 환경과 유사한 쿼리 실습
복합 쿼리 작성: CASE WHEN을 활용한 연령대별 그룹화, GROUP BY와 HAVING을 이용한 생존 통계 산출
실무 시뮬레이션: 데이터프레임을 테이블로 간주하고 조건 필터링 및 집계 수행

🛠 Tech Stack
1. Language: Python, SQL
2. Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scipy(Stats), Scikit-learn
3. Tools: Jupyter Notebook, Git/GitHub

💡 Key Learnings (배운 점)
1. 데이터 전처리의 힘: 단순히 데이터를 깨끗이 만드는 것을 넘어, 도메인 지식(호칭 등)을 활용해 소실된 정보를 복원하는 과정의 중요성을 깨달았습니다.
2. 숫자 뒤의 논리: 시각화 결과에 안주하지 않고 통계 검정을 통해 '근거 있는 분석'을 수행하는 습관을 길렀습니다.
3. 모델의 해석력: 예측 결과 자체보다 어떤 변수가 결과에 큰 영향을 미쳤는지(Feature Importance)를 파악하는 것이 분석가의 핵심 역할임을 배웠습니다.
