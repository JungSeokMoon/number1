
===
Chatbot_MorningCoffee
====
Slack 챗봇 프로젝트
이 게시물은 Samsung Software에서 만든 프로젝트

# 주제 선정 배경
-------------
- 아침에 간단하게 모닝커피를 한잔 마시며 체크하는 오늘의 이슈, 오늘의 날씨 등을 알아보는 챗봇

# 요구사항
-------
- 네이버 구미 인동 날씨 사이트를 크롤링하여 제공
- 네이버 뉴스 헤드라인을 크롤링하여 제공
- BUGS 실시간 음악 순위를 크롤링하여 제공
- CGV 영화 예매 순위 사이트를 크롤링하여 제공


# 내부구조
-------
[1] 챗봇 call

![1](https://user-images.githubusercontent.com/46041410/50432491-6d0c5a00-0915-11e9-91b6-d49f3834cca9.PNG)

- 처음 챗봇을 부르거나, 원하는 단어가 없을 시에 나타나는 텍스트

[2] 날씨 정보 call

![2](https://user-images.githubusercontent.com/46041410/50432502-87463800-0915-11e9-8acf-7e7d02eb34ae.PNG)
- 날씨, weather 의 단어가 들어가는 문장을 입력할 시 '오늘'부터 7일간의 '구미 인동'의 날씨를 알려줌

[2-1] 지금 날씨 정보 call


![3](https://user-images.githubusercontent.com/46041410/50432508-8ad9bf00-0915-11e9-97dc-e0133d7b7c22.PNG)

- 지금, now 그리고 날씨, weather의 단어가 들어가는 문장을 입력할 시 현재 '구미 인동'의 날씨를 알려줌
  - 미세먼지의 농도의 나쁨을 기준으로 문장이 변경되어 나옴
  
[3] 오늘의 뉴스 call


![4](https://user-images.githubusercontent.com/46041410/50432504-89a89200-0915-11e9-8673-31f72500f96e.PNG)
- 이슈, news, 뉴스의 단어가 들어가는 문장을 입력할 시 오늘의 주 topic 뉴스를 10개 보여줌

[4] 음악순위 call


![5](https://user-images.githubusercontent.com/46041410/50432505-89a89200-0915-11e9-84f1-56b9726a3682.PNG)
- 음악, music의 단어가 들어가는 문장을 입력할 시 실시간 음악 차트 10개를 보여줌

[5] 영화순위 call


![6](https://user-images.githubusercontent.com/46041410/50432506-8a412880-0915-11e9-9935-de81c214fd32.PNG)
- 영화, movie의 단어가 들어가는 문장을 입력할 시 실시간 음악 예매 순위 7개를 보여줌

  

# 개발환경 
-------- 
- FLASK
- Python
