# PJ_Funnel_Analysis
Analysis of fashion E-commerce's payment funnel

## 1. 프젝트 주제
 - 패션 이커머스 결제퍼널 개선

## 2. 프로젝트 목적
- 유입대비 이탈이 늘어나고 있는 결제퍼널 분석
- 매출로 이어질 수 있도록 서비스 개선 전략 수립

## 3. 분석과정
a.  현황 분석<br>

  신규가입자 수와 매출이 상승하고 있지만 결제까지 이어지지 않은 고객 상승, 유입 대비 매출층가율 소폭 하락<br>

  <p align="center"><img width="359" alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/7f403ec5-5537-4374-a821-9aea2180c450">
  <img width="329" alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/7ede7dee-1123-4138-9357-816d9bebf9ed"></p>  

<br>

b.  메인 결제퍼널 정의<br>

  결제로 이어지는 여러 경로 중 유입대비 결제 수가 가장 높은 퍼널을 선택<br>
  ('HOMEPAGE' -> 'SEARCH' -> 'ITEM_DETAIL' -> 'ADD_TO_CART' -> 'BOOKING')
  ```
  stream.funnel(
    stages=[
            'HOMEPAGE',
            'SEARCH',
            'ITEM_DETAIL',
            'ADD_TO_CART',
            'BOOKING'
    ],
    funnel_type='closed')
  ```

  <p align="center"><img src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/9efef1f3-fe7f-4562-93a9-a7236ac3afe0" width="600" height="360"> </p><br>


c. 단계별 전환율 분석<br>

ITEM_DETAIL -> ADD_TO_CART로의 전환율이 가장 낮음

<p align="center"> <img width="500" alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/e1e30a1f-3170-492d-aa92-62d3bd406056"></p>

d. 시즌별 분석<br>

메인 퍼널에만 초점을 맞춘 상품 상세페이지의 개선은 트렌드 파악이 어려워 개선에 한계가 있어 각 시즌 퍼널에 대한 전환율 추이 분석

<p align="center">
  <img width="574" alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/d0567b58-ebc4-4b4f-8d04-2d1456b71c05">
</p>
<p align="center"><개선이 필요한 퍼널></p>
<p align="center"> <img width="243" alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/1cc9186a-2be8-4631-ba16-e485682b319b"></p>

e. 결과

상세페이지 랜딩 후 스크롤과 클릭 값이 감소하는 것으로보아 이탈 경우는 2가지로 예상<br>

추측 1. 상세페이지에서 바로 이탈<br>
추측 2. 썸네일만 보고 이탈<br>

-> **상세페이지 첫 랜딩 후, 결제 넛지를 줄 수 있는 부분이 부족하다고 판단**

## 4. 결론
- 리뷰 상단 배치하기
  이전 구매 고객들의 리뷰와 평점을 상단에 배치하여 이탈 방지
- 쿠폰, 할인혜택 상단에 노출
  혜택을 상단에 노출하여 구매욕구 향상<br> 

<p align="center"><예시>
<p align="center"><img width="150" height='300' alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/03ac914f-d12b-43b6-8e26-9f70d8fc6c48">
<img width="140" height='300' alt="image" src="https://github.com/MijeongKim0533/PJ_Funnel_Analysis/assets/152786534/711473cb-70b4-464f-94c7-75e8b4b6488a"></p>
