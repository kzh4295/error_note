| | |
|--|--|
|상황|오라클 클라우드 opc@ip주소: Permission denied (publickey,gssapi-keyex,gssapi-with-mic)로 서버 접속불가|
|해결시도 |1) 인스턴스 하단의 콘솔창에 접속하여 초기 설정한 ssh를 변경하려고 시도|
||cat .ssh/id_rsa.pub 로 ssh확인>> ssh 입력 (미해결)|
||2)sudo vi /etc/hosts로  ip 주소가 잘못되었나 확인 (미해결)
||3)sudo vi /etc/ssh/sshd_config에서 password 설정 변경 후 systemctl restart ssh하려고 시도 (미해결)
||4) sudo vi /Users/pro/.ssh/known hosts 명령어로 처음 접속하는 host에서 잘못 된 게 있는지 확인하려고 시도 (미해결)
||5)ssh -o ProxyCommand로 인스턴스 내에 콘솔창에서 직접 접속하려고 시도하고 재부팅 시도 (미해결)|
|해결|기존 oracle cloud에 등록해 놓은 ssh가 있는데, 팀플 과정에서 ssh를 등록하기 위해 ssh key를 찾아야 하는 것을 새로 key-gen하게 되어 접속불가한 거 였음 
