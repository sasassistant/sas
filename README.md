# About SAS

The full name of SAS is Super Smart Application System. It uses Byzantine Fault Tolerance - Deligated Proof of Stake consensus mechanism to build a decentralized application system

SAS is base on [go-ethereum (v1.7.4)](https://github.com/ethereum/go-ethereum), the onsensus algorithm it is a simple version of DPOS-PBFT consensus algorithm.

We also use header.extra to record the all infomation of current block and keep signature of miner. The snapshot keep vote & confirm information of whole chain, which will be update by each Seal or VerifySeal. By the end of each loop, the miner will calculate the next loop miners from the snapshot.

Developers can configure SAS Mainnet on the development tools to create smart contracts.

#### SAS Mainnet
* [mainnet](https://www.sasmainnet.com): `SAS Mainnet URL`
* [networkid](): `40987`
* [browser](http://www.sasscan.com): `SAS blockchain browser`

#### To Support Ethereum Development Tool

SAS support Ethereum development tools, like web3.js, but SAS address it's not prefixed with `0x` like Ethereum, so developer will add prefix `0x` if you use like web3.js

if you have address on SAS it's `0000000000000000000000000000000000000001`, and you want to send a transaction to `0000000000000000000000000000000000000002`, then you can do it like below

```javascript
let rawTransaction = {
    "from": "0x0000000000000000000000000000000000000001",
    "nonce": 1,
    "gasPrice": 40,
    "gasLimit": 121000,
    "to": '0x0000000000000000000000000000000000000002',
    "value": 10,
    "data": ''
}; 
```

#### Other Documents List

* [go-ethereum](https://github.com/ethereum/go-ethereum): `The go-ethereum project `
* [solidity](https://github.com/ethereum/solidity)  : `Solidity, the Contract-Oriented Programming Language`
* [remix](https://github.com/ethereum/remix-ide): `Browser-Only Solidity IDE and Runtime Environment`
* [web.js](https://github.com/ethereum/web3.js): `Ethereum JavaScript API`
* [web3.py](https://github.com/ethereum/web3.py): `A python interface for interacting with the Ethereum blockchain and ecosystem`
* [web3j](https://github.com/ethereum/web3.py): `Lightweight Java and Android library for integration with Ethereum clients`
* [web3.php](https://github.com/sc0Vu/web3.php): `A php interface for interacting with the Ethereum blockchain and ecosystem.`
* [metamask](https://metamask.io/): `MetaMask is an extension for accessing Ethereum enabled distributed applications, or "Dapps" in your normal Chrome browser!`