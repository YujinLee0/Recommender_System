## Yelp 데이터를 활용한 레스토랑 추천 시스템 
-----
- Yelp Data : 레스토랑을 포함한 여러 비즈니스에 대한 사업 정보와 그에 대한 리뷰, 유저 등의 정보를 가지고 있는 데이터
  - 해당 원본 데이터에서 category에 'restaurant'이 포함되는 레스토랑 관련 데이터만 추출하여 사용함.
  - 또한 review.csv 파일을 메인으로 사용함.

🖥️ 구현 방식 
- 사용자 기반 추천을 위해 user based collaborative filtering 기법을 사용 
- user - item matrix에서 유저 기반 유사도를 구해 이를 기반으로 하나의 레스토랑 추천 리스트를 생성 (list 1)
- 추가적으로 리뷰 데이터를 활용해 tf - idf와 setiment polarity를 활용하여 하나의 레스토랑 추천 리스트를 생성 (list 2)
- list 1과 list2를 반영한 최종 추천 시스템 리스트 구현 
