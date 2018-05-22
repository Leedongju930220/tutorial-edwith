# 웹의 동작 원리
![Alt text](http://tcpschool.com/lectures/img_webbasic_10.png)

### 순서
+ HTTP
+ Request 형식
+ Request Method
+ Response 형식
+ 응답 코드


## 1단계 HTTP
+ HTTP란?<br/>
 0 www에서 정보를 주고 받을때 사용하는 프로토콜이며 80번 포트를 사용<br/>
 1 TCP기반의 통신방식 (3-way handshake)<br/>
 2 비연결 지향<br/>
 3 단방향 지향<br/>
 4 평문전송<br/>
 평문을 전송하기에 보안에 취약하다.<br/>
 보안방법 : <br/>
 1. 통신자체를 암호화 : SSL(Secure Socket Layer) or TLS(Transport Layer Security)라는 다른 프로토콜을 조합함으로써 HTTP의 통신 내용을 암호화할 수     있다. SSL을 조합한 HTTP를 HTTPS(HTTP Secure) or HTTP over SSL이라고 부른다.<br/>
 2. 콘텐츠를 암호화 : 말 그대로 HTTP를 사용해서 운반하는 내용인, HTTP 메시지에 포함되는 콘텐츠만 암호화하는 것이다. 암호화해서 전송하면 받은 측에서는     그 암호를 해독하여 출력하는 처리가 필요하다.<br/>
 ## HTTPS > SSL을 사용하는 HTTP라고 보면 된다.<br/>
+ HTTP 는 브라우저가 웹 서버와 통신하기 위해 사용하는 주요 프로토콜이다. 요청형식으로는 4가지가 있다.<br/>
 1 GET : 문서를 요청. 서버가 클라이언트에 상태 정보와 복제된 문서를 보냄으로써 응답을 함. (조회)<br/>
 2 HEAD : 상태 정보를 요청. GET 과 동일한 형태로 응답을 하지만, 문서를 복제하지는 않는다.<br/>
 3 POST : 데이터를 서버로 송신. 서버는 해당 데이터를 특정 아이템에 덧붙인다. (생성)<br/>
 4 PUT : 데이터를 서버로 송신. 서버가 특정 아이템을 완전히 대체한다. (수정)<br/>
