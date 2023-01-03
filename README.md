# 2022 빅콘테스트 퓨처스부 (최우수상)
- 목적 : 숲세권 데이터분석을 통한 자연친화교육환경 확대 및 활용방안
- 일정 : 2022.08.30 - 2022.10.14
- 주최 : 과학기술정보통신부, 한국지능정보사회진흥

## 주요 내용
앱 사용성 데이터를 통한 대출신청 예측분석과 모델 기반 군집 분석 및 군집 별 서비스 메시지 제안합니다. 실제로 대출을 신청할 ‘능력’과 ‘의지’를 가진 유저인지, 선호하는 ‘대출 상품은 무엇’인지 복합적으로 고려해 대출신청을 예측했습니다. 앱 사용 시간, 빈도, 변동성으로 앱 유저의 앱 사용 패턴을 파악하고 해석해 서비스 메시지를 제안했습니다.

### 1. 대출 신청 예측 모델
- 대출신청과 비신청 간의 불균형(4:96)의 문제를 해결하기 위해 sampling을 진행. 최종적으로 신청와 비신청의 비율을 10:90로 고정해 학습

- 개인정보, 행동변화정보, 심리적 요인, 상황적 요인을 나타내는 변수로 세분화하고 파생변수 20개를 추가 생성

- 3개월 내에 연수입이 2회 미만 변동된 유저를 실이용자로 필터링해 실이용자와 단순방문자 구분

- LightGBM과 RandomForest을 최종 모델로 선정

### 2. 예측 모델 해석
- 변수중요도
<img width="697" alt="화면 캡처 2023-01-03 181733" src="https://user-images.githubusercontent.com/97178674/210332932-970103e3-3b43-41c9-b9fb-ee69ce442ef4.png">

- Partial Dependence Plot(PDP)

### 3. 앱 사용패턴을 활용한 군집 분석
- 
