---
layout: single
title : "Bigquery(SQL) - 데이터 탐색"
tags : [github, blog]
comments : true
toc : true
toc_sticky: true
---

## 데이터 탐색 - 조건, 추출, 요약  
  
1. 데이터 탐색(SELECT, FROM, WHERE)  
  * 기초 내용이라 생략  

2. 집계(GROUP BY + HAVING + SUM/COUNT)
  * 집계함수는 **GROUP BY** 사용  
  * **DISTINCT** : 중복 제거 (= GROUP BY)  
  * WHERE/HAVING 차이  
      - **WHERE** : 테이블에 바로 조건 적용 (들여쓰기 적용 안됌)  
      - **HAVING** : GROUP BY 후 조건 적용 (들여쓰기 적용 안됌)  
  * 서브 쿼리 : SELECT 문 내에 존재하는 SELECT 쿼리  
      - 서브쿼리 바깥에서 WHERE 조건 설정 = 서브쿼리에서 HAVING 조건 설정  
  * WHERE **IN** (= OR) :  
    ex) WHERE salary IN (1000, 700, 24000)  
      - 괄호 안에 있는 value가 있는 row만 추출  
  * **COUNTIF**(조건)  
  ex) COUNTIF(칼럼 = "3")  
  
3. 쿼리 작성 전 고려사항

*#쿼리 작성하는 목표, 확인할 지표*  
*#쿼리 계산 방법*  
*#데이터의 기간*  
*#사용할 테이블*  
*# join KEY : 연결할 수 있는 것*  
*#데이터 특징*

----
241101
tags, comments, toc, toc_sticky 옵션 추가 
----
241120
서식 수정, comments 적용안됌 ..
