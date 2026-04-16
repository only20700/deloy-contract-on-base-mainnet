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
