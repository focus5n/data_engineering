# SQL 응용

    집계함수
    그룹함수
    윈도함수

## 집계함수

    GROUP BY
    HAVING [조건식]

## 그룹함수

    최대
    최소
    건수
    계산

    MAX
    MIN
    COUNT
    SUM, AVG, STDDEV, VARIAN

### ROLLUP

    SELECT DEPT, JOB, SUM(SALARY)
    FROM DEPT_SALARY
    GROUP BY ROLLUP(DEPT, JOB)

    마케팅부 총합
    기획부 총합
    부서 총합

### CUBE

    세분화된 소계에 사용
    시스템에 부담이 과함

## 윈도함수

    데이터베이스를 활용한 온라인 분석 처리
    OVER 문구가 필수적으로 포함

    SELECT 함수명(파라미터)
    OVER (
        [PARTITION BY 컬럼1, 컬럼2, ...]
        [ORDER BY 컬럼 A, ...]
        [SORT 정렬방식]
    )
    FROM 테이블명

### RANK

    컬럼 순위
    동일 순위가 존재하면 후순위를 비움 (2위에 2명이 할당되면, 3등은 없으며, 4등부터 시작)

### DENSE_RANK

    레코드 순위
    동일 순위가 존재해도 후순위에 할당 (2위에 2명이 할당되도, 4등이 아니라, 3등부터 시작)
### ROW_NUMBER

    레코드 순위
    순위와 관계없이 순서대로 번호 할당 (2위에 5명이 할당되도, 2, 3, 4, 5, 6등 부여)