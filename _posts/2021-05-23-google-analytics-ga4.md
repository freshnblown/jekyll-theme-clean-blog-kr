---
layout: post
permalink: /google-analytics-ga4/
title: '구글애널리틱스 GA4 사용해야 할까?'
date: 2021-05-23 10:35:00 +09:00
feature: '/img/posts/04-google-analytics-ga4/GA4_thumnail.png'
categories:
  - digital-marketing
tags:
  - 구글애널리틱스
  - GA4
  - 디지털마케팅
  - UA와GA4다른점
description: '유니버설 애널리틱스를 사용하다가 GA4 인터페이스를 확인했을 때 너무 많이 달라져 꽤나 놀랐는데, 어떤 것들이 대표적으로 달라졌는지 확인해보자.'
---
## 구글애널리틱스 GA4 사용해야 할까?

웹만 지원했던 구글 애널리틱스의 유니버설 애널리틱스와는 다르게 GA4 는 웹와 앱을 한번에 확인할 수 있는 새로운 형태의 애널리틱스다. 유니버설 애널리틱스를 사용하다가 GA4 인터페이스를 확인했을 때 너무 많이 달라져 꽤나 놀랐는데, 어떤 것들이 대표적으로 달라졌는지 확인해보자.



### 인터페이스가 달라졌다

![UA_home](/img/posts/04-google-analytics-ga4/UA_home.png)

> 유니버설애널리틱스 홈화면

![GA4_home](/img/posts/04-google-analytics-ga4/GA4_home.png)

> GA4 홈화면

기존 유니버설 애널리틱스는 보고서가 크게 실시간/ 잠재고객/ 획득/ 행동/ 전환으로 나뉘어져 있었다. 실시간에서는 홈페이지의 실시간 상황을 분석하고, 잠재고객에서는 홈페이지에 인입된 사용자에 대한 정보를, 획득에서는 사용자의 유입 경로를 확인할 수 있었다. 행동 보고서에서는 획득을 통해 인입된 사용자의 홈페이지 내 행동 흐름이나 이벤트를 확인할 수 있었고 전환에서는 목표를 달성한 사용자의 수치를 확인할 수 있었다.

GA4의 보고서는 UA 보고서와는 다르게 수명주기, 사용자, 이벤트, 탐색, 구성으로 나눌 수 있다.

- 수명주기: 유저가 어떻게 웹사이트를 들어왔는지를 보여주는 획득 보고서와 홈페이지 들어와서 하는 행동이나 이용 패턴등을 보여주는 참여도, 유지, 수익창출 보고서 등을 알 수 있다.
- 사용자: UA에서 잠재고객 보고서에 해당했던 인구통계나 기술 정보를 확인할 수 있다.
- 이벤트: 기존에는 다른 보고서 안에 들어있던 전환과 모든 이벤트가 밖으로 나와 좀더 쉽게 접근할 수 있게 됐다 .
- 탐색: 기존 맞춤 보고서에 해당되는 부분인데 보다 정교화되고 분석 기법이 다양화됐다.
- 구성: 관리 탭에 있던 사용자 세그먼트 지정하는 것이나 사용자 맞춤 정보 분석을 확인할 수 있으며 디버그뷰가 추가됐다.


달라진 화면만 봐도 구글 애널리틱스가 기업의 데이터 분석 활동에 무엇이 중요하다고 판단하는지 알 수 있다. 내가 봤을 때 가장 크게 달라진 부분은 그간 행동이나 전환에 속해있어서 다이렉트로 접속이 어려웠던 이벤트가 밖으로 나온 것이 크게 달라졌으며 기존에 거의 사용되지 않았던 맞춤 보고서가 탐색이라는 보고서로 새롭게 리디자인되어 드러난 것이 주목할 만하다. 무엇보다 그동안 웹만 가능했던 데이터 수집이 앱까지 통합 관리할 수 있다는 점에서 구글은 웹/앱 통합 데이터를 사용자의 모든 이벤트에 따라 맞춤 분석하는 것이 중요하다고 판단했음을 알 수 있다.



### 이벤트가 달라졌다

![유니버설-애널리틱스-이벤트](/img/posts/04-google-analytics-ga4/UA_event.png)

> 유니버설 애널리틱스 이벤트 화면

![GA4-이벤트](/img/posts/04-google-analytics-ga4/GA4_event.png)

> GA4 이벤트 화면

기존에 이벤트는 사용자가 페이지 안에 들어와서 행동을 하는 것에 국한되어 추적됐다. 무엇보다, 기업 관계자가 고객의 특별한 행동에 가치를 매겨 확인하고자 설치한 것에 한정되어 트래킹이 가능했다. 카테고리, 액션, 라벨이라는 항목에 고객 행동 데이터를 일일이 기재하고 매뉴얼로 관리해야 하는 항목이었다.

하지만 GA4에서의 이벤트는 사용자의 행동에서 벗어나 모든 데이터로 확장됐다. 사용자가 웹사이트 또는 앱과 상호작용할 때 트리거 되는 활동인데, 중요한 점은 굳이 코드를 추가하지 않아도 page_view를 비롯한 많은 이벤트를 수집할 수 있다는 것이다. GA4의 이벤트에는 다음 4가지 종류가 있다.

- 자동으로 수집되는 이벤트: GA와 웹/앱과의 기본적인 상호작용으로 트리거되는 데이터. 언어/ 위치/ 기기/ 광고 클릭으로 발행된 유입 등이 해당된다.
- 향상된 측정 이벤트: 페이지 조회, 스크롤, 이탈 클릭, 사이트 검색, 동영상에 호응, 파일 다운로드 등 사용자가 별도로 세팅하지 않아도 구글이 알아서 트래킹하는 이벤트다. https://support.google.com/analytics/answer/9216061
- 추천 이벤트: 개발자가 구현하지만 구글에서 사전 정의한 이름과 매개변수가 있는 이벤트다. 소매/ 전자상거래/ 여행/게임/부동산/교육 등 업종에 따라 구글이 추천하는 이벤트 종류가 있다. 이를 활용해 자체적으로 설정이 가능하다.
- 맞춤 이벤트: UA에서 이벤트를 설정한 것같이 개발자가 직접 이름을 지정하고 구현하는 이벤트. 맞춤 이벤트를 구현하기 전에 자동이벤트로 트래킹되고 있는 것이 아닌지 확인이 필요하다.



### 보고서가 달라졌다

![GA4-보고서](/img/posts/04-google-analytics-ga4/GA4_report.png)

> GA4 보고서 화면

기존 UA 보고서에서는 어떤 보고서든 거의 비슷한 형태의 인터페이스에서 정해진 내용을 맞춤 설정하여 확인할 수 있었다. 하지만 GA4에서는 템플릿을 활용하여 큰 구조 안에서 자유롭게 정보를 필터링해서 볼 수 있다. 또한 UA보고서에서는 제공하지 않았던 기여도 분석이 추가됐다.

- 탐색 분석: UA 맞춤 분석과 같이 원하는 형태의 그래프와 변수를 열과 행으로 설정해 데이터를 분석해볼 수 있다.
- 유입경로 분석: 유저가 어떻게 웹과 앱으로 유입됐고 퍼널에서 이탈했는지 확인할 수 있다.
- 경로 분석: 전환 퍼널에서 유저가 어떤 순서를 취하는지 확인할 수 있다. 기존 UA 보고서의 페이지 흐름과 유사하다.
- 세그먼트 중복 분석: 사용자가 2개 이상의 세그먼트에 속할 때 중복된 비율을 확인할 수 있다. 최대 3개까지 비교 가능하다.
- 동질 집단 분석: 코호트 분석. 특정 이벤트 혹은 전환까지 동질집단별로 얼마나 걸리는지 어떤 패턴을 보이는지 비교 분석할 수 있다.
- 사용자 생애가지 분석: 사용자별 수익 가치가 설정됐을 때 특정 기간 내 발생한 수익 등 사용자의 생애가치 정보를 분석할 수 있다.



## 이제는 GA4를 함께 봐야할 때

그동안 UA로 웹 데이터를 분석하던 사람들에게는 작년 말에 도입된 GA4를 도입하는 것이 망설여질 것이다. 인터페이스가 완전히 달라진 데다가 원래 쓰던 이벤트를 새로 세팅해야 하나 생각도 들 것이다. 하지만 구글에서 ‘차세대’ 구글 애널리틱스라고 하는 만큼 이제는 서서히 옮겨타야할 때가 됐다. 기존에 UA를 쓰던 사람이라면 GA4 속성을 추가해서 병행하여 분석하는 방법을 추천한다. 기존의 데이터를 꾸준히 관리하면서 GA4에서 제공하는 새로운 차원의 데이터를 함께 탐색하면서 언제든지 전환이 가능하기 때문이다.