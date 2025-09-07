# Chat_program
## 프로젝트 소개
리눅스 환경에서 콘솔을 이용해 여러명의 클라이언트가 단체채팅을 할 수 있는 프로그램<br/> 
## 구성인원
1명
## 기술 스택
![a](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=cpp&logoColor=white) ![b](https://img.shields.io/badge/TCP_IP-03234B?style=for-the-badge&logo=TCP_IP&logoColor=white) ![c](https://img.shields.io/badge/Multi_thread-03234B?style=for-the-badge&logo=Multi_thread&logoColor=white) ![d](https://img.shields.io/badge/Linux-FF6F00?style=for-the-badge&logo=linux&logoColor=white)
## 역할
-멀티스레드 기반 TCP/IP 통신서버, 클라이언트 구현 <br/>

## 사용법
1. 리눅스 환경에서 chat_server_linux.c 와 char_clnt_linux.c 를 다운받습니다.
2. 콘솔에서 `gcc chat_server_linux.c -D_REENTRANT -o chat_server_linux -lpthread`  를 입력하여 서버C파일을 실행파일로 컴파일 합니다.
3. 마찬가지로 클라이언트 C파일도 gcc chat_clnt_linux.c -D_REENTRANT -o chat_clnt_linux -lpthread  를 입력하여 실행파일을 만듭니다.
4. 콘솔에서 ./chat_server_linux 9190  을 입력하여 서버를 실행시킵니다.
5. 다른 콘솔을 틀고 ./chat_clnt_linux 127.0.0.1 9190 Kim 을 입력하여 클라이언트1을 접속시킵니다.
6. 또 다른 콘솔을 틀어 ./chat_clnt_linux 127.0.0.1 9190 Park  을 입력하여 클라이언트2를 접속시킵니다.
7. 이와같은 방식으로 계속해서 클라이언트를 늘려갈 수 있습니다. 이제 클라이언트 콘솔에서 채팅을 입력하면 다른 클라이언트에게 채팅이 전달됩니다. 서로 채팅이 가능해집니다.
