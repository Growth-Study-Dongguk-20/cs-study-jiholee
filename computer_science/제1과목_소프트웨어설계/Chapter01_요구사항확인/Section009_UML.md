## CS Study - Section009 UML(Unified Modeling Language)
### ✏️ Study
#### 💡 UML(Unified Modeling Language) 의 개요
시스템 분석, 설계, 구현 등 시스템 개발 과정에서 의사소통이 원활하게 이루어지도록 표준화한 대표적인 객체지향 모델링 언어
- 6개의 구조 다이어그램 + 7개의 행위 다이어그램으로 사물과 사물 간의 관계를 용도에 맞게 표현한다.
- 구성 요소 : 사물, 관계, 다이어그램
<br><br>

#### 💡 UML 구성요소 1) 사물(Things)
모델을 구성하는 가장 중요한 기본 요소로, 다이어그램 안에서 관계가 형성될 수 있는 대상

| 사물                       | 내용                                                  |
|--------------------------|-----------------------------------------------------|
| 구조 사물(Structure Things)  | - 시스템의 개념적, 물리적 요소를 표현<br/>- 클래스, 유스케이스, 컴포넌트, 노드 등 |
| 행동 사물(Behavioral Things) | - 시간과 공간에 따른 요소들의 행위를 표현<br/>- 상호작용, 상태 머신 등        |
| 그룹 사물(Grouping Things)   | - 요소들을 그룹으로 묶어서 표현<br/>- 패키지                        |
| 주해 사물(Annotation Things) | - 부가적인 설명이나 제약조건 등을 표현<br/>- 노트                     |

<br><br>

#### 💡 UML 구성요소 2) 관계(Relationships)
사물과 사물 사이의 연관성을 표현한 것
- 종류 : 연관(실선과 화살표), 집합(실선과 마름모), 포함(실선과 채워진 마름모), 일반화(실선과 속이 빈 화살표), 의존(점선과 화살표), 실체화(점선과 속이 빈 화살표) 등
<br><br>

#### 💡 UML 구성요소 3) 다이어그램(Diagram)
사물과 관계를 도형으로 표현한 것
- 종류 : 구조적 다이어그램(정적 모델링), 행위 다이어그램(동적 모델링)
- 구조적 다이어그램 : 클래스, 객체, 컴포넌트, 배치, 복합체 구조, 패키지
- 행위 다이어그램 : 유스케이스, 순차, 커뮤니케이션, 상태, 활동, 상호작용 개요, 타이밍