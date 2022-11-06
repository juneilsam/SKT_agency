영등포구 SKTelecom 공식 대리점 입지 선정 프로젝트

[notion - portfolio](https://indecisive-strand-a7c.notion.site/SKT-6fec5badd5e14c5084272f9f3d04f480)

[GitHub - juneilsam/SKT_agency](https://github.com/juneilsam/SKT_agency)

### 📆_기간

- 2022년 05월 ~ 2022년 05월(1개월)

### 🖍_주제 및 동기

- 영등포구 소재 유동 인구 데이터 기반 입지 선정 분석
- SKT 이용자를 유동 인구로 집계한 데이터이기 때문에 가장 높은 가치를 도출할 수 있는 주제는 SKT와 관련된 입지 선정이라고 판단

### 🛠_사용 기술

- 사용 언어 - Python3
- Tool - Jupyter Notebook, Google Colab
- 사용 라이브러리 - sklearn, Pandas, Numpy, Geopandas 등

### 📃_프로젝트 요약

- 영등포구의 SKT 기지국 기반 유동 인구 데이터를 기본으로 하여, 필요한 데이터를 수집하고 SKT 공식 대리점의 입지를 예측해본다.
- 수집한 데이터는 다음과 같다.
    - 영등포구 지리 데이터
    - 2019 09월 영등포 인구 현황
    - 서울시 지하철 역 정보
    - 서울시 버스 정류소 정보
    - 서울시 상권 정보 : 매출, 영역
    - SKT 공식 대리점 정보
- 수집한 데이터에 대하여 EDA로 기술 통계를 파악하고, 시각화를 진행하여 형태를 파악한다.
- 모든 데이터를 geopandas, pandas 등을 이용하여, 필요한 데이터 형태로 가공한다.
    - Geopandas의 buffer, points_from_xy, sjoin_nearest, within, unary_union 등
    - Pandas의 데이터 프레임 병합, 분할, 생성 등
- 기존 대리점의 특징을 파악해본 뒤, 새로운 입지의 기준으로 삼는다.
    - 인구 밀도의 정도
    - 지하철 역, 버스 정류장과의 거리, 수 등
    - 상권과의 거리 등
- 입지 분석의 방법은 다음과 같다.
    - 비지도 학습(군집 분석. K-Means, DBSCAN)
    - 지도 학습(Random Forest)
- 기업 블로그에 기재됨
    
    [통신사 대리점, '이곳'이 최적입니다! 입지 선정 분석 리포트 공개 (Feat. SKT)](https://www.biviz.ai/blog/read/?id=67)
    

### 🎭_주요 역할

- SKT 입지 선정에 필요한 데이터 수집
- 데이터의 여러 특징을 기준으로 통계치를 추출하고 시각화하여 목적에 맞는 특징을 선택하고 가공한다.
- EDA 분석한 결과와 주제를 고려하여 적합한 ML 알고리즘을 선정한다.
- 모델을 통해 추출된 결과를 시각화 하고 분석한다.
