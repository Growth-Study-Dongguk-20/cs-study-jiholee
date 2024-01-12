## CS Study - Section029 트리(Tree)
### ✏️ Study
#### 💡 트리의 개요
정점(Node)과 선분(Branch)을 이용하여 사이클을 이루지 않도록 구성한 그래프의 특수한 형태이다.
- 하나의 기억 공간을 노드라고 하며, 노드와 노드를 연결하는 선을 링크라고 한다.
- 디그리(Degree) : 각 노드에서 뻗어 나온 가지의 수, 차수
- 단말 노드(Terminal node) : 자식이 없는 노드(Degree=0)
- 트리의 디그리 : 노드들의 디그리 중 가장 큰 수
<br><br>

#### 💡 트리의 운행법
1. Preorder 운행 : Root -> Left -> Right
2. Inorder 운행 : Left -> Root -> Right
3. Postorder 운행 : Left -> Right -> Root
<br><br>

#### 💡 수식의 표기법
산술식을 계산하기 위해 이진 트리를 많이 사용한다.
- Preorder : 전위 표기(PreFix) +12
- Inorder : 중위 표기(InFix) 1+2
- Postorder : 후위 표기(PostFix) 12+