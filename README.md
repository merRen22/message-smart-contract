### Inbox Smart Contract

Smart contract with NodeJs. This project is a test on how to build a simple smart contract for storing a string and reading it. The contract is deployed to rinkeby testnet. Can be found [here](https://rinkeby.etherscan.io/address/0xe6eF96f0318b38Ef6a2Ce212EAD0ef4266931427)

## Configuration

    .
    โโโ README.md               # You are here ๐
    โโโ compile.js              # Compiler fo code ๐ฆ
    โโโ contracts               # All smart contracts ( solidity )
    โย ย  โโโ inbox.sol           # Contract to interact with inbox
    โโโ deploy.js               # Take compile code and deploy to network ๐
    โโโ package.json            # Scripts & dependencies ๐
    โโโ test                    # Test for the contracts
        โโโ inbox.test.js       # Mocha test ๐งช

## Test

The basic flow consist on the compiler taking the contract source code and genereting the bytecode and an ABI ( interface ). The bytecode will be deploy on a local test network using Ganache and the ABI will be feed to Web3 so we have programmatinc access.

To run the test use this command ๐

`npm run test`

## Deploy

To compile and deploy the contract create a `.env` file and fill the url of the api in Infura and your mnemonic from your wallet. Finally use this command ๐

`node deploy.js`
