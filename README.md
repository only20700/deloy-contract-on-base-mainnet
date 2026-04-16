# deloy-contract-on-base-mainnet
feat(deployment): deploy and verify staking contract on Base mainnet
- deploy contract using Hardhat with optimized gas settings
- verify source code on BaseScan for transparency
- initialize contract with production parameters
- integrate deployed address into frontend config
- add reusable deployment script for future upgrades
- validate staking, reward distribution, and withdrawal flows

Notes:
- ensure correct RPC endpoint for Base
- double-check private key security before deployment

Staking Contract
feat(staking): deploy staking contract on Base mainnet
- implement staking logic for ERC20 token
- add reward distribution mechanism (fixed APY)
- configure staking duration and lock period
- deploy contract using Hardhat
- verify contract on BaseScan
- set reward token and staking token addresses
- initialize contract parameters (APY, duration, pool limit)
- test stake, unstake, and claim reward flows
- integrate contract address into frontend

# 🚀 Smart Contract Deployment on Base

This repository contains smart contracts and deployment scripts for deploying on the Base network.

## 📦 Tech Stack

- Solidity
- Hardhat
- Ethers.js
- OpenZeppelin

---

## 🌐 Supported Network

- Base Mainnet
- Base Sepolia (Testnet)

---

## ⚙️ Setup

### 1. Clone repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo

npm install

cp .env.example .env

PRIVATE_KEY=your_wallet_private_key
BASE_RPC_URL=https://mainnet.base.org
BASESCAN_API_KEY=your_basescan_api_key

npx hardhat compile

npx hardhat run scripts/deploy.js --network base

npx hardhat run scripts/deploy.js --network baseSepolia

npx hardhat verify --network base <CONTRACT_ADDRESS> <constructor_args>

npx hardhat verify --network base 0xYourContractAddress "MyToken" "MTK"
