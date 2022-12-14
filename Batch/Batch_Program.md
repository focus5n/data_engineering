# Batch Program

## 유형

    1. 조건을 충족: event batch
    2. 명시적 요구: ondemand batch
    3. 정기적 배치: 정기 배치

## 특징 (정기 배치)

    1. 대용량 데이터를 처리한다.
    2. 특정 시간에 실행한다.
    3. 일괄적으로 처리한다.

## 배치 스케쥴러

    일괄 처리(Batch Processing)를 주기적으로 발생하거나 반복적으로 발생하는 작업을 지원

## Cron 표현식

    리눅스
    1. 분   0 ~ 59
    2. 시간 0 ~ 23
    3. 일   1 ~ 31
    4. 월   1 ~ 12, JAN ~ DEC
    5. 요일 1 ~ 7,  SUN ~ SAT
    6. 연도 1970 ~ 2099

    쿼츠
    1. 초   0 ~ 59
    2. 분   0 ~ 59
    3. 시간 0 ~ 23
    4. 일   1 ~ 31
    5. 월   1 ~ 12, JAN ~ DEC
    6. 요일 1 ~ 7,  SUN ~ SAT
    7. 연도 1970 ~ 2099

    특수문자
    * 모든 수
    ? 해당 항목을 미사용
    - 기간 설정
    . 특정 기간 설정
    / 시작시간과 반복간격 설정
    L 마지막 기간에 동작
    W 가장 가까운 평일에 동작
    # 몇 번째 주, 요일 설정

    특수문자 의미
    초 분 시 일 월 요일
    0 0 12 * * ?        매일 12시에 실행
