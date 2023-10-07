---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# DataBase

1. 데이터베이스 인덱스의 장단점은 무엇인가요?   [ 중복 : 4 ]
    1. [출처: [https://land-turtler.tistory.com/120](https://land-turtler.tistory.com/120) ]
    
    ```jsx
    장점
    - 테이블의 검색 및 정렬 속도를 향상
    - 질의나 보고서에서 그룹화 작업의 속도를 향상
    - 테이블 행의 고유성 강화
    - 필드 중에-+는 데이터 형식떄문에 인덱스 될 수 없는 필드도 있다.
    - 여러 필드로 이루어진(다중 필드) 인덱스를 사용하면 첫 필드 값이 같은 레코드도 구분할 수 있다.
    ```
    
    ※ 필드? [ [http://wiki.hash.kr/index.php/필드_(데이터베이스)](http://wiki.hash.kr/index.php/%ED%95%84%EB%93%9C_%28%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%29) ]
    
    데이터베이스에서 세로 방향으로 표시한 컬럼(Column)
    
2. 관계형 데이터베이스(RDBMS)와 Not Only SQL(NoSQL) 데이터베이스의 주요 차이점은 무엇인가요? [ 중복 : 3 ]
    1. [ 출처: [https://dev-coco.tistory.com/158](https://dev-coco.tistory.com/158) ]
    
    ```jsx
    RDBMS:  모든 데이터를 2차원 테이블로 표현하며, 테이블의 단위는 row 와 column으로 이루어져있다. sql을 사용해 관계형 연산을 하며, 하나의 고성능 머신에 데이터를 저장하는 수직적 확장방식. → 데이터가 자주 수정되는 경우, 스키마가 변경될 여지가 없고, 명확한 스키마가 중요한 경우 사용되는 것이 좋다.
    ※ 스키마?  [[https://coding-factory.tistory.com/216](https://coding-factory.tistory.com/216)]
    ```
    
    ```jsx
    NoSQL: 테이블간 관계를 정의하지 않고, 독립적으로 설계됨. 데이터를 여러서버에 분산시키는 분산형 구조에 용이하고, 대용량 데이터 처리에 적합하다.
    ```
    
3. ACID 원칙이 무엇을 나타내는지 설명해주세요. [ 중복 : 3 ]
    1. [ 출처: [https://burning-camp.tistory.com/91](https://burning-camp.tistory.com/91) ]
    
    ```jsx
    트랜잭션의 특성 4가지
    Atomic(원자성) - 트랜잭션의 작업이 전부 실행되거나, 전부 실행이 되지 않거나를 보장하는 것
    Consistency(일관성) - 트랜잭션이 성공적으로 완료되면 일관적인 DB상태를 유지하는 것.
    Isolation(고립성) - 트랜잭션 실행 중에는 다른 트랜잭션이 끼어들지 못한다.
    Duration(영구성) - 트랜잭션이 실행 뒤에 commit 된 사항은 영구적으로 반영되는 것.
    ```
    
    ※ 트랜잭션? [  [https://burning-camp.tistory.com/91](https://burning-camp.tistory.com/91) ]
    
    여러개의 작업을 하나로 묶은 단위(모두 실행되거나 모두 실행되지 않는다.)
    
4. 데이터베이스 샤딩(Sharding)이란 무엇인가요? [ 중복 : 1 ]
    1. [ 출처: [https://velog.io/@min9288/백엔드-기술-면접-질문데이터베이스 ]](https://velog.io/@min9288/%EB%B0%B1%EC%97%94%EB%93%9C-%EA%B8%B0%EC%88%A0-%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4)
    
    ```jsx
    테이블을 row(가로)단위로 분산하여 저장하는 방법. (수평파티셔닝)
    샤드 Key를 정하는 방법에 따라서 샤드 종류가 결정된다.
    (Hash Sharding / Dynamic Sharding)
    ```
    
5. 데이터베이스 복제(Replication)와 샤딩의 차이점을 설명해주세요. [ 중복 : 1 ]
    1. [ 출처: [https://dreamcoding.tistory.com/102](https://dreamcoding.tistory.com/102) ]
    
    ```jsx
    2대 이상의 DBMS를 나눠서 데이터를 저장하는 방식. (DB를 이중화)
    ```
    
    최소 구성은 Master / Slave 구성 → 여러 개의 DB를 권한에 따라 수직적인 구조(Master-Slave)로 구축하는 방식
    
6. ORM(Object-Relational Mapping)이란 무엇이며 어떤 이점을 제공하나요? [ 중복 : 1 ]
    1. [ 출처: [https://velog.io/@heumheum2/면접-질문-복기](https://velog.io/@heumheum2/%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8-%EB%B3%B5%EA%B8%B0) ]
    
    ```jsx
    객체와 관계형 데이터베이스의 데이터를 자동으로 연결해주는 개념. 
    장점
    - SQL Query 문을 길게 쓸 필요없이 ORM 메소드로 데이터들을 제어할 수 있어 프로그래머가 로직에 더 집중할 수 있게 도와줍니다.
    - 각종 역할에 대해 객체나 함수로 만들어서 하기 때문에 코드 가독성 및 유지보수의 편리성이 증가한다.
    - DBMS를 교체하는 거대한 작업에도 비교적 적은 리스크와 시간이 소요된다.
    - SQL Injection 공격을 막아주는 기능이 있어 버그나 해킹가능한 요소들을 줄여줍니다.
    ```
    
    ※ ORM? [ [https://gmlwjd9405.github.io/2019/02/01/orm.html](https://gmlwjd9405.github.io/2019/02/01/orm.html) ]
    
    객체와 관계형 데이터베이스(RDBMS)의 데이터를 자동으로 매핑해주는 것.
    
7. 데이터베이스 정규화(Normalization)와 역정규화(Denormalization)에 대해 설명해주세요. [ 중복 : 3 ]
    1. [ 출처: [https://hyonee.tistory.com/41](https://hyonee.tistory.com/41) ]
    
    ```jsx
    정규화
    데이터 무결성을 유지하기 위해 잘 정의된 방식으로 테이블을 분할 하여 데이터베이스에서 중복 데이터를 제거하는 프로세스. → 관계형 데이터베이스에서 중복을 최소화하기 위해서 데이터를 구조화하는 작업. → 많은 저장공간을 절약한다.
    
    비정규화
    복잡한 Query 속도를 높이고 성능을 향상시키기 위해 테이블에 중복 데이터를 추가한다.
    ```
    
8. Redis와 같은 인메모리 데이터베이스의 장점은 무엇인가요?
    1. [ 출처: [https://liamkwo.github.io/interview2/](https://liamkwo.github.io/interview2/) ]
    
    ※ Redis란? key-value store NOSQL DB입니다.
    
    ```jsx
    싱글스레드로 동작하며 자료구조를 지원합니다.
    그리고 다양한 용도로 사용될 수 있도록 다양한 기능을 지원합니다. 
    데이터의 스냅샷 혹은 AOF 로그를 통해 복구가 가능해서 어느정도 영속성도 보장됩니다.
    ```
    
9. 데이터베이스 트랜잭션 격리 수준(Isolation Levels)에 대해 설명하고 각 수준의 차이를 말씀해주세요. [ 중복 : 2 ]
    1. [ 출처: [https://theheydaze.tistory.com/582](https://theheydaze.tistory.com/582) ]
    
    ```jsx
    READ UNCOMMITTED: 다른 트랜잭션에서 커밋되지 않은 내용도 참조할 수 있습니다.
    READ COMMITED: 다른 트랜잭션에서 커밋된 내용만 참조할 수 있습니다.
    REPEATABLE READ: 트랜잭션에서 진입하기 이전에 커밋된 애용만 참조할 수 있습니다.
    SERIALIZABLE: 트랜잭션에 진입하면 락을 걸어 다른 트랜잭션이 접근하지 못하도록 합니다.
    ```