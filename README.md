# SDC Token
SDC token smart contract

## install @openzeppelin/contracts

```shell
npm install
```

## modify

1. edit solidity source in `internal` directory
2. flatten solidity source in `internal` directory to `contracts` directory

```shell
truffle-flattener internal/SDCToken.sol | sed '/SPDX-License-Identifier:/d' | sed 1i'// SPDX-License-Identifier: MIT' > contracts/SDCToken.sol
```

## compile

1. use truffle

```shell
truffle compile
```
2. use remix

<https://remix.ethereum.org/#optimize=true&evmVersion=null&version=soljson-v0.5.10+commit.5a6ea5b1.js&runs=200>
