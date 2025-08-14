# EDA(Exploratory Data Analysis; 탐색적 데이터 분석)란?

### 1. 탐색적 데이터 분석 (Exploratory Data Analysis)?

   데이터 분석 초기에 수행하는 과정으로, 데이터를 다양한 각도에서 관찰하고 이해하는 절차를 **탐색적 데이터 분석(Exploratory Data Analysis, EDA)** 이라고 합니다.   
   이는 본격적인 분석에 들어가기 전에 데이터를 직관적으로 파악하기 위해 시각화 자료나 기본 통계값(평균, 중앙값 등)을 생성하여 살펴보는 과정입니다.   
   즉, 데이터 수집과 전처리가 끝난 후, 목적에 맞는 분석을 시작하기 전에 그래프, 차트, 요약 통계치 등을 통해 데이터를 한 발짝 떨어져 객관적으로 바라보고, 데이터의 특성과 잠재적인 패턴이나 이상치를 탐색하는 단계라고 할 수 있습니다.   

### 2. 탐색적 데이터 분석이 중요한 이유
   - 데이터 수집 및 전처리 과정에서 미처 발견하지 못했던 문제를 발견할 수 있습니다.
   - 실제 데이터를 수집해 펼쳐놓고 보면, 데이터 수집 전에 생각해보지 못했던 데이터 간의 패턴을 발견할 수 있습니다.
   - 본격적으로 데이터 분석에 돌입할 때 사용할 데이터 분석 도구를 선정하는 데 도움이 됩니다. 또한 추가 자료 수집 여부를 결정하는 속도도 빨라집니다.


### 3. 탐색적 데이터 분석의 여러가지 방법
   - 기술 통계 방법으로 확인
       - std(), value_counts(), describe() 등의 방법으로 데이터의 구조 및 값 확인
   - 데이터 시각화로 확인
       - histplot, boxplot, violinplot, scatterplot, pairplot, heatmap, countplot, barplot 등으로 확인   
         matplotlib, seaborn, pandas등의 시각화 툴로 확인
   - 결측치 확인
       ```python
       df.isnull().sum() # 결측지 개수 확인
       df.isnull().mean().sort_values(ascending=False) *100 # 결측지 비율 확인
       ```
   - 이상치 확인   
       - IQR, z-score 등등
   - 중복값 확인
