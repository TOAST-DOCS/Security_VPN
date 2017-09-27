## Security > SSL VPN > Getting Started

## TOAST Cloud G SSL VPN 서비스 소개
TOAST Cloud G SSL VPN서비스는 고객의 네트워크(원격지)에서 클라우드 플랫폼 내부에 구성된 고객의 서비스로 접근하기 위한 암호화 되어진 가상사설망을 생성하여 보안 접속 통신을 제공하는 서비스입니다.<br><br>

TOAST Cloud G SSL VPN 구조는 아래와 같습니다. 

<center>![alt](http://static.toastoven.net/prod_gov_security/img_05.png)</center>

TOAST Cloud G의 네트워크는 아래와 같이 2개의 네트워크로 분류 되어집니다.

- Public Network: 이용자가 외부에 서비스를 제공하기 위한 네트워크로 VM에 공인 Floating IP를 부여한 네트워크
- Private Network: 이용자가 CLOUD내에 생성한 시스템을 운영/관리하기 위한 네트워크로 VM에 사설 VPN Network IP를 부여한 네트워크

SSL VPN 서비스를 통해 TOAST Cloud G에 구성되어진 고객 서비스 Private Network으로 언제 어디서든 운영 및 관리를 위해 안전한 접근을 할 수 있습니다 

## TOAST Cloud G SSL VPN 계정 및 접근 시스템 등록 절차

아래의 등록 절차를 통해 SSL VPN을 통해 시스템 접근을 이용하실 수 있습니다.

<center>![alt](http://static.toastoven.net/prod_gov_security/img_06.png)</center>

### Instance VM VPN IP 확인
SSL VPN을 이용하여 접근할 고객 VM의 VPN Floating IP 확인

### 계정 및 ACL 신청서 작성
SSL VPN을 이용하여 접근 할 운영/관리 담당자 계정 신청 및 접속 시스템 ACL 등록 신청서 작성<br>
(아래의 이미지 링크 통해 신청서 Download 및 Sheet. G-TOASCLOUD SSL VPN 계정 및 정책 요청서 작성)
<center>
[![](http://static.toastoven.net/prod_gov_security/img_04.png)](http://static.toastoven.net/prod_gov_security/TOASTCloud G 방화벽 및 SSL VPN 정책 신청서.xlsx)</center>

### SSL VPN 신청서 접수(E-Mail)
TOASTCloud G 대표 메일 support@gov-cloud.toast.com로 접수 신청 메일 발송. (접수일 기준으로 3일 이내 처리 및 회신)

### 신청서 검토 (접수 및 등록)
TOASTCloud G 사업부서에서 작성 내역의 검토 및 처리부서로 이관 등록

### SSL VPN 계정 발급
TOASTCloud G 보안부서에서 요청 내용을 확인하여 계정 생성 및 접근 권한 설정 적용

### 고객사 회신
고객에게 완료 처리 내용 통지

### SSL VPN Agent 설치
처리 완료 메일 수신 후 TOASTCloud G SSL VPN 사용 방법 가이드에 따라 SSL VPN Agent 설치 진행

###	접속
외부 접속용 PC에 설치 되어진 Agent 실행하여 등록되어진 VPN ID를 이용하여 접속합니다.

## TOAST Cloud G SSL VPN 사용 방법 및 이용자 VM 접속 방법
1. TOAST Cloud G SSL VPN Download Page 로그인
<center>![alt](http://static.toastoven.net/prod_gov_security/img_07.png)</center>

- URL창에 https://211.180.235.197:9001 을 입력합니다
- 발급 받으신 ID를 입력 합니다
- 발급 받으신 임시 초기 비밀번호를 입력합니다
- [로그인]을 클릭 합니다

2. TOAST Cloud G SSL VPN Agent Download
<center>![alt](http://static.toastoven.net/prod_gov_security/img_08.png)</center>

- [다운로드] 클릭 합니다
- [저장] 클릭 합니다 
- [저장] 클릭 한 후 계속 Download를 진행 및 Download 되어진 파일을 실행하여 설치합니다

3. TOAST Cloud G SSL VPN Agent 실행
<center>![alt](http://static.toastoven.net/prod_gov_security/img_09.png)</center>

- 다운로드 진행 후 바탕화면에 Client 아이콘이 생성 됩니다
- 설정하신 ID를 입력합니다
- 발급 받으신 임시 초기 비밀번호를 입력합니다
- [로그인] 클릭 합니다 

4. TOAST Cloud G SSL VPN Google OTP 2차 인증 수단 등록 설정
<center>![alt](http://static.toastoven.net/prod_gov_security/img_10.png)</center>

- 핸드폰 기기등에서 Google OTP 어플을 실행시켜 줍니다 
  (기본적으로 설치되어 있을 수도 있고, 없으시다면 Google OTP App을 다운로드 합니다)
- OTP 어플을 실행시켜 [시작] 클릭 후 제공된 키 입력을 선택 합니다
- 계정 이름 입력란에 계정 이름을 설정하여 줍니다
    - 키 입력란에는 16자리의 키를 입력하고 [추가]를 클릭하면 인증번호란이 생성 됩니다
    - 키 값 제한 
        - 안드로이드 8,9를 제외한 모든 숫자, 알파벳을 지원
        - 아이폰 0,1,8,9를 제외한 모든 숫자, 알파벳을 지원
    - 이 값은 SSL VPN Client에도 동일하게 넣어줘야 하는 부분으로 설정 값으로 기억 하셔야 합니다. 

5. TOAST Cloud G SSL VPN Client OTP 2차 인증 등록 설정
<center>![alt](http://static.toastoven.net/prod_gov_security/img_11.png)</center>

- SSL_VPN Client를 실행 하고 설정 한 아이디/비밀번호를 입력 하여 1차 인증 후 2차 인증 OTP 키 입력창이 생성되면 “Step4”에서 입력한 16자리를 키값을 입력합니다.
    - 키값은 최초 한번만 입력하면 됩니다
- OTP 키값이 입력되면 인증번호 입력창이 생성 됩니다
  인증번호는 ③에(Google OTP App) 생성된 6자리를 입력하면 로그인이 됩니다

6. 접속 완료
<center>![alt](http://static.toastoven.net/prod_gov_security/img_12.png)</center>

- ID/PASSWORD 및 2차 인증 성공하면 위와 같이 연결창이 나오며, 접속이 완료 됩니다.

7. 이용자 VM 접속
원격 터미널 접속 Tool[Putty, SecureCRT등]을 이용하여 이용자 VM SSH 연결 진행 (접속 시 VPN Private Floating IP로 접속)
<center>![alt](http://static.toastoven.net/prod_gov_security/img_13.png)</center>










