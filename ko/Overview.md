## Security > SSL VPN > 개요

SSL VPN이란 인터넷과 같은 공중망 환경에서 전용회선을 이용하는 것과 같이 내부 정보시스템을 안전하게 관리/운영/사용 할 수 있도록 SSL 프로토콜, 인증, 암호화 기술, 터널링 기술등을 적용하여 안전한 Virtual Private Network(가상사설네트워크) 제공해주는 보안기술을 말합니다.

### 서비스 구조

TOAST G SSL VPN서비스는 고객의 네트워크(원격지)에서 클라우드 플랫폼 내부에 구성된 고객의 서비스로 접근하기 위한 암호화 되어진 가상사설망을 생성하여 보안 접속 통신을 제공하는 서비스입니다.

TOAST G SSL VPN 구조는 아래와 같습니다.

![VPN 개요](http://static.toastoven.net/prod_gov_security/ssl-vpn-1.png)

### 네트워크 분류

TOAST G의 네트워크는 아래와 같이 2개의 네트워크로 분류 되어집니다.

- Public Network : 이용자가 외부에 서비스를 제공하기 위한 네트워크로 VM에 공인 Floating IP를 부여한 네트워크

- Private Network : 이용자가 CLOUD내에 생성한 시스템을 운영/관리하기 위한 네트워크로 VM에 사설 VPN Network IP를 부여한 네트워크

SSL VPN 서비스를 통해 TOAST G에 구성되어진 고객 서비스 Private Network으로 언제 어디서든 운영 및 관리를 위해 안전한 접근을 할 수 있습니다.
