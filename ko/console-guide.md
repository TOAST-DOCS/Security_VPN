## Security > SSL VPN > 사용 가이드

### NHN Cloud(공공기관용) SSL VPN 계정 및 접근 시스템 등록 절차

아래의 등록 절차를 통해 SSL VPN을 통해 시스템 접근을 이용하실 수 있습니다.

![등록 절차](https://static.toastoven.net/prod_gov_security/ssl-vpn-2.png)

\<SSL VPN 계정 발급 및 ACL 신청 프로세스\>

   1. Instance VM VPN IP 확인 : SSL VPN을 이용하여 접근 할 고객 VM의 VPN Floating IP 확인
   2. 계정 및 ACL 신청서 작성 : SSL VPN을 이용하여 접근 할 운영/관리 담당자 계정 신청 및 접속 시스템 ACL 등록 신청서 작성
      (아래의 Link를 통해 신청서 Download 및 신청서 작성)
      
      [![](https://static.toastoven.net/prod_gov_security/fileicon_download_excel.png)](https://static.toastoven.net/prod_gov_security/NHN%20Cloud%20%EB%B0%A9%ED%99%94%EB%B2%BD%20%EB%B0%8F%20SSL%20VPN%20%EC%A0%95%EC%B1%85%20%EC%8B%A0%EC%B2%AD%EC%84%9C.xlsx)
   
   3. SSL VPN 신청서 접수(E-Mail) : NHN Cloud(공공기관용) 대표 메일 support@gov.toast.com로 접수 신청 메일 발송 (접수일 기준으로 3일 이내 처리 및 회신)
   4. 신청서 검토 (접수 및 등록) : NHN Cloud(공공기관용) 사업부서에서 작성 내역의 검토 및 처리부서로 이관 등록
   5. SSL VPN 계정 발급 : NHN Cloud(공공기관용) 보안부서에서 요청 내용을 확인하여 계정 생성 및 접근 권한 설정 적용
   6. 고객사 회신 : 고객에게 완료 처리 내용 통지
   7. SSL VPN Agent 설치 : 처리 완료 메일 수신 후 NHN Cloud(공공기관용) SSL VPN 사용 방법 가이드에 따라 SSL VPN Agent 설치 진행
   8. 접속 : 외부 접속용 PC에 설치 되어진 Agent 실행하여 등록되어진 VPN ID를 이용하여 접속
<BR>

### NHN Cloud(공공기관용) SSL VPN 사용 방법 및 이용자 VM 접속 방법

Step1. NHN Cloud(공공기관용) SSL VPN Download Page 로그인

![로그인](https://static.toastoven.net/prod_gov_security/ssl-vpn-3-1.png)

   1. URL창에 SSL VPN 사용 리전에 맞는 도메인 주소를 입력합니다.
      * KR1(판교) 리전 : [https://gov-sslvpn.nhncloud.com:9001](https://gov-sslvpn.nhncloud.com:9001/)
      * KR2(평촌) 리전 : [https://kr2-sslvpn.gov-nhncloud.com:9001](https://kr2-sslvpn.gov-nhncloud.com:9001/)
   2. 발급 받으신 ID를 입력합니다.
   3. 발급 받으신 임시 초기 비밀번호를 입력합니다.
   4. **\[로그인\]**을 클릭합니다.

   
Step2. NHN Cloud(공공기관용) SSL VPN Agent Download

![Agent 다운로드](https://static.toastoven.net/prod_gov_security/ssl-vpn-4-1.png)

   1. **\[다운로드\]** 클릭합니다.
   2. **\[저장\]** 클릭합니다.
   3. **\[저장\]** 클릭한 후 계속 Download를 진행 및 Download 되어진 파일을 실행하여 설치합니다.

   
Step3. NHN Cloud(공공기관용) SSL VPN Agent 실행

![Agent 실행](https://static.toastoven.net/prod_gov_security/ssl-vpn-5.png)

   1. 다운로드 진행 후 바탕화면에 Client 아이콘이 생성됩니다.
   2. 설정하신 ID를 입력합니다.
   3. 발급 받으신 임시 초기 비밀번호를 입력합니다.
   4. **\[로그인\]**을 클릭합니다.

※ NHN Cloud(공공기관용) KR1(판교)/KR2(평촌) 리전 접속변경 방법

![Agent 접속변경](https://static.toastoven.net/prod_gov_security/ssl-vpn-5(230613).png)

   1. SSLVPN Agent 실행 후 하단 ‘자동 접속 정보 설정’ 메뉴를 선택합니다.
      * KR1(판교) 리전 : [https://gov-sslvpn.nhncloud.com:9001](https://gov-sslvpn.nhncloud.com:9001)
      * KR2(평촌) 리전 : [https://kr2-sslvpn.gov-nhncloud.com:9001](https://kr2-sslvpn.gov-nhncloud.com:9001)
   2. 자동 접속 정보 설정 팝업창에서, 접속할 리전의 Use 항목을 선택합니다.
   3. 서버 설정 사용 확인 창에서 ‘예(Y)’를 선택합니다.


Step4. NHN Cloud(공공기관용) SSL VPN Google OTP 2차 인증 수단 등록 설정

![OTP 2차 인증](https://static.toastoven.net/prod_gov_security/ssl-vpn-6.png)

   1. 핸드폰 기기 등에서 Google OTP 앱을 실행시켜 줍니다.
      (기본적으로 설치되어 있을 수도 있고, 없으시다면 Google OTP 앱을 다운로드 합니다.)
   2. OTP 앱을 실행시켜 **\[시작\]** 클릭 후 제공된 키 입력을 선택합니다.
   3. 계정 이름 입력란에 계정 이름을 설정하여 줍니다.
      키 입력란에는 16자리의 키를 입력하고 **\[추가\]**를 클릭하면 인증번호란이 생성됩니다.
      ※ 키 값 제한 - 안드로이드 8,9를 제외한 모든 숫자, 알파벳을 지원
         * 아이폰 0,1,8,9를 제외한 모든 숫자, 알파벳을 지원
      ※ 이 값은 SSL VPN Client에도 동일하게 넣어줘야 하는 부분으로 설정 값으로 기억 하셔야 합니다.

   
Step5. NHN Cloud(공공기관용) SSL VPN Client OTP 2차 인증 등록 설정

![OTP 2차 인증 등록 설정](https://static.toastoven.net/prod_gov_security/ssl-vpn-7(230613).png)

   1. SSL\_VPN Client를 실행 하고 설정 한 아이디/비밀번호를 입력 하여 1차 인증 후 2차 인증 OTP 키 입력창이 생성되면 “Step4”에서 입력한 16자리를 키값을 입력합니다.
      \※ 키값은 최초 한번만 입력하면 됩니다.
   2. OTP 키값이 입력되면 인증번호 입력창이 생성 됩니다.
      인증번호는 ③에(Google OTP App) 생성된 6자리를 입력하면 로그인이 됩니다.


Step6. 접속 완료

![접속 완료](https://static.toastoven.net/prod_gov_security/ssl-vpn-8(230613).png)

   * ID/PASSWORD 및 2차 인증 성공하면 위와 같이 연결창이 나오며, 접속이 완료 됩니다.


Step7. 이용자 VM 접속

   * 원격 터미널 접속 Tool\[Putty, SecureCRT등\]을 이용하여 이용자 VM SSH 연결 진행 (접속 시 VPN Private Floating IP로 접속)

![VM 접속](https://static.toastoven.net/prod_gov_security/ssl-vpn-9(230613).png)

<BR>

   
### Q&A

Q. 사용자 계정 PASSWORD 변경은 어떻게 하나요?<br>
```
A. NHN Cloud (공공기관용) SSL VPN Client 프로그램을 이용하여 아래와 같이 Password 변경 기능을 제공하고 있습니다.
```

![Password 변경](https://static.toastoven.net/prod_gov_security/ssl-vpn-10(230613).png)

- 열쇠 모양을 클릭하게 되면 오른쪽의 화면이 나타납니다.
  (비밀번호 변경하기 위해선 먼저 Client에 접속한 뒤 변경 가능합니다)
- 기존 비밀번호를 입력합니다.
- 변경 할 비밀번호를 입력합니다.
- [변경] 클릭 합니다.


Q. 이용기관의 데이터를 서버로 이전 시 어떻게 옮겨야 하나요?<br>
```
A. NHN Cloud (공공기관용) SSL VPN을 실행하여 암호화 되어진 가상사설망을 통해 데이터 이전을 안전하게 이관할수 있도록 제공하고 있습니다.
```

![데이터 이관](https://static.toastoven.net/prod_gov_security/ssl-vpn-11(230613).png)

- NHN Cloud (공공기관용) SSL VPN Client 실행 및 로그인
- 데이터 Upload Tool[WinScp등]을 이용하여 이용자 VM 접속
- 이관이 필요한 데이터 전송


Q. KR1(판교)리전 SSL VPN 사용 중에 추가로 KR2(평촌)리전 SSL VPN을 사용이 필요할 경우, 어떻게 KR2(평촌)리전을 사용(등록) 하나요?<br>
```
A. NHN Cloud SSL VPN Client 프로그램은 KR1(판교)리전 / KR2(평촌)리전 동일한 버전의 프로그램으로, SSL VPN Client 프로그램의 접속 정보 설정을 추가하여 KR1(판교)리전 / KR2(평촌)리전 모두 사용이 가능합니다. 
```

![데이터 이관](https://static.toastoven.net/prod_gov_security/ssl-vpn-12(230613).png)

※ 접속 서버 추가 설정 내용

    - KR1(판교) 리전, 접속 URL : gov-sslvpn.nhncloud.com / Port : 9001 / SSL : 사용 check
    - KR2(평촌) 리전, 접속 URL : kr2-sslvpn.gov-nhncloud.com / Port : 9001 / SSL : 사용 check
    
### 참고
- SSL VPN 계정 생성 이후 30일 이내 접속 이력이 없으면 유휴 계정으로 전환되며, 90일 미접속 시 계정이 삭제됩니다.
