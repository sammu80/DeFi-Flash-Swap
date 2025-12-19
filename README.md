# ⚡ DeFi Flash Swap Arbitrage

A smart contract-based arbitrage bot that uses **Uniswap V2 Flash Swaps** to exploit price differences between decentralized exchanges.

## 🚀 How it Works
1. **Borrow:** The contract borrows tokens (e.g., 1000 USDC) from Uniswap via Flash Swap.
2. **Swap:** It buys an asset (e.g., ETH) on **Sushiswap** where the price is lower.
3. **Sell:** It sells the same asset on **Uniswap** where the price is higher.
4. **Repay:** It repays the borrowed amount + fee to Uniswap.
5. **Profit:** The remaining difference is kept as profit in the contract.

## 🛠️ Tech Stack
- **Solidity** (Smart Contracts)
- **Hardhat** (Testing with Mainnet Forking)
- **Ethers.js** (Interacting with Dex Routers)
- **DEXs:** Uniswap V2, Sushiswap

## ⚠️ Disclaimer
This is for educational purposes. Arbitrage in real markets requires high-speed bots (MEV) to compete with other traders.

## 🔧 Installation
1. `npm install`
2. Configure your Alchemy/Infura mainnet URL in `hardhat.config.js`.
3. Run tests on a local fork: `npx hardhat test`# DeFi-Flash-Swap
