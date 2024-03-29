## CS Study - Section065 관계형 데이터베이스의 제약 조건 - 무결성
### ✏️ Study
#### 💡 무결성의 개념 및 종류
무결성이란 DB에 저장된 데이터 값과 그것이 표현하는 현실 세계의 실제 값이 일치하는 정확성을 의미한다.
 - 무결성 제약 조건은 DB에 들어 있는 데이터의 정확성을 보장하기 위해 부정확한 자료가 DB에 저장되는 것을 방지하기 위한 제약 조건을 말한다.
 - 종류 : 개체 무결성, 도메인 무결성, 참조 무결성, 사용자 정의 무결성 등이 있다.
<br><br>

#### 💡 개체 무결성
기본 테이블의 기본키를 구성하는 어떤 속성도 Null 값이나 중복 값을 가질 수 없다는 규정이다.
<br><br>

#### 💡 도메인 무결성
주어진 속성 값이 정의된 도메인에 속한 값이어야 한다는 규정이다.
<br><br>

#### 💡 참조 무결성
외래키 값은 Null이거나 참조 릴레이션의 기본키 값과 동일해야 한다. 즉, 릴레이션은 참조할 수 없는 외래키 값을 가질 수 없다는 규정이다.
<br><br>

#### 💡 사용자 정의 무결성
속성 값들이 사용자가 정의한 제약조건에 만족해야 한다는 규정이다.
<br><br>

#### 💡 데이터 무결성 강화
데이터 품질에 직접적인 영향을 미치므로 데이터 특성에 맞는 적절한 무결성을 정의하고 강화해야 한다.
- 애플리케이션, 데이터베이스 트리거, 제약 조건을 이용하여 강화할 수 있다.
    - 애플리케이션 : 데이텨 생성, 수정, 삭제 시 무결성 조건을 검증하는 코드를 데이터 조작 프로그램 내에 추가한다.
    - 데이터베이스 트리거 : 트리거 이벤트에 무결성 조건을 실행하는 절차형 SQL을 추가한다.
    - 제약 조건