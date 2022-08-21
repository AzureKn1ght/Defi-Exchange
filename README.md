# Build a Decentralized Exchange like Uniswap

Scenario: Now its time for you to launch a DeFi Exchange for your `Crypto Dev` tokens

![](https://i.imgur.com/nvLT06K.png)

![](https://i.imgur.com/uWJAYcZ.png)

---

## Requirements

- Build an exhange with only one asset pair (ETH / Crypto Dev)
- Your Decentralized Exchange should take fees of `1%` on swaps
- When user adds liquidity, they should be given `Crypto Dev LP` tokens (Liquidity Provider tokens)
- CDLP tokens should be given propotional to the `Ether` a user is willing to add to the liquidity

---

## Prerequisites

- Must have completed the [ICO tutorial](https://github.com/AzureKn1ght/ICO)

---

## BUILD IT

### Smart Contract

To build the smart contract we would be using [Hardhat](https://hardhat.org/).
Hardhat is an Ethereum development environment and framework designed for full stack development in Solidity. In simple words you can write your smart contract, deploy them, run tests, and debug your code.

- This project uses `@openzeppelin/contracts` as we would be importing [Openzeppelin's ERC20 Contract](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol) in our `Exchange` contract

- We would also install `dotenv` package to be able to import the env file and use it in our config. Thereby protecting our private keys and API keys, so as not to hardcode them and leak them on the Internet. Create a `.env` file in the `hardhat` folder and add the following lines, use the instructions in the comments to get your Alchemy API Key URL and Goerli Private Key. Make sure that the account from which you get your Goerli private key is funded with Goerli Test Ether.

 
  ```js
  // Go to https://www.alchemyapi.io, sign up, create
  // a new App in its dashboard and select the network as Rinkeby, and replace "add-the-alchemy-key-url-here" with its key url
  ALCHEMY_API_KEY_URL="add-the-alchemy-key-url-here"

  // Replace this private key with your GOERLI account private key
  // To export your private key from Metamask, open Metamask and
  // go to Account Details > Export Private Key
  // NEVER put real ETH into testing accounts
  GOERLI_PRIVATE_KEY="add-the-goerli-private-key-here"
  ```

### Website

- To develop the website we would be using [React](https://reactjs.org/) and [Next Js](https://nextjs.org/). 

- We will also use the [Web3Modal library](https://github.com/Web3Modal/web3modal). 
Web3Modal is an easy-to-use library to help developers add support for multiple providers in their apps with a simple customizable configuration. By default Web3Modal Library supports injected providers like (Metamask, Dapper, Gnosis Safe, Frame, Web3 Browsers, etc), You can also easily configure the library to support Portis, Fortmatic, Squarelink, Torus, Authereum, D'CENT Wallet and Arkane.

### Technologies Used 
- [Hardhat](https://hardhat.org/)
- [Solidity](https://soliditylang.org/)
- [Ethers.js](https://github.com/ethers-io/ethers.js/)
- [React](https://reactjs.org/)
- [Next.js](https://nextjs.org/)

---

## DEPLOY 🚀

We have deployed the dApp, so that everyone can see the website and we can share it with the world.

### Smart Contract 
https://goerli.etherscan.io/address/0x2eda149048dF83547DF2b53D4c73eeb933f2b0eF

### Dapp Frontend
https://defi-exchange-azurekn1ght.vercel.app/

