## 🙏 Acknowledgements

Special thanks to **Cyfrin**, the **Updraft program**, and **Patrick Collins** for creating such a powerful and practical learning journey for aspiring Web3 developers.

Their clear teaching and real-world examples made it possible for me to complete this smart contract project — even as someone from a non-technical background.

> 🧠 "Learn by building. Grow by shipping." — Updraft by Cyfrin
# 🏦 FundMe Smart Contract

This is a simple Solidity smart contract that allows users to fund the contract with ETH. Only the contract owner can withdraw the funds.

## 🚀 Features

- Accepts ETH from multiple funders
- Uses Chainlink Price Feeds to convert ETH → USD
- Enforces a minimum funding of **$5 USD**
- Allows only the contract owner to withdraw
- Records all funding addresses and their amounts

## 🛠 Tech Stack

- Solidity `^0.8.18`
- Chainlink Price Feeds
- Remix IDE
- Deployed on Remix VM / EVM-compatible networks

## 📦 Files

- `FundMe.sol`: Main contract logic
- `PriceConverter.sol`: Library to convert ETH to USD using Chainlink

## 🔗 Deployed Transaction

- ✅ [Transaction Hash](https://sepolia.etherscan.io/tx/0x1911f8c01f0fc4736e0d4d28c8789fb802b74519869b5261a3e2262c1e1c6aaa)  
(Click to view on Etherscan)

## 📚 How It Works

1. A user sends ETH to the `fund()` function.
2. Contract checks that the USD value (via Chainlink) ≥ $5.
3. Address and amount are recorded in `addressToAmountFunded`.
4. Owner can call `withdraw()` to collect all ETH.
5. If non-owner tries to withdraw → transaction fails.

## ✍️ Author

- Name: **Ng Wei Min (David Ng)**
- LinkedIn: [linkedin.com/in/davidng-web3](https://www.linkedin.com/in/davidng-web3)
- GitHub: [github.com/DavidNg-DAO](https://github.com/DavidNg-DAO)

## 📜 License

MIT
