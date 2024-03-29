## CS Study - Section062  E-R(개체-관계) 모델
### ✏️ Study
#### 💡 E-R(Entity-Relationship) 모델의 개요
E-R 모델은 개념적 데이터 모델의 가장 대표
- 데이터를 개체, 관계, 속성으로 묘사한다.
- 특정 DBMS를 고려한 것이 아니다.
- 1:1, 1:N, N:M 등의 관계 유형을 제한 없이 나타낼 수 있다.
<br><br>

#### 💡 ERD(E-R Diagram)
E-R 다이어그램은 E-R 모델의 기본 아이디어를 시각적으로 표현하기 위한 그림이다.

| 기호          | 기호 이름 | 의미 |
|-------------|--------|-----------|
| □ | 사각형 | 개체 타입|
| ◇ | 마름모 | 관계 타입 |
| ○ | 타원 | 속성 |
| ◎ | 이중 타원 | 다중값 속성 |
| ⊖ | 밑줄 타원 | 기본키 속성 |
| ○○ | 복수 타원 | 복합 속성 |
| □-◇-□ | 관계 | 개체 간 관계에 대한 대응수를 선 위에 기술 |
| - | 선, 링크 | 개체 타입과 속성을 연결 |