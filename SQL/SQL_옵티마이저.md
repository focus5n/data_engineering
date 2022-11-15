# Optimizer

    쿼리 성능을 튜닝하기 위하여 사용

## Cost Based Optimizer, CBO

    비용 기반 옵티마이저

## Hint

    옵티마이저가 항상 최선을 선택을 할 수는 없음.
    명시적인 힌트를 통해 실행계획을 변경.

    /*+ RULE */
    /*+ CHOOSE */
    /*+ INDEX(테이블명 인덱스명) */
    /*+ USE_HASH(테이블명) */
    /*+ USE_MERGE(테이블명) */
    /*+ USE_NL(테이블명) */
