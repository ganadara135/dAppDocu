# 전체과정<br>
## 환경설정<br>
## Geth 로컬 구축<br>
## Nodejs 설치<br>
## 소스 다운로드<br>
## 스마트컨트랙트 작성 및 배포<br>
## 웹서버 구축<br>
## 웹클라이언트 구축<br>


# Geth 설정 과정<br>
### 1. genesis.json 파일을 c:\users\user\geth 폴더 밑으로 이동 <br>
### 2. geth --datadir docu5 init genesis.json console // 채글난이도를 낮추기 위해 필요  <br>
### 3. geth --networkid 1234 --datadir docu5 --rpc --rpcaddr "0.0.0.0" --rpcport \\
### 8545 --rpccorsdomain "*" --rpcapi "admin, db, eth, debug, miner, net, shh, \\
### txpool, personal, web3" console   <br>
### 4. 명령 프롬프트 추가로 띄움 <br>
### 5. > geth attach rpc:http://localhost:8545 // 원격 연결 가능여부 확인 <br>
### 6. > personal.newAccount("1234") // 계정 생성  <br>
### 7. > personal.unlockAccount(eth.accounts[0],"1234") <br>
### 8. > miner.start() <br>
### 9. > eth.mining <br>
### 10. > eth.getBalance(eth.accounts[0]) // 채굴해서 코인생겼는지 확인  <br>
