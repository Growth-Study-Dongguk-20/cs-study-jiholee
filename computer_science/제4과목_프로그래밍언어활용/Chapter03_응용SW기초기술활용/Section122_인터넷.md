## CS Study - Section122 인터넷
### ✏️ Study
#### 💡 인터넷의 개요
인터넷이란 TCP/IP 프로토콜을 기반으로 하여 전 세계 수많은 컴퓨터와 네트워크들이 연결된 광범위한 컴퓨터 통신망이다.
- 유닉스 운영체제를 기반으로 한다.
- 모든 컴퓨터는 고유한 IP 주소를 갖는다.
- 컴퓨터 또는 네트워크를 연결하기 위해 브리지, 라우터, 게이트웨이가 사용된다.
- 인터넷의 주가되는 기간망을 일컫는 용어를 백본이라고 한다.
<br><br>

#### 💡 IP 주소
IP 주소는 인터넷에 연결된 모든 컴퓨터 자원을 구분하기 위한 고유한 주소이다.
- 숫자로 8비트씩 4부분, 총 32비트로 구성되어 있다.
- IP 주소는 네트워크 부분의 길이에 따라 A~E Class로 구성된다.
  - A Class : 국가나 대형 통신망에 사용되며, 0~127로 시작한다. 단, 0과 127은 예약된 주소이다.
  - B Class : 중대형 통신망에 사용되며, 128~191로 시작한다.
  - C Class : 소규모 통신망에 사용되며, 192~223로 시작한다.
  - D Class : 멀티캐스트 용으로 사용되며, 224~239로 시작한다.
  - E Class : 실험적 주소이며 공용되지 않는다.
<br><br>

#### 💡 서브네팅
서브네팅은 할당된 네트워크 주소를 다시 여러 개의 작은 네트워크로 나누어 사용하는 것을 말한다.
- 4byte의 IP 주소 중 네트워크 주소와 호스트 주소를 구분하기 위한 비트를 서브넷마스크라고 하며, 이를 변경하여 네트워크 주소를 여러 개로 ㅂㄴ할하여 사용한다.
- 서브넷마스크는 각 클래스마다 다르게 사용한다.
<br><br>

#### 💡 IPv6(Internet Protocol version 6)의 개요
IPv6은 현재 사용하고 있는 IP 주소 체계인 IPv4의 주소 부족 문제를 해결하기 위해 개발되었다.
- 128bit의 긴 주소를 사용하여 주소 부족 문제를 해결할 수 있으며, IPv4에 비해 자료 전송 속도가 빠르다.
- 인증성, 기밀성, 데이터 무결성의 지원으로 보안 문제를 해결할 수 있다.
- IPv4와 호환성이 뛰어나다.
- 주소의 확장성, 융통성, 연동성이 뛰어나며, 실시간 흐름 제어로 향상된 멀티미디어 기능을 지원한다.
- Traffic Class, Flow Label을 이용하여 등급별, 서비스별로 패킷을 구분할 수 있어 품질 보장이 용이하다.
- 패킷 크기를 확장할 수 있으므로 패킷 크기에 제한이 없다.
- 기본 헤더 뒤에 확장 헤더를 더함으로써 더욱 다양한 정보의 저장이 가능해져 네트워크 기능 확장이 용이하다.
- 미리 예약된 알고리즘을 통해 고유성이 보장된 주소를 자동으로 구성할 수 있다.
- IPv4 -> IPv6 전략
  - 듀얼 스택 : 호스트에서 IPv4와 IPv6을 모두 처리할 수 있도록 두 개의 스택을 구성하는 것
  - 터널링 : IPv6 망에서 인접한 IPv4망을 거쳐 다른 IPv6 망으로 통신할 때 IPv4 망에 터널을 만들어 IPv6 패킷이 통과할 수 있도록 하는 것
  - IPv4/IPv6 변환 : 헤더 변환, 전송 계층 릴레이 방식, 응용 계층 게이트웨이 방식
<br><br>

#### 💡 IPv6의 구성
- 16bit씩 8부분, 총 128bit로 구성되어 있다.
- 각 부분을 16진수로 표현하고, 콜론으로 구분한다.
- IPv6은 다음과 같이 세 가지 주소 체계로 나누어진다.
  - 유니캐스트 : 1:1
  - 멀티캐스트 : 1:n
  - 애니캐스트 : 1:1(가장 가까이 있는 단일 수신자 통신)
<br><br>

#### 💡도메인 네임
숫자로 된 IP 주소를 사람이 이해하기 쉬운 문자 형태로 표현한 것이다.
- 호스트 컴퓨터 이름, 소속 기관 이름, 소속 기관의 종류, 소속 국가명 순으로 구성되며, 왼쪽에서 오른쪽으로 갈수록 상위 도메인을 의미한다.
- 문자로 된 도메인 네임을 컴퓨터가 이해할 수 있는 IP 주소로 변환하는 역할을 하는 시스템을 DNS라고 하며, 이런 역할을 하는 서버를 DNS 서버라고 한다.