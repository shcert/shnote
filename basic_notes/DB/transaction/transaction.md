# 트랜잭션 (Transaction)
* 데이터베이스의 상태를 하나의 상태에서 또다른 일관된 상태로 변화시켜주는 일련의 논리적인 연산의 집합을 의미  
* 하나의 논리적 기능을 수행하기 위한 작업의 단위  
* 병행 제어(Concurrency Control) 및 회복 작업(Recovery)의 논리적 작업 단위  
* 하나의 트랜잭션은 완료(Commit)되거나 복귀(Rollback)되어야 함  

# 상태
* 활동(Active)
* 부분 완료(Partially Committed)
* 완료(Committed)
* 실패(Failed)
* 철회(Aborted)

* 활동(Active)
    * 트랜잭션이 실행 중인 상태
* 부분 완료(Partially Committed)
    * 마지막 연산을 처리
    * 데이터베이스에 실행 결과를 적용하기 직전 상태
* 완료(Committed)
    * 데이터베이스에 적용 완료 상태
* 실패(Failed)
    * 트랜잭션 실행 중 오류에 의해 진행불가상태
* 철회(Aborted)
    * 트랜잭션 실패하여 복귀된 상태

# 특징

* 원자성(Atomicity)
    * 트랜잭션의 가장 중요한 성질
    * 연산의 집단(=논리적으로는 하나의 연산임)
    * 불리할 수 없음
    * 모두 반영(All)되거나 전혀 반영되지 않아야 함(Nothing)의 성질이 있음
* 일관성(Consistency)
    * 고정 요소는 트랜잭션 실행 전과 후가 동일해야 함
    * 무결성이 유지되고 모순되지 말아야 함
* 독립성(Isolation, 격리성)
    * 트랜잭션 실행 중 다른 트랜잭션 연산에 침범하지 말아야 함
    * 같은 자원이 여러 트랜잭션에 의해 동시 활용될 수 없어야 함
* 영속성(Durability, 지속성, 계속성)
    * 변화된 상태는 계속해서 유지되어야 함
    * 트랜잭션 성공적 완료 후, 효과는 지속되어야 함

# 연산

* 완료(Commit)
    * 트랜잭션 실행이 성공적으로 종료되었음을 알리는 연산자
    * 데이터 아이템의 값들은 영속성이 보장
    * DB의 상태가 일관성 있는 상태로 변화된 상태
``` sql
DELETE FROM 학생 WHERE 성별=‘남’;
COMMIT;
```

* 복귀(Rollback)
    * 트랜잭션 실행이 실패하였음을 알리는 연산자
    * 트랜잭션이 수행한 결과를 원래의 상태로 복귀시켜야 하는 상태
``` sql
DELETE FROM 학생;
ROLLBACK;
```