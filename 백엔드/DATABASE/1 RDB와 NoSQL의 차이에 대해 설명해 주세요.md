---
created: 2023-10-07T09:25
updated: 2023-10-07T18:27
---
# 1. RDB와 NoSQL의 차이에 대해 설명해 주세요.

강경모

#RDB #NoSQL #DataBase

## 답변

<aside>
📌 RDB(Relational Database)는 구조화된 데이터와 정적 스키마를 가지며 복잡한 쿼리 및 ACID 트랜잭션을 지원하고 NoSQL(Not Only SQL)은 다양한 데이터 모델과 동적 스키마, 수평 확장 및 BASE 모델을 통해 높은 확장성과 유연성을 제공합니다.

</aside>

데이터 관리는 디지털 환경에서 핵심적인 역할을 담당하며, RDB(Relational Database)와 NoSQL(Not only SQL)이 주요 접근 방식입니다.                 

RDB는 사전에 정의된 테이블 형태의 데이터 모델을 사용하며, 이는 변경하기 어려운 정적 스키마를 가집니다. 복잡한 쿼리 작성이 가능한 SQL 언어를 사용하여 다양한 데이터 조작을 수행합니다. 그러나 확장성은 주로 수직 확장에 의존하며, ACID 원칙을 따라 데이터 일관성과 무결성을 보장합니다.

반면에 NoSQL은 다양한 형태의 데이터 모델(문서형, 키-값형 등)을 제공하고 동적 스키마를 갖추고 있어 유연함이 특징인 반면, 각 모델별로 다른 쿼리 언어가 사용되어 단순 검색 및 필터링 작업에 주로 이용됩니다. 또한 수평 확장으로 크거나 변화하는 워크 로드에서 용이하며 BASE 원칙을 따라 높은 가용성과 확장성을 갖습니다.

따라서 애플리케이션의 요구 사항에 맞게 RDB와 NoSQL 중 적절한 선택이 필요합니다.

## **꼬리 질문**

### NoSQL의 강점과, 약점이 무엇인가요?

- 쉽게 확장할 수 있어 대량의 데이터 처리와 더 많은 트래픽을 지원하기 용이하고 데이터 모델을 자유롭게 변경이 가능해 필드나 속성을 추가/제거가 쉽습니다. 또한 빠른 성능으로 읽기 및 쓰기 작업을 빠르게 처리할 수 있고 다양한 데이터 모델을 처리할 수 있는 장점이 있습니다.
- SQL과 같은 표준 언어를 갖추고 있지 않아 복잡한 쿼리의 실행이 어려울 수 있고 분산 환경에서 일관성 보장이 되지 않는 경우가 있습니다. 또한 ACID 특징을 완전히 지원하지 않는 경우가 많다는 단점이 있습니다.

### DDL, DML, DCL 이란 무엇인가요?

- 데이터 정의어(DDL, Data Definition Language):
    - 데이터베이스 구조를 정의, 수정, 삭제하는 명령어입니다.
    - 대표적인 명령어로는 CREATE, ALTER, DROP 등이 있습니다.
- 데이터 조작어(DML, Data Manipulation Language)
    
    ```sql
    # 데이터베이스 생성
    CREATE DATABASE my_database;
    
    # 테이블 생성
    CREATE TABLE users (
      id INT NOT NULL AUTO_INCREMENT,
      name VARCHAR(255) NOT NULL,
      email VARCHAR(255) NOT NULL,
      PRIMARY KEY (id)
    );
    
    # 열 정의
    ALTER TABLE users ADD COLUMN age INT;
    
    # 제약 조건 설정
    ALTER TABLE users ADD CONSTRAINT age_positive CHECK (age >= 0);
    ```
    
    - 데이터의 값을 변경하거나 새로운 데이터를 생성하는 명령어입니다.
    - 대표적인 명령어로는 INSERT, UPDATE, DELETE 등이 있습니다.

```sql
# 데이터 삽입
INSERT INTO users (name, email) VALUES ('momo', 'momo@example.com');

# 데이터 수정
UPDATE users SET name = 'momo' WHERE id = 1;

# 데이터 삭제
DELETE FROM users WHERE id = 1;
```

- 데이터 제어(DCL, Data Control Language)
    - 데이터베이스 접근 권한과 보안을 관리하는 명령어입니다.
    - 대표적인 명령어로는 GRANT, REVOKE 등이 있습니다.

```sql
# 사용자 생성
CREATE USER user1;

# 사용자 권한 부여
GRANT SELECT, UPDATE ON my_database.users TO user1;

# 사용자 권한 회수
REVOKE SELECT, UPDATE ON my_database.users FROM user1;
```

## 추가 개념

### 1. 스키마:

- 데이터베이스 내에 어떤 구조로 데이터가 저장되는지 나타내는 데이터베이스 구조입니다.
    - 정적 스키마: 데이터베이스에 저장되는 데이터의 구조가 미리 정의되어 있는 스키마이며 데이터 구조가 명확해서 데이터 관리가 쉽고 무결성을 쉽게 보장한다는 등의 장점이 있지만 데이터 구조를 변경하기 어렵고 유연성이 낮습니다.
    - 동적 스키마: 데이터베이스에 저장되는 데이터의 구조가 런타임에 결정되는 스키마이며 데이터 구조를 유연하게 변경 가능하고 유연성이 높은 대신 데이터 구조가 명확하지 않아 데이터 관리가 어렵고 무결성을 보장하기 어렵습니다.

---

⚠️여기에 각주내용 및 출처, 그림 제목 등에 대해서 달아주세요!!!

표: 노션에서 제공해주는 기본 표 사용. 데이터베이스X

그림: 피그잼으로 도식화하여 사용 ~ 임시로 레퍼런스 사용 가능

코드: 노션에서 제공해주는 코드 블럭 사용 

단축키: ```(백틱 3개)

`백틱`: 메서드 및 코드 블럭에서 사용한 내용을 본문에서 언급할 때 

단축키: 해당 내용을 드래그하여 ctrl+E

인용: 노션에서 제공해주는 기본 스타일 사용

출처가 필요한 내용: *기울게* → 추후 일괄 수정 예정*

⚠️ 질문에 대한 답변 완료 및 저작권, 맞춤법 등의 추가 검사까지 완료

→페이지 아이콘 바꾸기 ✅ 해당 아이콘으로 페이지 아이콘을 바꿔주세요!