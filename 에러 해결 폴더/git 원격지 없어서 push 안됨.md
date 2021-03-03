
| | |
|:----------|:----------|
| 상황 | git remote add origin <git-remote-url> 입력후 push 하였는데, permission denied (publickey) fatal: Could not read from remote repository 유저의 ssh가 등록 되지 않아 접근권한이 없어서 생기는 문제| 
|해결| 1. ssh-keygen -t rsa -C "git이메일" |
|    | 2. 생성된 public key 경로 복사|
|    | 3. cat ~/.ssh/id_rsa.pub >> sequence 복사|
|    | 4. 웹브라우저 깃허브 세팅에서 'ssh and gpg keys에 3. 붙여넣기|

