# LogAuHFBCH: Log Auditing emitted by HFB's Chaincode

![alt text](https://github.com/sfl0r3nz05/LogAuHFBCH/blob/main/img/System%20overview.png)

## CASE SOLO 2ORG WITH GOLEVELDB

1. Deploy HFB network
   - cd networks/2org_2peer_solo_goleveldb
   - docker-compose up -d

2. If error "gopath not found":
   find -name gopath
      The container id is returned: 4300e823d5268d558c19370bda0ff2fa61e54c4c743133b5be58634adfbefc3b

3. go get github.com/google/uuid
   sudo cp -rf /home/ubuntu/go/src/github.com/google /var/lib/docker/overlay2/4300e823d5268d558c19370bda0ff2fa61e54c4c743133b5be58634adfbefc3b/diff/opt/gopath/src/github.com/

4. Add use case chaicode container number in filebeat.yml 

### To Do:
 1. Deploy ELK infrastructure
 2. Deploy Hyperledger Explorer
 3. Include Python Script to verify each log
![alt text](https://github.com/sfl0r3nz05/LogAuHFBCH/blob/main/img/System%20overviewII.png)
 4. Include performance evaluation, e.g.:
![alt text](https://github.com/sfl0r3nz05/LogAuHFBCH/blob/main/img/performance.png) 