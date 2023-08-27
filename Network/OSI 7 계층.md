# OSI 7 계층



- OSI 7 계층이란
  
  - 네트워크 프로토콜이 통신하는 구조를 7개의 계층으로 분리한 것이며, 각 계층간 상호 작동하는 방식을 정해 놓은 것
  
  - ISO(International Organization for Standardization_국제표준화기구)에서 만든 네트워크 통신 7단계
  
  - 각 계층이 어떤 역할을 하고 있는지 알 수 있는 일종의 메뉴얼
  
  - 각 계층별로 모듈화가 되어 있어서 각 계층을 하나로 보는 것이 아니라 융화시켜 호환성에 용이하도록 만들었음
  
  - 각 계층별 용어
    
    - 7계층: 응용 계층 (HTTP, SMTP, POP, FTP, SSH 등) (Application Layer)
    
    - 6계층: 표현 계층 (Presentation Layer)
    
    - 5계층: 세션 계층 (Session Layer)
    
    - 4계층: 전송 계층 (TCP/UDP) (Transport Layer)
    
    - 3계층: 네트워크 계층 (IP, ICMP, ARP) (Network Layer)
    
    - 2계층: 데이터 링크 계층 (Ethernet) (Data Link Layer)
    
    - 1계층: 물리 계층 (전선, 전파, 광섬유) (Physical Layer)



![OSI 모델과 TCP_IP 모델 계층 비교.png](https://github.com/TaeDongUm/CS_Study/blob/main/Network/images/OSI 모델과 TCP_IP 모델 계층 비교.png)

                    <출처: [네트워크 통신에 필수적인 프로토콜 이해하기 | 와탭 블로그](https://www.whatap.io/ko/blog/160/)>    

- 특징:
  
  - 계층을 나누게 되면 통신이 일어나는 과정을 단계별로 알기 쉽고, 특정한 계층에 이상이 생기면 그 단계만 개선하면 된다.
    
    - 다른 계층은 건드리지 않으며 유지, 관리도 수월해짐
  
  - 상하구조를 가진다.
    
    - 상위 계층의 프로토콜이 제대로 동작하기 위해선 하위의 모든 계층에 문제가 없어야 한다.



### 제 1계층 : 물리 계층(Physical Layer)

- 물리계층
  
  - 컴퓨터는 전기적 특성 ON(1) 과 OFF(0) 2 가지 만으로 데이터를 읽음
  
  - 아날로그 신호를 디지털 신호로(Encoding), 디지털 신호를 아날로그 신호로(Decoding) 바꾸는 과정이 필요
  
  - 상위 계층(Data Link)에서 전송된 데이터를 물리적인 전송 매체(허브, 라우터, 케이블 등)를 통해 다른 시스템에 전기적 신호를 전송하는 역할
  
  - 데이터를 전기적인 신호로 변환해서 주고받는 기능만 수행할 뿐, 어떤 데이터인지, 어떤 에러가 발생했는지 판별하지 않음

- 특징:
  
  - 단위는 BIT
  
  - 물리매체(공기, UTP, STP 케이블, 광케이블, 네트워크 장치 등)를 통해 데이터 전송 및 수신
  
  - 대표 프로토콜: Coax, Fiber, Wireless
  
  - 미디어 타입, 커넥터 타입, 신호표현 방법(시그널링), 속도 등을 정의한다.
  
  - 주요 장비: 허브(HUB), 리피터(Repeater), 네트워크 카드 (NIC : Network Interface Card) 등
    
    - 허브: 여러 대의 컴퓨터, 네트워크 장비를 연결하는 장치(공유기)
    
    - 리피터: 신호가 더 멀리 갈 수 있도록 도와주는 장치
    
    - 네트워크 카드:  0과 1의 정보를 전기적 신호로 바꿔주는 역할
    
    - 모뎀: 신호변조


