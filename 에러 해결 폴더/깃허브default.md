| | |
|:----------|:----------|
| 상황 | 깃허브에 push를 해도 잔디밭 미생성
|해결| repository branch default는 main으로 설정했는데, push는 master branch로 하고 있었음 git push origin main --force으로 default에 강제로 때려넣음|


