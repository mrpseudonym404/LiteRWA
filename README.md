# ✦ LiteRWA

**Tokenize and trade real-world assets on LitVM testnet.**

Live demo: [https://literwa.vercel.app](https://literwa.vercel.app)

---

## What is this?

LiteRWA is a simple marketplace where you can mint, list, buy, and transfer tokenized assets like Gold, Silver, Oil, and Real Estate. All transactions happen on LitVM testnet (Litecoin's ZK-rollup).

Built to learn dApp development and explore RWA (Real-World Assets) on blockchain.

---

## Features

- **Mint** — Turn any asset into a token
- **List** — Sell your tokens for zkLTC (min 0.01)
- **Buy** — Purchase tokens from other users
- **Transfer** — Send tokens to any wallet
- **Points + Badges** — Mint = 10, List = 5, Buy = 20
- **Daily Check-in** — Streak rewards
- **Activity log** — Every transaction saved locally
- **Explorer links** — Click "View" to see tx on-chain

---

## How to use

### 1. Connect wallet
Click "Connect Wallet" → approve LitVM network (Chain ID: 4441)  
Then grab free zkLTC from [faucet](https://testnet.litvm.com)

### 2. Mint an asset
Pick a category, give it a name, set a USD value (min 1), click "Mint Asset".

| Category | Example Name | Valuation |
|----------|--------------|-----------|
| Gold | "1kg Gold Bar" | 2500 |
| Silver | "500g Silver Bar" | 450 |
| Oil | "WTI Crude Barrel" | 72 |
| Real Estate | "Apartment 5B" | 250000 |

### 3. List for sale
Go to "My Assets" → click "List" → set price in zkLTC (min 0.01)

### 4. Buy from marketplace
Browse "Marketplace", use search or filters, click "Buy"

### 5. Earn points & badges
Every action gives points. Reach:
- 30 points → Bronze
- 75 points → Silver
- 150 points → Gold
- 300 points → Platinum
- 500 points → Diamond

---

## Tech stack

- **Frontend**: HTML, CSS, JavaScript (no frameworks)
- **Web3**: Ethers.js v6
- **Blockchain**: LitVM testnet (Chain ID 4441)
- **Oracle**: CoinGecko API (price display only)
- **Hosting**: Vercel

---

## Contract

Deployed on LitVM testnet at:  
`0xeA1Dc56f30d3DFFaeA65F6a0cd5ff35A7Fb67e3A`

Explorer: [https://liteforge.explorer.caldera.xyz](https://liteforge.explorer.caldera.xyz)

---

## Run locally

```bash
git clone https://github.com/mrpseudonym404/LiteRWA.git
cd LiteRWA
python3 -m http.server 3000
# then open http://localhost:3000
