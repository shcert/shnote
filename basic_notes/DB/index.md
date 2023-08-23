# 인덱스(INDEX)

인덱스의 특징

-데이터를 빠르게 찾을 수 있는 수단

-데이터베이스 성능에 많은 영향을 주는 DBMS의 구성 요소

-인덱스는 테이블과 클러스터에 연관되어 독립적인 저장 공간을 보유하며, 데이터베이스에 저장된 자료를 더욱 빠르게 조회하기 위하여 사용되는 것

-인덱스는 테이블의 특정 레코드(=튜플=행)의 위치를 알려주기 위해 사용됨

-자동생성이 안 되는 구성요소. 연월일, 이름 기준 인덱스는 자동생성되지 않음

*기본키(PRIMARY KEY) 컬럼 한정으로 자동 인덱스 생성

-'테이블 이름' 컬럼에 인덱스가 없는 경우 : 테이블 전체 내용을 검색한다 (TABLE FULL SCAN)

| 종류              | 내용                                                                                                                                |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| 순서 인덱스       | 데이터 정렬된 순서대로 생성되는 인덱스<br>B-TREE 알고리즘 활용(오름차순/내림차순 지정가능)                                          |
| 해시 인덱스       | 해시 함수에 의해 직접 데이터 키 값으로 접근하는 인덱스<br>데이터 접근 비용 동일, 튜플(행, ROW) 양에 무관                            |
| 비트맵 인덱스     | 각 컬럼에 적은 개수 값이 저장된 경우 선택하는 인덱스<br>수정 변경이 적을 경우 유용(생년월일, 상품번호)                              |
| 함수기반 인덱스   | 수식이나 함수를 적용하여 만든 인덱스                                                                                                |
| 단일 인덱스       | 하나의 컬럼으로만 구성된 인덱스<br>주 사용 컬럼이 하나일 경우 사용                                                                  |
| 결합 인덱스       | 두 개 이상의 컬럼으로 구성한 인덱스<br>WHERE 조건으로 사용하는 빈도가 높은 경우 사용                                                |
| 클러스터드 인덱스 | 기본 키(PK) 기준으로 레코드를 묶어서 저장하는 인덱스<br>저장 데이터의 물리적 순서에 따라 인덱스가 생성<br>특정 범위 검색 시 유리함  |

인덱스 생성 - CREATE [UNIQUE] INDEX 인덱스명 ON 테이블명(컬럼명);

인덱스 변경 - ALTER [UNIQUE] INDEX 인덱스명 ON 테이블명(컬럼명);

인덱스 삭제 - DROP INDEX 인덱스명;