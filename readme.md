전체과정
환경설정
Geth 로컬 구축
Nodejs 설치
소스 다운로드
스마트컨트랙트 작성 및 배포
웹서버 구축
웹클라이언트 구축


Geth 설정 과정
geth --networkid 1234 --datadir "./geth/docu" --rpc --rpcaddr "0.0.0.0" --rpcport 8545 --rpccorsdomain "*" --rpcapi "admin, db, eth, debug, miner, net, shh, txpool, personal, web3" console
명령 프롬프트 추가로 띄움
> geth attach rpc:http://localhost:8545      // 원격 연결 가능여부 확인
> personal.newAccount("1234")                        // 계정 생성
> personal.unlockAccount(eth.accounts[0],"1234")
> miner.start()
> eth.mining
> eth.getBalance(eth.accounts[0])       // 채굴해서 코인생겼는지 확인
