---
layout: post
title : "Bigquery(SQL) - 데이터 탐색"

toc_sticky: true
---

# Bigquery(SQL)
##데이터 탐색 - 조건, 추출, 요약

1. 데이터 탐색(SELECT, FROM, WHERE)
  * 기초 내용이라 생략

2. 집계(GROUP BY + HAVING + SUM/COUNT)
  * 집계함수는 <code>GROUP BY</code> 사용
  * <code>DISTINCT</code> : 중복 제거 (= GROUP BY)
  * WHERE/HAVING 차이
    * <code>WHERE</code> : 테이블에 바로 조건 적용
    * <code>HAVING</code> : GROUP BY 후 조건 적용
  * 서브 쿼리 : SELECT 문 내에 존재하는 SELECT 쿼리
    * 서브쿼리 바깥에서 WHERE 조건 설정 = 서브쿼리에서 HAVING 조건 설정
  * <code>WHERE "IN"</code> : (= OR)
    ex) WHERE salary IN (1000, 700, 24000)
    * 괄호 안에 있는 value가 있는 row만 추출, 
  * <code>COUNTIF(조건)</code> :
  ex) COUNTIF(칼럼 = "3")

3. 쿼리 작성 전 고려사항
*#쿼리 작성하는 목표, 확인할 지표*
*#쿼리 계산 방법*
*#데이터의 기간*
*#사용할 테이블*
*#join KEY : 연결할 수 있는 것*
*#데이터 특징*
