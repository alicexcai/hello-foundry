# logs

Setup
1. setup repo following readme
2. edit and test contract at package/contracts/src/Counter.sol
3. configure test scripts at package/contracts/src/Counter.t.sol
4. run ```forge test -vv```
5. configure scripts under package/contracts/scripts/Deploy.s.sol
6. run ```forge script script/Deploy.s.sol```

Deployment
1. create RPC URL on goerli following [Alchemy tutorial](https://docs.alchemy.com/docs/how-to-add-alchemy-rpc-endpoints-to-metamask#2.-create-an-api-key-for-the-desired-network-on-metamask)
2. set temp env variables in bash/zshrc ```ETH_RPC_URL=<alchemy app https url>```
3. get some eth on goerli at https://goerlifaucet.com/
4. set global env variables with ```sudo vim ~/.zshrc``` and insert
```
export ETH_RPC_API=<alchemy app api key>
export ETHERSCAN_API_KEY=<ehterscan api key>
export ETH_PK=<wallet private key>
```
5. source or open new zsh shell, then test, deploy, and verify following readme