# 절차형 SQL

    절차지향적 프로그래밍 기능 제공
    트랜잭션 언어

## 종류

    1. Procedure
    2. User-Defined Function
    3. Trigger

## 출력

    1. DBMS_OUTPUT
       1. DBMS_OUTPUT.PUT(문자열);
       2. DBMS_OUTPUT.PUT_LINE(문자열);

## 제어

### IF 구문
    
    IF 조건 THEN
        문장;
    ELSIF 조건 THEN
        문장;
    ELSIF 조건 THEN
        문장;
    ELSE
        문장;
    END IF;

### SIMPLE CASE 구문

    CASE 변수
        WHEN 값1 THEN
            SET 명령어;
        WHEN 값2 THEN
            SET 명령어;
        WHEN 값3 THEN
            SET 명령어;
        ELSE
            SET 명령어;
    END CASE;

### SEARCHED CASE 구문

    CASE
        WHEN 조건1 THEN
            SET 명령어;
        WHEN 조건2 THEN
            SET 명령어;
        ELSE
            SET 명령어;
    END CASE;

### LOOP 구문

    LOOP
        문장
        EXIT WHEN 탈출조건;
    END LOOP;

### WHILE 구문

    WHILE TRUE_조건 LOOP
        문장;
        EXIT WHEN FALSE_조건;
    END LOOP;

### FOR LOOP 구문

    FOR 인덱스
    IN 시작값 .. 종료값
    LOOP
        문장;
    END LOOP;

## 예외(EXCEPTION)

    EXCEPTION
        WHEN 조건 THEN
        SET 명령어;
