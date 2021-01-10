## Overview
erlang chat server 코드실습
erlang으로 여러명의 클라이언트가 접속하는 채팅서버 클라이언트들을 서버에 연결하고 순간적으로 클라이언트 수가 증가될 경우 erlang 서버의 동작 결과예측 

OTP 22에서 컴파일시 GS가 빠져있어 OTP 우분투 16.04버전에서 자동설치로 OTP 18을 이용하였음.

##### 동작예측
채팅프로그램에서 클라이언트 수가 갑자기 증가한다면?
erlang은 메시지 패싱으로 프로세스간의 통신이 이루어져 있다. error와 ok인 경우가 케이스로 나뉘어져 프로세스에 문제가 생기더라도 이를 정상적으로 처리할 프로세스가 만들어져 서버를 안정적으로 구현할 수 있게 될 것으로 예측.

##### 참고
오류메세지 참고 [https://erlang.org/doc/reference_manual/errors.html] [Add1]  
GS [http://erlang.org/documentation/doc-5.6.4/pdf/gs-1.5.9.pdf] [GS]  
TCP 사용함수 참고 [https://erlang.org/doc/man/gen_tcp.html] [TCPF]  

[Add1]: <https://erlang.org/doc/reference_manual/errors.html>
[GS]: <http://erlang.org/documentation/doc-5.6.4/pdf/gs-1.5.9.pdf>
[TCPF]: <https://erlang.org/doc/man/gen_tcp.html>
