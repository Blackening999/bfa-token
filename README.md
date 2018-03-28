## BitFinance Access Token

Investigation results: https://docs.google.com/document/d/1ySddONsecz_Dea0FLVIIdvLMh7pTMTifijtTBxvdzgA
Security concerns: https://docs.google.com/document/d/1Yt_fvr-uJGD0D7WmUGbdjCYzJ2OAXPfqnT1FNDqz24Q
How to Participate in Token Sale: https://blog.matryx.ai/matryx-public-token-sale-how-to-participate-tips-on-staying-safe-4270017df0f6
^ update with our own article

TODO:
1. update tests
2. test on testnet and play via Mist Wallet
3. analyse Solidity 0.4.13 - 0.4.21 versions
4. decide on MultiSigWallet usage and test it if so

```
Total Supply: 1,000,000,000 BFA
Name: BFAToken
Symbol: BFA
Ether Cap: 219,058 Eth
```

## Requirements

npm/node
eth testrpc
truffle

## Install

```npm i```

## Compile Contracts

```truffle compile```

## Deploy Contracts

Set unix epoch for start and end time

```truffle migrate```

## Test

run via npm script

`npm run test`

or

install testrpc

```
npm install -g ethereumjs-testrpc

```

Run testrpc chain

ex
```
testrpc -b 1.5 --account="0xc7dcd9e96b41cb0f5d3d519550966fc36e9472f92be7d16af3638e600a48d588,2000000000000000000000000" --account="0xb6485e6830a5d9aff97fa9d799c16aa9e387a2eea684c4b7d2c9f656798e2710,15000000000000000000000000"
```

set test bool to true in /migrations/2_deploy_contracts.js
run truffle tests

```truffle test```

Credits:
TokenMarket ( https://tokenmarket.net )
Matryx ( https://tokenmarket.net/blog/matryx-token-and-token-sale-smart-contract-audit/ )