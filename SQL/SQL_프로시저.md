# Procedure

    함수처럼 쿼리 집합을 하나의 단어로 실행

## 선언

    DECLARE
    BEGIN
        CONTROL 조건문 반복문
        SQL DQL DML
        EXCEPTION
        TRANSACTION COMMIT ROLLBACK
    END

## 문법

    MODE == IN | OUT | INOUT

    CREATE [OR REPLACE] PROCEDURE 프로시저_명칭(파라미터_명칭 [MODE] 데이터_타입, ...)
    IS
        변수선언
    BEGIN
        명령어;
    [COMMIT | ROLLBACK]
    END;

## 실행

    SQL> EXECUTE 프로시저_명칭 (파라미터1, 파라미터2, ...)