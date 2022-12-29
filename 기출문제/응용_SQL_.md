# 응용 SQL

## Aggregate Function

    SELECT
    FROM
    [WHERE]
    GROUP BY
    [HAVING]

## 기출문제

    1. 조건
       1. 대소문자 구분하지 않음
       2. WHERE 구문 사용하지 않음
       3. GROUP BY, HAVING 구문 반드시 사용
       4. 세미콜론 생략 가능
       5. 별칭 사용
       6. 과목별 점수 평균 90 이상
       7. 과목이름, 최소점수, 최대점수 구하기

    SELECT
            과목이름    과목이름
          , MIN(점수)   최소점수
          , MAX(점수)   최대점수
    FROM
            성적
    GROUP BY
            과목이름
    HAVING
            AVG(점수) >= 90

    =============================

    2. 조건
       1. 대소문자 구분하지 않음
       2. WHERE 구문 사용하지 않음
       3. GROUP BY 반드시 사용
       4. 세미콜론 생략 가능
       5. 별칭 반드시 사용
       6. 집계함수 반드시 사용
       7. 학과별 튜플 수를 구하라

    SELECT
            학과            학과
          , COUNT(학과)     학과별튜플수1
          , COUNT(*)        학과별튜플수2
    FROM
            학생
    GROUP BY
            학과

    =============================

    3. 계산

    SELECT
            COUNT(*)
    FROM
            급여
    WHERE
            EMPNO > 100
        AND SAL >= 3000
        OR  EMPNO = 200

    OUTPUT
            1