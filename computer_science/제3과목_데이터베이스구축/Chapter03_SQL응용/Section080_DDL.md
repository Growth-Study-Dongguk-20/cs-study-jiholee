## CS Study - Section080 DDL
### ✏️ Study
#### 💡 DDL(Data Define Language)의 개요
DB 구조, 데이터 형식, 접근 방식 등 DB를 구축하거나 수정할 목적으로 사용하는 언어이다.
- DDL은 번역한 결과가 데이터 사전이라는 특별한 파일에 여러개의 테이블로서 저장된다.
- 종류 : CREATE SCHEMA, CREATE DOMAIN, CREATE TABLE, CREATE VIEW, CREATE INDEX, ALTER TABLE, DROP 등
<br><br>

#### 💡 CREATE SCHEMA
스키마를 정의하는 명령문으로, 스키마의 식별을 위해 스키마 이름과 소유권자나 허가권자를 정의한다.
> CREATE SCHEMA 스키마명 AUTHORIZATION 사용자_id

<br>

#### 💡 CREATE DOMAIN
도메인을 정의하는 명령문으로, 정의된 도메인명은 일반적인 데이터 타입처럼 사용된다.
- 임의의 속성에서 취할 수 있는 값의 범위가 SQL에서 지원하는 전체 데이터 타입의 값이 아니고 일부분일 때, 사용자는 그 값의 범위를 도메인으로 정의할 수 있다.
> CREATE DOMAIN 도메인명 [AS] 데이터_타입  
>        [DEFAULT 기본값]  
>        [CONSTRAINT 제약조건명 CHECK(범위값)];

<br>

#### 💡 CREATE TABLE
테이블을 정의하는 명령문이다.
> CREATE TABLE 테이블명 
>        (속성명 데이터_타입 [DEFAULT 기본값] [NOT NULL], ...
>        [, PRIMARY KEY(기본키_속성명, ...)]
>        [, UNIQUE(대체키_속성명, ...)]
>        [, FOREIGN KEY(외래키_속성명, ...)]
>                [REFERENCES 참조테이블(기본키_속성명, ...)]
>                [ON DELETE 옵션]
>                [ON UPDATE 옵션]
>        [, CONSTRAINT 제약조건명] [CHECK (조건식)]);

<br>

#### 💡CREATE VIEW
뷰(View)를 정의하는 명령문으로, SELECT문을 서브 쿼리로 사용하여 SELECT문의 결과로서 뷰를 생성한다.
- 서브 퀴리인 SELECT문에는 UNION이나 ORDER BY절을 사용할 수 없다.
> CREATE VIEW 뷰명[(속성명[, 속성명, ...])]
> AS SELECT문;

<br>

#### 💡 CREATE INDEX
인덱스를 정의하는 명령문이다.
> CREATE [UNIQUE] INDEX 인덱스명
> ON 테이블명(속성명 [ASC | DESC] [,속성명 [ASC | DESC]])
> [CLUSTER];

<br>

#### 💡 ALTER TABLE
테이블에 대한 정의를 변경하는 명령문이다.
- ADD : 새로운 속성을 추가할 때 사용한다.
- ALTER : 특정 속성의 Default 값을 변경할 때 사용한다.
- DROP COLUMN : 특정 속성을 삭제할 때 사용한다.
> ALTER TABLE 테이블명 ADD 속성명 데이터_타입 [DEFAULT '기본값'];
> ALTER TABLE 테이블명 ALTER 속성명 [SET DEFAULT '기본값'];
> ALTER TABLE 테이블명 DROP COLUMN 속성명 [CASCADE];

<br>

#### 💡 DROP
스키마, 도메인, 기본 테이블, 뷰 테이블, 인덱스, 제약 조건 등을 제거하는 명령문이다.
> DROP SCHEMA 스키마명 [CASCADE | RESTRICT];
> DROP CONSTRAINT 제약조건명;