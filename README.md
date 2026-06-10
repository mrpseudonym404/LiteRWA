
**Explorer:**
[https://liteforge.explorer.caldera.xyz](https://liteforge.explorer.caldera.xyz)

**Contract Functions:**

| Function | Description |
|----------|-------------|
| `createAsset(name, assetType, valueUSD, ipfsHash)` | Mint a new RWA token. Returns token ID. |
| `listAsset(id, price)` | List an owned asset for sale. |
| `buyAsset(id)` | Purchase a listed asset (payable in zkLTC). |
| `delistAsset(id)` | Remove an asset from marketplace. |
| `transferAsset(id, to)` | Transfer asset to another wallet. |
| `getUserAssets(user)` | View all assets owned by a specific address. |
| `totalAssets()` | Get total number of assets minted. |
| `assets(id)` | Get details of a specific asset by ID. |
| `creator()` | Get the contract creator address. |

## Technology Stack

| Category | Technology |
|----------|------------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Web3 Library | Ethers.js v6 |
| Blockchain | LitVM Testnet (Chain ID: 4441) |
| Oracle | CoinGecko API (live price feeds) |
| Hosting | Vercel |
| Version Control | Git + GitHub |
| Wallet Support | MetaMask, Rabby Wallet, any EVM-compatible wallet |

## Getting Started

### Prerequisites

- A Web3 browser extension (MetaMask or Rabby Wallet recommended)
- Internet connection
- Modern web browser (Chrome, Firefox, Edge, or Safari)

### Initial Setup

1. **Connect Wallet**
   - Click the "Connect Wallet" button
   - Approve the addition of LitVM testnet (Chain ID: 4441)
   - Authorize wallet connection

2. **Get Testnet Gas**
   - Visit [https://testnet.litvm.com](https://testnet.litvm.com)
   - Paste your wallet address
   - Request free zkLTC tokens (0.2 zkLTC per request)

## How to Use

### Step 1: Connect Wallet

Click the "Connect Wallet" button in the top-right corner. Your Web3 wallet will prompt you to approve the LitVM network (Chain ID: 4441). Once connected, your wallet address, zkLTC balance, and current points will be displayed.

### Step 2: Mint an Asset

Navigate to the "Mint New RWA" section:

1. Enter an asset name (e.g., "1kg Gold Bar")
2. Select a category: Gold, Silver, Oil, or Real Estate
3. Set a USD valuation (minimum $1)
4. (Optional) Provide an IPFS hash for metadata
5. Click "Mint Asset (+10 pts)"

Example valuations for reference:

| Category | Example Name | Suggested Valuation (USD) |
|----------|--------------|---------------------------|
| Gold | 1kg Gold Bar | 2500 |
| Silver | 500g Silver Bar | 450 |
| Oil | WTI Crude Barrel | 72 |
| Real Estate | Apartment Unit 5B | 250000 |

### Step 3: List an Asset for Sale

1. Go to the "My Assets" tab
2. Locate the asset you want to sell
3. Click the "List" button
4. Enter a price in zkLTC (minimum 0.01)
5. Confirm the transaction in your wallet

The asset will now appear in the marketplace and in your "My Listings" tab.

### Step 4: Browse and Buy from Marketplace

1. Navigate to the "Marketplace" section
2. Use search to find assets by name or token ID
3. Apply category filters (Gold, Silver, Oil, Real Estate)
4. Sort by price or asset ID as needed
5. Click "Buy" on any listed asset
6. Confirm the purchase in your wallet

### Step 5: Transfer an Asset

1. Go to the "My Assets" tab
2. Locate the asset you wish to transfer
3. Click the "Transfer" button
4. Enter the recipient's wallet address
5. Confirm the transfer transaction

### Step 6: Earn Points and Badges

Every action contributes to your gamification progress:

| Action | Points Earned |
|--------|---------------|
| Mint Asset | +10 |
| List Asset | +5 |
| Buy Asset | +20 |
| Daily Check-in | +5 to +100 (based on streak) |
| Complete All Actions | +30 bonus |

### Step 7: Daily Check-in

Click the "Check In" button in the check-in banner to earn daily points. Your streak increases with consecutive check-ins:

- Days 1-2: +5 points
- Days 3-6: +10 points
- Days 7-29: +25 points
- Day 30 and beyond: +100 points

## Points & Badges System

### Point Accumulation

Points are automatically awarded on-chain after each successful transaction:

- **Mint Asset**: +10 points per mint
- **List Asset**: +5 points per listing
- **Buy Asset**: +20 points per purchase
- **Daily Check-in**: Progressive rewards based on streak length
- **Challenge Bonus**: +30 points after completing all three actions (mint, list, buy)

### Badge Progression

| Badge | Points Required | Visual Indicator |
|-------|----------------|------------------|
| Starter | 0 | White circle |
| Bronze | 30 | Bronze medal |
| Silver | 75 | Silver medal |
| Gold | 150 | Gold medal |
| Platinum | 300 | Platinum medal |
| Diamond | 500 | Diamond icon |

### Rank System

Users are ranked from 1 to 200 based on total points. Lower rank numbers indicate higher standing:

- Rank 1: Highest points (500+)
- Rank 200: Minimum points (0)

## Marketplace Functionality

### Search Features

- **By Name**: Partial or full asset name matching
- **By Token ID**: Enter "#" followed by ID number (e.g., "#20")

### Filter Options

- All (default)
- Gold
- Silver
- Oil
- Real Estate

### Sort Options

- Price: Low to High
- Price: High to Low
- Asset ID: Ascending

### Display Information

Each marketplace listing shows:
- Asset name
- Category badge
- Token ID
- Price in zkLTC
- Approximate USD value
- Buy button (or "Your asset" label if owned)

## Price Feeds

LiteRWA integrates real-time price data from the CoinGecko API:

| Asset | Update Frequency | Display Location |
|-------|------------------|------------------|
| Litecoin (LTC) | Every 60 seconds | Top price bar |
| Gold | Every 60 seconds | Top price bar |
| Silver | Every 60 seconds | Top price bar |
| Oil | Every 60 seconds | Top price bar |
| Bitcoin (BTC) | Every 60 seconds | Top price bar |

All marketplace prices automatically convert to USD using the current LTC price from the feed.

## Network Information

**LitVM Testnet Details:**

| Parameter | Value |
|-----------|-------|
| Network Name | LitVM Testnet |
| RPC URL | https://liteforge.rpc.caldera.xyz/http |
| Chain ID | 4441 |
| Currency Symbol | zkLTC |
| Block Explorer | https://liteforge.explorer.caldera.xyz |

## Local Development

### Clone the Repository

```bash
git clone https://github.com/mrpseudonym404/LiteRWA.git
cd LiteRWA
