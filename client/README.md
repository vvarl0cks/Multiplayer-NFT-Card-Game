# Avax Gods - Web3 Multiplayer NFT Card Game   

Create and join live battles, Choose your Battleground, and Battle other players in real-time!   

Avalanche is an open, programmable smart contracts platform for decentralized applications. It allows you to build fast, low-cost, Solidity-compatible dApps, and launch customized blockchain networks via Subnets. Create without limits - Build anything you want, any way you want.   

Avalanche has the tooling and composability you need to speed from concept to launch. Learn more about building on Avalanche with the below developer resources:   
📙Developer Documentation - https://docs.avax.network/   
📙Avalanche-Cli - https://github.com/ava-labs/avalanche-cli   
📙Avalanche Network Runner - https://github.com/ava-labs/avalanche-network-runner   
📙AvalancheJS - https://github.com/ava-labs/avalanchejs   
📙Postman Collection - https://github.com/ava-labs/avalanche-postman-collection   

# Demo ⏩ https://warl0cks-multiplayer-nftcardgame.netlify.app   

<a href="https://github.com/vvarl0cks/Multiplayer-NFT-Card-Game"><img src="https://iili.io/HZCRmqg.png" alt="Web3 Multiplayer NFT Card Game" border="0" /></a>   

<a href="https://github.com/vvarl0cks/Multiplayer-NFT-Card-Game"><img src="https://iili.io/HZCRDLF.png" alt="Web3 Multiplayer NFT Card Game" border="0" /></a>   

<a href="https://github.com/vvarl0cks/Multiplayer-NFT-Card-Game"><img src="https://iili.io/HZCRZzP.jpg" alt="Web3 Multiplayer NFT Card Game" border="0" /></a>   

**Demo URL: https://warl0cks-multiplayer-nftcardgame.netlify.app**   
**Network: Avalanche Fuji Testnet**   

### Tutorial from [JS Mastery Pro](https://www.jsmastery.pro).

## Instructions on setting up the Web3 part of the project
0. `cd backend-web3`
1. `npx hardhat` -> y → typescript → enter → enter
2. `npm install @openzeppelin/contracts dotenv @nomiclabs/hardhat-ethers` + Hardhat packages `npm install --save-dev "hardhat@^2.12.0" "@nomicfoundation/hardhat-toolbox@^2.0.0"`
3. Install [Core](https://chrome.google.com/webstore/detail/core/agoakfejjabomempkjlepdflaleeobhb), a Metamask smart wallet alternative built for Avalanche dApps
  1. Turn on the testnet mode by: opening up the Core extension -> click the hamburger menu on the top left -> go to advanced -> turn on the testnet mode
4. Fund your wallet from the [Avax Faucet](https://faucet.avax.network/)
5. Create a `.env` file and specify a PRIVATE_KEY variable.
6. To get to the private key, do the following steps:
  1. Open up the Core extension -> click the hamburger menu on the top left -> go to security and privacy -> click show recovery phase -> enter your password -> copy the phrase -> go to [wallet.avax.network](https://wallet.avax.network/) -> click access wallet -> choose mnemonic key phrase -> paste what the words we’ve copied from Core -> on the sidebar click manage keys -> view c-chain private key -> copy -> paste it in the .env file
7. Setup `hardhat.config.ts` file from the GitHub gist down in the description
8. Setup `deploy.ts` script from the GitHub gist down in the description
9. Copy the `AvaxGods.sol` smart contract code from above
10. Compile the contract by running the `npx hardhat compile` command
11. Deploy the smart contract on the Fuji test network by running the `npx hardhat run scripts/deploy.ts --network fuji` command
  Move the `/artifacts/contracts/AVAXGods.json` file to the `/contract` folder on the frontend
  Copy the address of the deployed contract from the terminal and paste it into the `/contract/index.js` file of the frontend application   

## Deploy Smart Contract

```bash
gitpod /workspace/Multiplayer-NFT-Card-Game/backend-web3 (main) $ npx hardhat run scripts/deploy.ts --network fuji
Deploying a smart contract...
{ AVAXGods: '0x7183Da1076b96c428D471F165BF5eC7b3312434f' }
```
