## CS Study - Section082 DML
### ✏️ Study
#### 💡 DML(Data Manipulation Language)의 개요
DML은 데이터베이스 사용자가 응용 프로그램이나 질의어를 통해 저장된 데이터를 실질적으로 관리하는데 사용되는 언어이다.
- DML은 데이터베이스 사용자와 데이터베이스 관리 시스템 간의 인터페이스를 제공한다.
- 유형 : SELECT, INSERT, DELETE, UPDATE
<br><br>

#### 💡 INSERT INTO~
삽입문은 기본 테이블에 새로운 튜플을 삽입할 때 사용한다.
> INSERT INTO 테이블명([속성명1, 속성명2, ...])
> VALUES (데이터1, 데이터2, ...);

<br>

#### 💡 DELETE FROM~
삭제문은 기본 테이블에 있는 튜플들 중에서 특정 튜플을 삭제할 때 사용한다.
> DELETE FROM 테이블명
> [WHERE 조건];

<br>

#### 💡 UPDATE~ SET~
갱신문은 기본 테이블에 있는 튜플들 중에서 특정 튜플의 내용을 변경할 때 사용한다.
> UPDATE 테이블명
> SET 속성명 = 데이터[, 속성명=데이터, ...]
> [WHERE 조건];
