# TCP vs UDP

## TCP와 UDP란?

네트워크 계층 중 전송 계층에서 사용하는 프로토콜로 **데이터의 전달을 담당**

> 전송 계층은 송신자와 수신자를 연결하는 통신 서비스를 제공하는 계층

![그림으로 비교하는 TCP vs UDP](/Network/images/tcpvsudp1.png)

<br>

## TCP(Transmission Control Protocol)

애플리케이션 사이에서 **안전하게 데이터를 통신하는 규약**

- **TCP 특징**

1. 연결 지향적 프로토콜로 가상 회선 방식을 제공

   > 3-way handshaking 과정을 통해 연결을 설정하고, 4-way handshaking 과정을 통해 해제

2. 흐름 제어 및 혼잡 제어 기능 수행

   - 흐름 제어 : 데이터를 송수신하는 곳의 처리 속도를 조절하여 수신자의 오버플로우를 방지

   - 혼잡 제어 : 네트워크 내의 패킷 수가 넘치지 않도록 방지

3. 높은 신뢰성을 보장

4. UDP보다 속도가 느림

5. 전이중(Full-Duplex)과 점대점(Point to Point) 방식을 사용

   - 전이중(Full-Duplex) : 전송이 양방향으로 동시에 일어날 수 있음

   - 점대점(Poing to Point) : 각 연결이 정확히 2개의 종단점을 가지고 있음

- **TCP 사용사례**
  <br>

  파일 전송(FTP), 웹 브라우징, 이메일 등 신뢰성과 순서가 중요한 애플리케이션

  <br>

## UDP(User Datagram Protocol)

보안과 신뢰성보다 전송 속도와 효율성이 더 중요한 프로토콜

- **UDP 특징**

1. 비연결형 프로토콜로 데이터그램 방식을 제공

   > 연결을 설정하고, 해제하는 과정이 존재하지 않음

2. 정보를 주고 받을 때 정보를 보내거나 받는다는 신호절차를 거치지 않음

3. 신뢰성이 낮음

4. TCP보다 속도가 빠름
   > 패킷에 순서를 부여하여 재조립을 하거나 흐름 제어 또는 혼잡 제어와 같은 기능도 처리하지 않기 때문에 속도가 빠름

- **UDP 사용사례**
  <br>

  실시간 스트리밍, 온라인 게임, VoIP 등 빠른 전송이 중요하고 데이터 손실을 허용할 수 있는 애플리케이션

  <br>

## TCP와 UDP 비교

![표로 비교하는 TCP vs UDP](/Network/images/tcpvsudp2.png)

<br>

### 참고자료

https://dev-coco.tistory.com/144

https://chanhan.tistory.com/entry/CS-TCP%EC%99%80-UDP%EB%9E%80

https://docs.tosspayments.com/resources/glossary/tcp

https://developer.mozilla.org/ko/docs/Glossary/UDP
