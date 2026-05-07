# Awesome Crypto MCPs [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**A curated list of the best Crypto, Blockchain & Web3 Model Context Protocol (MCP) servers — connect AI agents like Claude, Cursor, ChatGPT, and Claude Code to on-chain data, DEX trades, wallets, DeFi, NFTs, and trading.**

> Awesome PRs Welcome — see [Contributing](#-contributing).

---

## ⭐ Featured: Bitquery MCP

> **The fastest way to give your AI agent production-grade blockchain trading data.**

[![Bitquery MCP](https://img.shields.io/badge/MCP-mcp.bitquery.io-blue?style=for-the-badge)](https://mcp.bitquery.io/)
[![Chains](https://img.shields.io/badge/Chains-8-green?style=for-the-badge)](https://docs.bitquery.io/docs/mcp/mcp-server/)
[![Auth](https://img.shields.io/badge/Auth-OAuth%202.1-orange?style=for-the-badge)](https://docs.bitquery.io/docs/mcp/mcp-server/)

**[Bitquery MCP Server](https://mcp.bitquery.io/)** connects your AI client to Bitquery's production trading dataset — the same data behind Bitquery's GraphQL APIs, Kafka streams, and TradingView feeds. Ask in plain English; get clean, structured rows back. **No SQL, no schema, no rate-limit juggling.**

| Feature | Details |
| --- | --- |
| **Endpoint** | [`https://mcp.bitquery.io`](https://mcp.bitquery.io/) |
| **Chains** | Solana, Ethereum, BSC, Base, Arbitrum, Optimism, Polygon, Tron |
| **Data** | Billions of swap-level trades, OHLC candles (1m / 5m / 1h / 1d), market cap, FDV, circulating supply |
| **Auth** | OAuth 2.1 (browser sign-in) — token-in-URL fallback for autonomous agents |
| **Pricing** | Free tier with a [Bitquery account](https://account.bitquery.io/); metered above |
| **Clients** | Claude Desktop, Claude Code, Cursor, ChatGPT, VS Code, any MCP client |
| **Mode** | Read-only · outlier-filtered · near real-time |

### What you can ask it

- *"Top 10 Solana tokens by USD volume in the last 24h, skip wash-traded pools."*
- *"Pull every trade for wallet `7xKX…` in the last 7 days. Compute realised PnL per token."*
- *"1-minute OHLC for the WIF/USDC pool on Raydium for the last 6 hours."*
- *"Which Base tokens crossed $10M market cap in the last 24h?"*
- *"How many new tokens launched on Pump.fun in the last hour vs the 24h average?"*
- *"For each chain, show 24h DEX volume, trades, and unique traders."*

### Install in 60 seconds

**Cursor** → Settings → MCP → Add new MCP server → URL: `https://mcp.bitquery.io`

**Claude Desktop / ChatGPT** → Settings → Connectors → Add custom connector → URL: `https://mcp.bitquery.io`

**Claude Code (terminal):**

```bash
claude mcp add bitquery -- npx -y mcp-remote https://mcp.bitquery.io/mcp
```

**Cursor `.cursor/mcp.json`:**

```json
{
  "mcpServers": {
    "bitquery": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://mcp.bitquery.io/mcp"]
    }
  }
}
```

**Docs:** [docs.bitquery.io/docs/mcp/mcp-server](https://docs.bitquery.io/docs/mcp/mcp-server/) · **Use cases:** [trading examples](https://docs.bitquery.io/docs/mcp/trading/examples/) · **Support:** [Telegram](https://t.me/Bloxy_info)

---

## 📖 About

**Awesome Crypto MCPs** is a comprehensive, curated directory of the best **Model Context Protocol (MCP) servers** for cryptocurrency, blockchain, DeFi, NFTs, and Web3. This repository is the definitive resource for developers, traders, and AI agent builders who want to connect LLMs (Claude, ChatGPT, Cursor, Claude Code, Codex, Windsurf, VS Code Copilot, Cline, and others) to live on-chain data and execution.

Whether you are building **AI trading agents**, **on-chain copilots**, **DeFi research assistants**, **wallet analytics tools**, **NFT trading bots**, **MEV systems**, or **crypto research workflows**, this list covers the entire MCP ecosystem — including blockchain data MCPs, DEX MCPs, CEX trading MCPs, wallet MCPs, NFT MCPs, oracle MCPs, bridge MCPs, security MCPs, and more.

### What is MCP?

[Model Context Protocol (MCP)](https://modelcontextprotocol.io/) is an open standard introduced by Anthropic that lets AI models connect to external tools, APIs, and data sources in a standardised way. For crypto and Web3, MCP turns any LLM into an on-chain-aware agent — one that can read live blockchain data, place trades, transfer assets, query DeFi protocols, and analyse markets through plain-English conversations.

### Key Features of this list

- ⭐ **Featured Top Pick**: Bitquery MCP for production-grade DEX trading data across 8 chains
- 🌐 **Multi-Chain & Universal MCPs**: Aggregators that span EVM, Solana, Bitcoin, and beyond
- 🔌 **Infrastructure / RPC MCPs**: Alchemy, QuickNode, Chainstack, Tatum, Nodit, Moralis, thirdweb
- 💱 **DEX & Trading MCPs**: Uniswap, Jupiter, PancakeSwap, Raydium, Aster, Hyperliquid, dYdX-style
- 🏦 **DeFi & Lending MCPs**: Aave, Euler, Lista, DefiLlama, Arcadia, Philidor, Morpho integrations
- 📊 **Market Data MCPs**: CoinGecko, CoinMarketCap, DexScreener, DexPaprika, Pyth, Chainlink, technical indicators
- 🐳 **On-Chain Analytics MCPs**: Whale tracking, wallet inspection, ENS, Tornado Cash, validators
- 🔒 **Security & Risk MCPs**: Honeypot detection, rug-check, token-allowance revoke, vault risk scoring
- 🖼️ **NFT MCPs**: OpenSea, Magic Eden, NFT analytics
- 🌉 **Cross-Chain & Bridge MCPs**: deBridge, Stargate, Wormhole, bridge rates
- 📰 **News & Sentiment MCPs**: CryptoPanic, Cointelegraph, BlockBeats, sentiment, exchange announcements
- 💸 **Payment MCPs**: Lightning Network, Bitcoin Lightning, USDC on Base, x402
- 🤖 **CEX Trading MCPs**: Binance, Bybit, OKX, Coinbase Base
- 🛠️ **Developer MCPs**: Contract scrapers, token minters, EVM tooling, Solana dev kits

---

## 📑 Table of Contents

- [⭐ Featured: Bitquery MCP](#-featured-bitquery-mcp)
- [📖 About](#-about)
- [🌐 Universal & Multi-Chain MCPs](#-universal--multi-chain-mcps)
- [🔌 Blockchain Infrastructure & RPC MCPs](#-blockchain-infrastructure--rpc-mcps)
- [📊 Blockchain Data & Indexing MCPs](#-blockchain-data--indexing-mcps)
- [⛓️ Ethereum & EVM MCPs](#-ethereum--evm-mcps)
- [🟣 Solana MCPs](#-solana-mcps)
- [🟠 Bitcoin & Lightning MCPs](#-bitcoin--lightning-mcps)
- [🔵 Base, BNB, TON, Sui, Tron & Other Chain MCPs](#-base-bnb-ton-sui-tron--other-chain-mcps)
- [💱 DEX & On-Chain Trading MCPs](#-dex--on-chain-trading-mcps)
- [🏛️ Centralized Exchange (CEX) MCPs](#-centralized-exchange-cex-mcps)
- [🏦 DeFi, Lending & Yield MCPs](#-defi-lending--yield-mcps)
- [💲 Price Feeds & Oracle MCPs](#-price-feeds--oracle-mcps)
- [📈 Market Data & Analytics MCPs](#-market-data--analytics-mcps)
- [🐳 Whale & On-Chain Activity MCPs](#-whale--on-chain-activity-mcps)
- [👛 Wallet & Portfolio MCPs](#-wallet--portfolio-mcps)
- [🔒 Security, Risk & Compliance MCPs](#-security-risk--compliance-mcps)
- [🌉 Cross-Chain & Bridge MCPs](#-cross-chain--bridge-mcps)
- [🖼️ NFT MCPs](#-nft-mcps)
- [📰 News, Sentiment & Information MCPs](#-news-sentiment--information-mcps)
- [💸 Crypto Payments MCPs](#-crypto-payments-mcps)
- [🚀 Memecoins & Launchpad MCPs](#-memecoins--launchpad-mcps)
- [🗳️ DAO & Governance MCPs](#-dao--governance-mcps)
- [🛠️ Developer Tools & Utility MCPs](#-developer-tools--utility-mcps)
- [📚 Resources](#-resources)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🔍 Related Searches](#-related-searches)
- [📈 Popular Use Cases](#-popular-use-cases)

> **Legend** — 🟢 Live · 🟡 Beta / Preview · ⭐ Featured · ☁️ Remote (hosted) · 💻 Self-host

---

## 🌐 Universal & Multi-Chain MCPs

The all-in-one crypto MCP servers — designed to give an AI agent a unified surface across many blockchains, protocols, and data sources.

| MCP | Coverage | Type | Hosting | Status | Link |
| --- | --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | Solana, Ethereum, BSC, Base, Arbitrum, Optimism, Polygon, Tron | DEX trades, OHLC, market cap, wallet PnL | ☁️ Remote | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **Hive Intelligence** | Multi-chain | Unified crypto / DeFi / Web3 analytics | ☁️ Remote | 🟢 Live | [hiveintelligence.xyz/crypto-mcp](https://hiveintelligence.xyz/crypto-mcp) · [GitHub](https://github.com/hive-intel/hive-crypto-mcp) |
| **Heurist Mesh** | Multi-chain | Network of specialised Web3 AI agents | 💻 / ☁️ | 🟢 Live | [heurist-mesh-mcp-server](https://github.com/heurist-network/heurist-mesh-mcp-server) |
| **Web3 MCP (Strangelove)** | Solana, Ethereum, Cardano, THORChain, XRP, Bitcoin, TON | Multi-chain balances & actions | 💻 | 🟢 Live | [strangelove-ventures/web3-mcp](https://github.com/strangelove-ventures/web3-mcp) |
| **Universal Crypto MCP** | 20+ chains (EVM + Solana) | 380+ tools, swaps, bridges, x402 payments | 💻 | 🟢 Live | [nirholas/universal-crypto-mcp](https://github.com/nirholas/universal-crypto-mcp) |
| **All-in-One Crypto Trading MCP** | 8 chains, 5 CEXs | Trading, analytics, whale monitoring | 💻 | 🟢 Live | [allinonecryptomcp.dev](https://allinonecryptomcp.dev/) |
| **GOAT** | Ethereum, Solana, Base + more | 200+ on-chain actions, "one MCP for all chains" | 💻 | 🟢 Live | [goat-sdk/goat](https://github.com/goat-sdk/goat/tree/main/typescript/examples/by-framework/model-context-protocol) |
| **Bankless Onchain** | EVM | ERC-20, transactions, contract state | 💻 | 🟢 Live | [bankless/onchain-mcp](https://github.com/bankless/onchain-mcp) |
| **WAIaaS** | EVM + Solana | Self-hosted wallet daemon, 59+ tools, policy engine | 💻 | 🟢 Live | [minhoyoo-iotrust/WAIaaS](https://github.com/minhoyoo-iotrust/WAIaaS) |

---

## 🔌 Blockchain Infrastructure & RPC MCPs

MCPs from the major node, RPC, and blockchain-data infrastructure providers — the backbone for any production AI agent.

| MCP | Provider | Capabilities | Hosting | Status | Link |
| --- | --- | --- | --- | --- | --- |
| **Alchemy MCP** | Alchemy | 159 tools — token prices, NFT metadata, tx history, contract sim, 100+ chains | ☁️ / 💻 | 🟢 Live | [alchemy.com/docs/alchemy-mcp-server](https://www.alchemy.com/docs/alchemy-mcp-server) · [GitHub](https://github.com/alchemyplatform/alchemy-mcp) |
| **Chainstack MCP** | Chainstack | Deploy nodes, search docs, manage infra, 70+ chains | ☁️ Remote | 🟢 Live | [docs.chainstack.com/docs/chainstack-mcp-server](https://docs.chainstack.com/docs/chainstack-mcp-server) |
| **QuickNode MCP** | QuickNode | Configure endpoints, monitor usage & billing | 💻 | 🟢 Live | [quiknode-labs/qn-mcp](https://github.com/quiknode-labs/qn-mcp) |
| **Tatum MCP** | Tatum | 130+ networks via Tatum Blockchain Data API & RPC Gateway | 💻 | 🟢 Live | [tatumio/blockchain-mcp](https://github.com/tatumio/blockchain-mcp) |
| **Nodit MCP** | Nodit Labs | Multi-chain blockchain data via Web3 APIs | 💻 | 🟢 Live | [noditlabs/nodit-mcp-server](https://github.com/noditlabs/nodit-mcp-server) |
| **Moralis MCP** | Moralis | Wallet activity, token metrics, dapp usage on Moralis REST API | 💻 | 🟢 Live | [moralisweb3/moralis-mcp-server](https://github.com/moralisweb3/moralis-mcp-server) |
| **thirdweb AI** | thirdweb | Insight, Engine, Storage, Nebula natural-language onchain | 💻 | 🟢 Live | [thirdweb-dev/ai](https://github.com/thirdweb-dev/ai) |
| **Blockscout MCP** | Blockscout | Wraps Blockscout APIs for balances, tokens, NFTs | 💻 | 🟢 Live | [blockscout/mcp-server](https://github.com/blockscout/mcp-server) |

---

## 📊 Blockchain Data & Indexing MCPs

The "data warehouse" layer for AI agents — query indexed blockchain data at scale.

| MCP | Source | Capabilities | Hosting | Status | Link |
| --- | --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | Bitquery | Trades, OHLC, market cap across 8 chains; outlier-filtered | ☁️ Remote | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **Dune Analytics MCP** | Dune | SQL on indexed chains, dashboards, visualisations | ☁️ Remote | 🟢 Live | [docs.dune.com/api-reference/agents/mcp](https://docs.dune.com/api-reference/agents/mcp) |
| **The Graph MCP** | The Graph | Search subgraphs, GraphQL queries on indexed data | 💻 | 🟢 Live | [Data-Nexus-Web3/thegraph-mcp](https://github.com/Data-Nexus-Web3/thegraph-mcp) |
| **The Graph Token API MCP** | The Graph | Token metadata, balances, transfers, holders | 💻 | 🟢 Live | [thegraph.com/docs/ai-suite/token-api-mcp](https://thegraph.com/docs/ar/ai-suite/token-api-mcp/introduction/) |
| **Spice (Nimbus)** | Flipside | Solana metadata catalog & blockchain queries | 💻 | 🟢 Live | [getnimbus/spice](https://github.com/getnimbus/spice) |
| **Dappier** | Dappier | Real-time, rights-cleared crypto + finance data | 💻 | 🟢 Live | [DappierAI/dappier-mcp](https://github.com/DappierAI/dappier-mcp) |

---

## ⛓️ Ethereum & EVM MCPs

For Ethereum mainnet and the EVM ecosystem (Polygon, BSC, Arbitrum, Optimism, Base, Avalanche, Linea, etc.).

| MCP | Type | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | Ethereum + EVM (BSC, Base, Arbitrum, Optimism, Polygon) | Per-trade DEX rows, OHLC, market cap, wallet PnL, outlier-filtered | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **EVM MCP Server** | Multi-EVM | 30+ EVM networks: native tokens, ERC-20, NFTs, contracts, ENS | 🟢 Live | [mcpdotdirect/evm-mcp-server](https://github.com/mcpdotdirect/evm-mcp-server) |
| **Etherscan MCP** | Block explorer | Token balances, ENS, contracts via Etherscan API | 🟢 Live | [crazyrabbitLTC/mcp-etherscan-server](https://github.com/crazyrabbitLTC/mcp-etherscan-server) |
| **Ethereum MCP** | Single-chain | ETH balances, prices, tx details | 🟢 Live | [qingfengzxr/eth-mcp-server](https://github.com/qingfengzxr/eth-mcp-server) |
| **Web3 MCP (tumf)** | EVM | Generic Web3 / EVM interactions | 🟢 Live | [tumf/web3-mcp](https://github.com/tumf/web3-mcp) |
| **Web3 Assistant** | EVM | ABI analysis & secure contract method invocation | 🟢 Live | [EmanuelJr/web3-mcp-server](https://github.com/EmanuelJr/web3-mcp-server) |
| **Ethereum Validators Queue** | Ethereum staking | Validator activation & exit queues in real time | 🟢 Live | [kukapay/ethereum-validators-queue-mcp](https://github.com/kukapay/ethereum-validators-queue-mcp) |
| **ENS MCP** | ENS | Resolve & analyse ENS domain activity | 🟢 Live | [kukapay/ens-mcp](https://github.com/kukapay/ens-mcp) |
| **Contract Scraper MCP** | Multi-chain | Scrape verified contract source code & ABIs | 🟢 Live | [kukapay/contract-scraper-mcp](https://github.com/kukapay/contract-scraper-mcp) |
| **Find Block MCP** | EVM | Resolve block numbers from timestamps | 🟢 Live | [kukapay/findblock-mcp](https://github.com/kukapay/findblock-mcp) |

---

## 🟣 Solana MCPs

Comprehensive coverage of the Solana ecosystem — wallets, swaps, memecoins, validators, dev tooling.

| MCP | Type | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | Solana data | Pump.fun / Raydium / Jupiter trades, OHLC, market cap, wallet PnL, outlier-filtered | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **Solana Agent Kit MCP** | All-in-one | 40+ Solana actions, full SendAI Agent Kit | 🟢 Live | [sendaifun/solana-agent-kit](https://github.com/sendaifun/solana-agent-kit/tree/main/examples/agent-kit-mcp-server) |
| **Aldrin Labs Solana MCP** | RPC | 21 Solana RPC methods — accounts, tokens, staking | 🟢 Live | [Aldrin-labs/solana-mcp-server](https://github.com/Aldrin-labs/solana-mcp-server) |
| **Solana Dev MCP** | Dev tools | Solana Foundation MCP for development | 🟢 Live | [solana-foundation/solana-dev-mcp](https://github.com/solana-foundation/solana-dev-mcp) |
| **Jupiter MCP** | DEX aggregator | Token swaps via Jupiter Ultra API | 🟢 Live | [kukapay/jupiter-mcp](https://github.com/kukapay/jupiter-mcp) |
| **Solana Limit Order MCP** | Trading | Limit buy/sell orders via Jupiter | 🟢 Live | [dimitrov-d/solana-limit-order-mcp](https://github.com/dimitrov-d/solana-limit-order-mcp) |
| **Raydium LaunchLab MCP** | Launchpad | Launch / buy / sell tokens on Raydium LaunchLab | 🟢 Live | [kukapay/raydium-launchlab-mcp](https://github.com/kukapay/raydium-launchlab-mcp) |
| **PumpSwap MCP** | DEX | Automated trading on PumpSwap | 🟢 Live | [kukapay/pumpswap-mcp](https://github.com/kukapay/pumpswap-mcp) |
| **PumpFun Wallets MCP** | Analytics | Analyse wallets on Pump.fun and PumpSwap | 🟢 Live | [kukapay/pumpfun-wallets-mcp](https://github.com/kukapay/pumpfun-wallets-mcp) |
| **Memecoin Observatory** | Analytics | Memecoin radar, social signals, whale tracking | 🟢 Live | [tony-42069/solana-mcp](https://github.com/tony-42069/solana-mcp) |
| **Memecoin Radar MCP** | Analytics | Solana memecoin & Pump.fun launch radar | 🟢 Live | [kukapay/memecoin-radar-mcp](https://github.com/kukapay/memecoin-radar-mcp) |
| **Solana Launchpads MCP** | Analytics | Daily activity across Solana launchpads | 🟢 Live | [kukapay/solana-launchpads-mcp](https://github.com/kukapay/solana-launchpads-mcp) |
| **MCP Meme Deployer** | Token deploy | Deploy tradable Solana tokens at zero cost | 🟢 Live | [kirabuilds/mcp-meme-deployer](https://github.com/kirabuilds/mcp-meme-deployer) |
| **Hubble MCP** | Analytics | Pump.fun & DEX visualisation in natural language | 🟢 Live | [HubbleVision/hubble-ai-mcp](https://github.com/HubbleVision/hubble-ai-mcp) |
| **Solana DeFi Analytics MCP** | Analytics | Wallet behaviour & DeFi-strategy insights | 🟢 Live | [kirtiraj22/solana-mcp](https://github.com/kirtiraj22/solana-mcp) |
| **Quant72 MCP** | Trading | On-chain quantitative trading + Solana Agent Kit | 🟢 Live | [Quant72AI/quant72-mcp](https://github.com/Quant72AI/quant72-mcp) |
| **AMOCA MCP** | Wallet | Solana wallet analysis, balances, history | 🟢 Live | [manolaz/amoca-solana-mcp-server](https://github.com/manolaz/amoca-solana-mcp-server) |
| **SolMCP** | Multi-tool | Helius + DexScreener + Pyth integrations | 🟢 Live | [N-45div/SolMCP](https://github.com/N-45div/SolMCP---SendAI-MCP-competition) |
| **Solana Forum Summarizer** | Research | Browse and summarise Solana Forum content | 🟢 Live | [dimitrov-d/solana-forum-summarizer-mcp](https://github.com/dimitrov-d/solana-forum-summarizer-mcp) |
| **daoCLI MCP** | DAO | Solana-based DAO deployment via CLI | 🟢 Live | [DaoCLI/daoCLI-init](https://github.com/DaoCLI/daoCLI-init) |
| **Awesome Solana MCP** | Resource list | Curated list of Solana MCP servers | 🟢 Live | [sendaifun/awesome-solana-mcp-servers](https://github.com/sendaifun/awesome-solana-mcp-servers) |

---

## 🟠 Bitcoin & Lightning MCPs

> **Note:** Bitquery's MCP currently covers Solana, Ethereum, BSC, Base, Arbitrum, Optimism, Polygon, and Tron. For Bitcoin-native trade and UTXO data, use the dedicated MCPs below.

| MCP | Network | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Bitcoin MCP** | Bitcoin + Lightning | Key generation, validation, queries | 🟢 Live | [AbdelStark/bitcoin-mcp](https://github.com/AbdelStark/bitcoin-mcp) |
| **Bitcoin UTXO MCP** | Bitcoin | Track Bitcoin UTXOs and block statistics | 🟢 Live | [kukapay/bitcoin-utxo-mcp](https://github.com/kukapay/bitcoin-utxo-mcp) |
| **Lightning Network MCP** | Lightning | AI-driven Lightning payments, invoices, balances | 🟢 Live | [AbdelStark/lightning-mcp](https://github.com/AbdelStark/lightning-mcp) |
| **Zebedee ZBD MCP** | Lightning | Bitcoin micropayments & rewards | 🟢 Live | [zebedeeio/zbd-mcp-server](https://github.com/zebedeeio/zbd-mcp-server) |

---

## 🔵 Base, BNB, TON, Sui, Tron & Other Chain MCPs

| MCP | Chain | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | Base, BSC, Tron (+ Arbitrum, Optimism, Polygon) | Per-trade DEX rows, OHLC, market cap, wallet PnL across all 8 chains | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **Base MCP** | Base (Coinbase) | Wallet, contracts, ERC-20/721/1155, Morpho vaults, onramp, Farcaster | 🟢 Live | [base/base-mcp](https://github.com/base/base-mcp) |
| **Base USDC Transfer** | Base | Free USDC transfers via Coinbase MPC wallets | 🟢 Live | [magnetai/mcp-free-usdc-transfer](https://github.com/magnetai/mcp-free-usdc-transfer) |
| **PancakeSwap PoolSpy** | BNB / multi | Tracks new PancakeSwap liquidity pools | 🟢 Live | [kukapay/pancakeswap-poolspy-mcp](https://github.com/kukapay/pancakeswap-poolspy-mcp) |
| **BSC Multisend** | BSC | Bulk BNB / BEP-20 transfers | 🟢 Live | [kukapay/bsc-multisend-mcp](https://github.com/kukapay/bsc-multisend-mcp) |
| **Sui Trader MCP** | Sui | Token swaps on Sui blockchain | 🟢 Live | [kukapay/sui-trader-mcp](https://github.com/kukapay/sui-trader-mcp) |
| **Ergo Explorer MCP** | Ergo | Tx history, address forensic analysis | 🟢 Live | [marctheshark3/ergo-mcp](https://github.com/marctheshark3/ergo-mcp) |
| **Uniswap on Monad** | Monad | Uniswap V2 trading on Monad Testnet | 🟢 Live | [K115DuyBowl/Monad-Testnet-Uniswap-MCP-Server](https://github.com/K115DuyBowl/Monad-Testnet-Uniswap-MCP-Server) |
| **Chainlist MCP** | EVM meta | Verified EVM chain info & RPC endpoints | 🟢 Live | [kukapay/chainlist-mcp](https://github.com/kukapay/chainlist-mcp) |

---

## 💱 DEX & On-Chain Trading MCPs

For AI agents that swap, trade, snipe, copy-trade, and analyse decentralised exchanges across chains.

| MCP | Venue | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **⭐ Bitquery MCP** | All major DEXs | Per-trade rows, OHLC, market cap, outlier filter | 🟢 Live | [mcp.bitquery.io](https://mcp.bitquery.io/) |
| **Uniswap Trader MCP** | Uniswap V3 | Automated Uniswap trading | 🟢 Live | [kukapay/uniswap-trader-mcp](https://github.com/kukapay/uniswap-trader-mcp) |
| **Uniswap Pools MCP** | Uniswap | Query pools / pairs by token | 🟢 Live | [kukapay/uniswap-pools-mcp](https://github.com/kukapay/uniswap-pools-mcp) |
| **Uniswap PoolSpy** | Uniswap multi-chain | Track new Uniswap pools | 🟢 Live | [kukapay/uniswap-poolspy-mcp](https://github.com/kukapay/uniswap-poolspy-mcp) |
| **Uniswap Price MCP** | Uniswap V3 | Real-time Uniswap V3 prices | 🟢 Live | [kukapay/uniswap-price-mcp](https://github.com/kukapay/uniswap-price-mcp) |
| **Jupiter MCP** | Solana | Token swaps on Jupiter Ultra | 🟢 Live | [kukapay/jupiter-mcp](https://github.com/kukapay/jupiter-mcp) |
| **Aster Info MCP** | Aster DEX | Structured Aster market data | 🟢 Live | [kukapay/aster-info-mcp](https://github.com/kukapay/aster-info-mcp) |
| **Binance Alpha MCP** | Binance Alpha | Track Binance Alpha trades | 🟢 Live | [kukapay/binance-alpha-mcp](https://github.com/kukapay/binance-alpha-mcp) |
| **DEX Metrics MCP** | Multi-DEX | Trading volume metrics by chain & frontend | 🟢 Live | [kukapay/dex-metrics-mcp](https://github.com/kukapay/dex-metrics-mcp) |
| **DEX Pools MCP** | Multi-DEX | Real-time DEX liquidity pool data | 🟢 Live | [kukapay/dex-pools-mcp](https://github.com/kukapay/dex-pools-mcp) |
| **DexScreener MCP** | DexScreener | Real-time DEX pair data & market stats | 🟢 Live | [opensvm/dexscreener-mcp-server](https://github.com/opensvm/dexscreener-mcp-server) |
| **DexScreener Trending MCP** | DexScreener | Trending tokens feed | 🟢 Live | [kukapay/dexscreener-trending-mcp](https://github.com/kukapay/dexscreener-trending-mcp) |
| **DexPaprika MCP** | DexPaprika | 5M+ tokens, 20+ chains, prices, pools, history | 🟢 Live | [coinpaprika/dexpaprika-mcp](https://github.com/coinpaprika/dexpaprika-mcp) |
| **Hyperliquid Info MCP** | Hyperliquid | Perp DEX market data | 🟢 Live | [kukapay/hyperliquid-info-mcp](https://github.com/kukapay/hyperliquid-info-mcp) |
| **Hyperliquid MCP (edk)** | Hyperliquid | Bracket orders, account mgmt, testnet | 🟢 Live | [edkdev/hyperliquid-mcp](https://github.com/edkdev/hyperliquid-mcp) |
| **Hyperliquid MCP (PlayAI)** | Hyperliquid | USD sizing, leverage, dual-account security | 🟢 Live | [PlayAINetwork/hyperliquid](https://github.com/PlayAINetwork/hyperliquid) |
| **Alpha Arena MCP** | Hyperliquid | Account data + perp tools for AI agents | 🟢 Live | [kukapay/alpha-arena-mcp](https://github.com/kukapay/alpha-arena-mcp) |
| **Funding Rates MCP** | All major venues | Real-time funding rates across exchanges | 🟢 Live | [kukapay/funding-rates-mcp](https://github.com/kukapay/funding-rates-mcp) |
| **Crypto Orderbook MCP** | Multi-venue | Order book depth & imbalance analysis | 🟢 Live | [kukapay/crypto-orderbook-mcp](https://github.com/kukapay/crypto-orderbook-mcp) |
| **Crypto Liquidations MCP** | Multi-venue | Streams liquidation events | 🟢 Live | [kukapay/crypto-liquidations-mcp](https://github.com/kukapay/crypto-liquidations-mcp) |
| **Freqtrade MCP** | Freqtrade | Connect Freqtrade trading bot to LLMs | 🟢 Live | [kukapay/freqtrade-mcp](https://github.com/kukapay/freqtrade-mcp) |
| **Backtrader MCP** | Backtrader | AI-accessible trading sandbox | 🟢 Live | [kukapay/backtrader-mcp](https://github.com/kukapay/backtrader-mcp) |

---

## 🏛️ Centralized Exchange (CEX) MCPs

For AI agents that need access to centralised exchange APIs — trading, balances, derivatives, and announcements.

| MCP | Exchange | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Binance MCP (nirholas)** | Binance | 478+ tools — spot, margin, futures, staking, NFT, copy trading | 🟢 Live | [nirholas/binance-mcp](https://github.com/nirholas/binance-mcp) |
| **Bybit MCP (official)** | Bybit | 247 tools — full Bybit V5 API, spot, derivatives, block trading | 🟢 Live | [bybit-exchange/bybit-mcp](https://github.com/bybit-exchange/bybit-mcp) |
| **Bybit Trading MCP** | Bybit | 22 market data + 11 account tools, WebSocket | 🟢 Live | [bybit-exchange/trading-mcp](https://github.com/bybit-exchange/trading-mcp) |
| **Coinbase Base MCP** | Coinbase / Base | Wallet, contracts, NFTs, Morpho, onramp | 🟢 Live | [base/base-mcp](https://github.com/base/base-mcp) |
| **Binance Announcements** | Binance | Latest announcements feed | 🟢 Live | [kukapay/binance-announcements-mcp](https://github.com/kukapay/binance-announcements-mcp) |
| **Bybit Announcements** | Bybit | Latest announcements feed | 🟢 Live | [kukapay/bybit-announcements-mcp](https://github.com/kukapay/bybit-announcements-mcp) |
| **OKX Announcements** | OKX | Latest announcements feed | 🟢 Live | [kukapay/okx-announcements-mcp](https://github.com/kukapay/okx-announcements-mcp) |
| **Gate.io Announcements** | Gate.io | Latest announcements feed | 🟢 Live | [kukapay/gate-announcements-mcp](https://github.com/kukapay/gate-announcements-mcp) |
| **MEXC Announcements** | MEXC | Latest announcements feed | 🟢 Live | [kukapay/mexc-announcements-mcp](https://github.com/kukapay/mexc-announcements-mcp) |

---

## 🏦 DeFi, Lending & Yield MCPs

DeFi-native MCPs for lending markets, vaults, yields, and liquidity-pool risk.

| MCP | Protocol | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **DefiLlama MCP** | DefiLlama | TVL, prices, stablecoin info | 🟢 Live | [dcSpark/mcp-server-defillama](https://github.com/dcSpark/mcp-server-defillama) |
| **DeFi Yields MCP** | DefiLlama | Explore DeFi yield opportunities | 🟢 Live | [kukapay/defi-yields-mcp](https://github.com/kukapay/defi-yields-mcp) |
| **Aave MCP** | Aave | Real-time lending markets on Aave | 🟢 Live | [kukapay/aave-mcp](https://github.com/kukapay/aave-mcp) |
| **Euler Vaults MCP** | Euler Finance | Instant access to Euler lending vaults | 🟢 Live | [kukapay/euler-vaults-mcp](https://github.com/kukapay/euler-vaults-mcp) |
| **Lista Vaults MCP** | Lista DAO | Track and act across Lista DAO lending vaults | 🟢 Live | [kukapay/lista-vaults-mcp](https://github.com/kukapay/lista-vaults-mcp) |
| **Arcadia Finance** | Arcadia | Concentrated liquidity, leverage, rebalancing on Base / Optimism | 🟢 Live | [arcadia-finance/mcp-server](https://github.com/arcadia-finance/mcp-server) |
| **Philidor DeFi Vault Risk** | Morpho, Aave, Spark, Yearn, Beefy, Compound, Uniswap | 700+ vault risk scoring (Asset / Platform / Governance) | 🟢 Live | [mcp.philidor.io](https://mcp.philidor.io) · [GitHub](https://github.com/Philidor-Labs/philidor-mcp) |
| **Uma Rocks** *(prediction market)* | UMA / Polygon | DeFi prediction-market data | 🟢 Live | [umarocks.com](https://umarocks.com) |

---

## 💲 Price Feeds & Oracle MCPs

| MCP | Source | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Chainlink Feeds MCP** | Chainlink | Real-time decentralised on-chain price feeds | 🟢 Live | [kukapay/chainlink-feeds-mcp](https://github.com/kukapay/chainlink-feeds-mcp) |
| **Pyth Network MCP (Python)** | Pyth | 1,930+ feeds, real-time prices, TWAP, historical | 🟢 Live | [itsOmSarraf/pyth-network-mcp](https://github.com/itsOmSarraf/pyth-network-mcp) |
| **Pyth MCP Server (TS)** | Pyth | 11 tools — feeds, OHLCV candles, EMA, TWAP | 🟢 Live | [Chop-Kampfire/pyth-mcp-server](https://github.com/Chop-Kampfire/pyth-mcp-server) |
| **Pyth Pro MCP** | Pyth | Pyth Pro feeds, candlesticks, historical | 🟢 Live | [aditya520/pyth-mcp](https://github.com/aditya520/pyth-mcp) |

---

## 📈 Market Data & Analytics MCPs

For LLMs that need price, volume, market-cap, sentiment, and technical-analysis data.

| MCP | Source | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **CoinGecko MCP** | CoinGecko | Tokens, market data | 🟢 Live | [Blockchain-MCPs/coingecko-mcp](https://github.com/Blockchain-MCPs/coingecko-mcp) |
| **CoinMarketCap MCP** | CoinMarketCap | Real-time prices, market cap, volume | 🟢 Live | [anjor/coinmarket-mcp-server](https://github.com/anjor/coinmarket-mcp-server) · [longmans/coin_api_mcp](https://github.com/longmans/coin_api_mcp) |
| **CoinCap MCP** | CoinCap | Real-time market data — no API key | 🟢 Live | [QuantGeekDev/coincap-mcp](https://github.com/QuantGeekDev/coincap-mcp) |
| **CoinStats MCP** | CoinStats | Market data, portfolio tracking, news | 🟢 Live | [CoinStatsHQ/coinstats-mcp](https://github.com/CoinStatsHQ/coinstats-mcp) |
| **Crypto Indicators MCP** | Computed | 50+ technical indicators & strategies | 🟢 Live | [kukapay/crypto-indicators-mcp](https://github.com/kukapay/crypto-indicators-mcp) |
| **Crypto Trending MCP** | CoinGecko | Trending tokens feed | 🟢 Live | [kukapay/crypto-trending-mcp](https://github.com/kukapay/crypto-trending-mcp) |
| **Crypto Fear & Greed MCP** | Index | Real-time + historical Crypto Fear & Greed Index | 🟢 Live | [kukapay/crypto-feargreed-mcp](https://github.com/kukapay/crypto-feargreed-mcp) |
| **Crypto Sentiment MCP** | Santiment | Sentiment analysis for tokens & projects | 🟢 Live | [kukapay/crypto-sentiment-mcp](https://github.com/kukapay/crypto-sentiment-mcp) |
| **ETF Flow MCP** | Flow data | Crypto ETF flow data | 🟢 Live | [kukapay/etf-flow-mcp](https://github.com/kukapay/etf-flow-mcp) |
| **Crypto Stocks MCP** | Equities | Real-time data for crypto-related stocks | 🟢 Live | [kukapay/crypto-stocks-mcp](https://github.com/kukapay/crypto-stocks-mcp) |
| **Crypto Funds MCP** | Funds | Crypto investment funds data | 🟢 Live | [kukapay/crypto-funds-mcp](https://github.com/kukapay/crypto-funds-mcp) |
| **Crypto Projects MCP** | Mobula.io | Project metadata & metrics | 🟢 Live | [kukapay/crypto-projects-mcp](https://github.com/kukapay/crypto-projects-mcp) |

---

## 🐳 Whale & On-Chain Activity MCPs

| MCP | Type | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Whale Tracker MCP** | Multi-chain | Track large whale transactions | 🟢 Live | [kukapay/whale-tracker-mcp](https://github.com/kukapay/whale-tracker-mcp) |
| **Hyperliquid Whale Alert** | Hyperliquid | Real-time whale alerts on Hyperliquid | 🟢 Live | [kukapay/hyperliquid-whalealert-mcp](https://github.com/kukapay/hyperliquid-whalealert-mcp) |
| **Wallet Inspector MCP** | Multi-chain | Inspect wallet balances & on-chain activity | 🟢 Live | [kukapay/wallet-inspector-mcp](https://github.com/kukapay/wallet-inspector-mcp) |
| **Tornado Cash MCP** | Ethereum | Track Tornado Cash deposits / withdrawals | 🟢 Live | [kukapay/tornado-cash-mcp](https://github.com/kukapay/tornado-cash-mcp) |
| **PumpFun Wallets MCP** | Solana | Analyse Pump.fun & PumpSwap wallets | 🟢 Live | [kukapay/pumpfun-wallets-mcp](https://github.com/kukapay/pumpfun-wallets-mcp) |

---

## 👛 Wallet & Portfolio MCPs

| MCP | Coverage | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Octav API MCP** | 20+ chains | Portfolio tracking — holdings, DeFi positions, tx history | 🟢 Live | [Octav-Labs/octav-api-mcp](https://github.com/Octav-Labs/octav-api-mcp) |
| **Armor Wallet MCP** | Solana (more chains coming) | Wallet management, swaps, DCA, stop-loss / take-profit | 🟢 Live | [armorwallet/armor-crypto-mcp](https://github.com/armorwallet/armor-crypto-mcp) |
| **WAIaaS** | EVM + Solana | Self-hosted wallet daemon, 59+ tools, x402 payments | 🟢 Live | [minhoyoo-iotrust/WAIaaS](https://github.com/minhoyoo-iotrust/WAIaaS) |
| **Wallet Inspector MCP** | Multi-chain | Wallet balances and activity | 🟢 Live | [kukapay/wallet-inspector-mcp](https://github.com/kukapay/wallet-inspector-mcp) |

---

## 🔒 Security, Risk & Compliance MCPs

| MCP | Type | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Honeypot Detector MCP** | Token risk | Detect honeypot tokens on Ethereum, BSC, Base | 🟢 Live | [kukapay/honeypot-detector-mcp](https://github.com/kukapay/honeypot-detector-mcp) |
| **Rug Check MCP** | Solana | Detects rug-pull risk in Solana meme tokens | 🟢 Live | [kukapay/rug-check-mcp](https://github.com/kukapay/rug-check-mcp) |
| **Token Revoke MCP** | EVM | Check & revoke ERC-20 token allowances | 🟢 Live | [kukapay/token-revoke-mcp](https://github.com/kukapay/token-revoke-mcp) |
| **Solana Wallet Security Scanner** | Solana | Scan wallets for threats & suspicious programs | 🟢 Live | [mohitparmar1/Solana-Wallet-Security-Scanner](https://github.com/mohitparmar1/Solana-Wallet-Security-Scanner) |
| **Philidor DeFi Vault Risk** | DeFi vaults | 700+ vaults — Asset / Platform / Governance scoring | 🟢 Live | [Philidor-Labs/philidor-mcp](https://github.com/Philidor-Labs/philidor-mcp) |
| **Heurist Mesh** | Multi-chain | Smart-contract security + on-chain analytics agents | 🟢 Live | [heurist-network/heurist-mesh-mcp-server](https://github.com/heurist-network/heurist-mesh-mcp-server) |
| **Web3 Assistant** | EVM | ABI analysis & secure contract method invocation | 🟢 Live | [EmanuelJr/web3-mcp-server](https://github.com/EmanuelJr/web3-mcp-server) |

---

## 🌉 Cross-Chain & Bridge MCPs

| MCP | Bridge | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **deBridge MCP** | deBridge | Cross-chain swap routes, fees, non-custodial trades across 30+ chains | 🟢 Live | [debridge-finance/debridge-mcp](https://github.com/debridge-finance/debridge-mcp) |
| **Stargate Bridge MCP** | Stargate | Cross-chain token transfers via Stargate | 🟢 Live | [kukapay/stargate-bridge-mcp](https://github.com/kukapay/stargate-bridge-mcp) |
| **Bridge Rates MCP** | Multi-bridge | Real-time bridge rates and routing | 🟢 Live | [kukapay/bridge-rates-mcp](https://github.com/kukapay/bridge-rates-mcp) |
| **Bridge Metrics MCP** | Multi-bridge | Real-time cross-chain bridge metrics | 🟢 Live | [kukapay/bridge-metrics-mcp](https://github.com/kukapay/bridge-metrics-mcp) |
| **Wormhole Metrics MCP** | Wormhole | Wormhole cross-chain activity analytics | 🟢 Live | [kukapay/wormhole-metrics-mcp](https://github.com/kukapay/wormhole-metrics-mcp) |

---

## 🖼️ NFT MCPs

| MCP | Marketplace / Source | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **OpenSea Skill (MCP)** | OpenSea | NFT data + Seaport trades, ERC-20 swaps multi-chain | 🟢 Live | [ProjectOpenSea/opensea-skill](https://github.com/ProjectOpenSea/opensea-skill) |
| **OpenSea MCP Sample** | OpenSea | Next.js + Vercel AI SDK sample over OpenSea MCP | 🟢 Live | [ProjectOpenSea/opensea-mcp-next-sample](https://github.com/ProjectOpenSea/opensea-mcp-next-sample) |
| **Magic Eden MCP** | Magic Eden | 17 chains — collections, NFTs, wallets, analytics, 22 tools | 🟢 Live | [Tairon-ai/magiceden-mcp](https://github.com/Tairon-ai/magiceden-mcp) |
| **NFT Analytics MCP** | Dune | NFT collection analytics powered by Dune | 🟢 Live | [kukapay/nft-analytics-mcp](https://github.com/kukapay/nft-analytics-mcp) |

---

## 📰 News, Sentiment & Information MCPs

| MCP | Source | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **CryptoPanic MCP** | CryptoPanic | Latest crypto news to AI agents | 🟢 Live | [kukapay/cryptopanic-mcp-server](https://github.com/kukapay/cryptopanic-mcp-server) |
| **Cointelegraph MCP** | Cointelegraph | Real-time news from Cointelegraph | 🟢 Live | [kukapay/cointelegraph-mcp](https://github.com/kukapay/cointelegraph-mcp) |
| **BlockBeats MCP** | BlockBeats | Blockchain news & articles | 🟢 Live | [kukapay/blockbeats-mcp](https://github.com/kukapay/blockbeats-mcp) |
| **Crypto News MCP** | NewsData | Aggregated crypto news | 🟢 Live | [kukapay/crypto-news-mcp](https://github.com/kukapay/crypto-news-mcp) |
| **Crypto RSS MCP** | RSS feeds | Aggregated RSS news for agents | 🟢 Live | [kukapay/crypto-rss-mcp](https://github.com/kukapay/crypto-rss-mcp) |
| **Kukapay News MCP** | Kukapay | Hosted aggregated crypto news MCP | 🟢 Live | [kukapay/kukapay-news-mcp](https://github.com/kukapay/kukapay-news-mcp) |
| **Crypto Whitepapers MCP** | Whitepapers | Knowledge base of crypto whitepapers | 🟢 Live | [kukapay/crypto-whitepapers-mcp](https://github.com/kukapay/crypto-whitepapers-mcp) |
| **Twitter Username Changes MCP** | X / Twitter | Track Twitter username history (alpha signals) | 🟢 Live | [kukapay/twitter-username-changes-mcp](https://github.com/kukapay/twitter-username-changes-mcp) |
| **Dappier MCP** | Dappier | Real-time crypto + finance + news content | 🟢 Live | [DappierAI/dappier-mcp](https://github.com/DappierAI/dappier-mcp) |

---

## 💸 Crypto Payments MCPs

| MCP | Network | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Lightning Network MCP** | Bitcoin Lightning | Invoice payments & balances | 🟢 Live | [AbdelStark/lightning-mcp](https://github.com/AbdelStark/lightning-mcp) |
| **Zebedee ZBD MCP** | Lightning | Micropayments & rewards | 🟢 Live | [zebedeeio/zbd-mcp-server](https://github.com/zebedeeio/zbd-mcp-server) |
| **Base USDC Transfer** | Base | Free USDC transfers via Coinbase MPC | 🟢 Live | [magnetai/mcp-free-usdc-transfer](https://github.com/magnetai/mcp-free-usdc-transfer) |
| **Universal Crypto MCP (x402)** | EVM + Solana | x402 Payment Protocol for AI agent payments | 🟢 Live | [nirholas/universal-crypto-mcp](https://github.com/nirholas/universal-crypto-mcp) |

---

## 🚀 Memecoins & Launchpad MCPs

| MCP | Ecosystem | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Memecoin Radar MCP** | Solana | Pump.fun & Solana memecoin radar | 🟢 Live | [kukapay/memecoin-radar-mcp](https://github.com/kukapay/memecoin-radar-mcp) |
| **Memecoin Observatory** | Solana | Cultural analysis, social signals, rug protection | 🟢 Live | [tony-42069/solana-mcp](https://github.com/tony-42069/solana-mcp) |
| **Solana Launchpads MCP** | Solana | Daily launchpad activity | 🟢 Live | [kukapay/solana-launchpads-mcp](https://github.com/kukapay/solana-launchpads-mcp) |
| **Raydium LaunchLab MCP** | Solana | Launch / buy / sell on Raydium LaunchLab | 🟢 Live | [kukapay/raydium-launchlab-mcp](https://github.com/kukapay/raydium-launchlab-mcp) |
| **PumpSwap MCP** | Solana | Automated PumpSwap trading | 🟢 Live | [kukapay/pumpswap-mcp](https://github.com/kukapay/pumpswap-mcp) |
| **MCP Meme Deployer** | Solana | Deploy tradable memecoins via chat | 🟢 Live | [kirabuilds/mcp-meme-deployer](https://github.com/kirabuilds/mcp-meme-deployer) |
| **PumpFun Wallets MCP** | Solana | Analyse Pump.fun & PumpSwap wallets | 🟢 Live | [kukapay/pumpfun-wallets-mcp](https://github.com/kukapay/pumpfun-wallets-mcp) |

---

## 🗳️ DAO & Governance MCPs

| MCP | Coverage | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **DAO Proposals MCP** | Major DAOs | Live governance proposals across DAOs | 🟢 Live | [kukapay/dao-proposals-mcp](https://github.com/kukapay/dao-proposals-mcp) |
| **daoCLI** | Solana | Deploy customisable DAOs via CLI | 🟢 Live | [DaoCLI/daoCLI-init](https://github.com/DaoCLI/daoCLI-init) |

---

## 🛠️ Developer Tools & Utility MCPs

| MCP | Type | Capabilities | Status | Link |
| --- | --- | --- | --- | --- |
| **Token Minter MCP** | EVM | Mint ERC-20 tokens across chains | 🟢 Live | [kukapay/token-minter-mcp](https://github.com/kukapay/token-minter-mcp) |
| **Contract Scraper MCP** | Multi-chain | Scrape verified contract source code & ABIs | 🟢 Live | [kukapay/contract-scraper-mcp](https://github.com/kukapay/contract-scraper-mcp) |
| **Find Block MCP** | EVM | Resolve block numbers from timestamps | 🟢 Live | [kukapay/findblock-mcp](https://github.com/kukapay/findblock-mcp) |
| **Chainlist MCP** | EVM | Verified EVM chain info & RPC endpoints | 🟢 Live | [kukapay/chainlist-mcp](https://github.com/kukapay/chainlist-mcp) |
| **mcp-clickhouse** | Database | The open-source server underneath Bitquery's MCP | 🟢 Live | [ClickHouse/mcp-clickhouse](https://github.com/ClickHouse/mcp-clickhouse) |

---

## 📚 Resources

### Official MCP Resources

- [Model Context Protocol — Specification](https://modelcontextprotocol.io/) — the open standard MCP servers implement
- [MCP Servers — Official List by Anthropic](https://github.com/modelcontextprotocol/servers) — the canonical reference index
- [How to Use MCP Tools on Claude Desktop](https://medium.com/@pedro.aquino.se/how-to-use-mcp-tools-on-claude-desktop-app-and-automate-your-daily-tasks-1c38e22bc4b0) — beginner-friendly guide
- [Model Context Protocol Quickstart](https://glama.ai/blog/2024-11-25-model-context-protocol-quickstart) — protocol basics, server & client setup

### Bitquery (Featured) Resources

- [Bitquery MCP — Overview](https://docs.bitquery.io/docs/mcp/mcp-server/) — what the server is and how it works
- [Bitquery MCP — Use Cases](https://docs.bitquery.io/docs/mcp/trading/use-cases/) — eleven conversational patterns with prompting tips
- [Bitquery MCP — Worked Examples](https://docs.bitquery.io/docs/mcp/trading/examples/) — six trader workflows with charts and real numbers
- [Bitquery Crypto Price API](https://docs.bitquery.io/docs/trading/crypto-price-api/introduction/) — GraphQL alternative for the same data
- [Bitquery Crypto Trades API](https://docs.bitquery.io/docs/trading/crypto-trades-api/trades-api/) — swap-level streams (real-time + historical)
- [Bitquery Price Index Algorithm](https://docs.bitquery.io/docs/trading/crypto-price-api/price-index-algorithm/) — outlier-filter & ranking logic
- [Bitquery Account](https://account.bitquery.io/) — sign up / manage plan / generate API tokens

### Other Awesome Lists

- [badkk/awesome-crypto-mcp-servers](https://github.com/badkk/awesome-crypto-mcp-servers)
- [royyannick/awesome-blockchain-mcps](https://github.com/royyannick/awesome-blockchain-mcps)
- [hive-intel/awesome-crypto-mcp-servers](https://github.com/hive-intel/awesome-crypto-mcp-servers)
- [sendaifun/awesome-solana-mcp-servers](https://github.com/sendaifun/awesome-solana-mcp-servers)
- [kukapay/kukapay-mcp-servers](https://github.com/kukapay/kukapay-mcp-servers)

### MCP Directories & Discovery

- [MCPHub](https://mcphub.com/) — directory of MCP servers
- [MCP.so Server Directory](https://mcp.so/) — searchable catalogue
- [MCP-Hub.ink](https://mcp-hub.ink/) — community catalogue
- [Smithery](https://smithery.ai/) — install & manage MCP servers
- [Glama AI MCP Directory](https://glama.ai/mcp/servers) — comprehensive listing

### Client Setup Guides

- [Cursor — MCP Setup](https://docs.cursor.com/context/model-context-protocol)
- [Claude Desktop — MCP Setup](https://modelcontextprotocol.io/quickstart/user)
- [Claude Code — MCP CLI Reference](https://docs.anthropic.com/en/docs/build-with-claude/claude-code/mcp)
- [VS Code — MCP Support](https://code.visualstudio.com/docs/copilot/copilot-mcp)

### Community

- [MCP Discord](https://discord.gg/modelcontextprotocol)
- [Anthropic Discord](https://discord.gg/anthropic)
- [Bitquery Telegram](https://t.me/Bloxy_info)
- [Bitquery Support](https://support.bitquery.io/)

---

## 🤝 Contributing

Contributions are very welcome! Help make this the most comprehensive crypto MCP directory on the internet.

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/AddYourMCP`)
3. Add your MCP server in the most relevant category — use the existing table format
4. Make sure your MCP:
   - Has a public GitHub repo or hosted endpoint
   - Implements the [MCP specification](https://modelcontextprotocol.io/)
   - Provides clear setup instructions
5. Commit your changes (`git commit -m 'Add YourMCP under DEX & On-Chain Trading MCPs'`)
6. Push to your branch (`git push origin feature/AddYourMCP`)
7. Open a Pull Request

**Quality bar:** every entry should genuinely help an AI agent work with crypto. We don't list MCPs that are abandoned, broken, or unrelated to crypto/Web3.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

**Note**: The MCP ecosystem moves fast. Status, features, and endpoints can change — always verify on each project's website / repository before using in production.

Made with ❤️ for the AI × Crypto community.

---

## 🔍 Related Searches

If you arrived here looking for any of the following, you're in the right place:

`crypto MCP servers` · `blockchain MCP` · `Bitquery MCP` · `Solana MCP` · `Ethereum MCP` · `EVM MCP` · `DeFi MCP` · `DEX trading MCP` · `on-chain data MCP` · `AI crypto agents` · `MCP server for Cursor` · `MCP server for Claude Desktop` · `best crypto MCP servers`

---

## 📈 Popular Use Cases

- **AI Trading Agents** — give Claude / Cursor / GPT real-time DEX trade data via Bitquery MCP, then execute swaps via Jupiter, Uniswap, or GOAT
- **On-Chain Copilots** — wallet-level PnL, holdings, history, and risk via Bitquery + Octav + Wallet Inspector
- **Memecoin Hunting** — combine Memecoin Radar, Pump.fun trackers, Bitquery trades, and Rug Check MCP for a degen workflow
- **DeFi Research** — query Aave / Euler / Lista vaults, score risk with Philidor, and check yields via DefiLlama MCP
- **Whale Tracking** — pipe Whale Tracker MCP and Hyperliquid Whale Alert into your agent for early signals
- **Cross-Chain Operations** — let your agent quote and route through deBridge, Stargate, and Bridge Rates MCP
- **Smart Contract Security** — combine Honeypot Detector, Token Revoke, Rug Check, and Heurist Mesh for a security copilot
- **NFT Analytics & Trading** — OpenSea, Magic Eden, and NFT Analytics MCPs for collection-level insight + trades
- **Crypto Research Assistants** — CryptoPanic + Cointelegraph + sentiment + Crypto Whitepapers MCP into a research agent
- **Quant Backtesting** — Backtrader MCP + Crypto Indicators MCP + Bitquery trade history for a full quant loop
- **CEX Trading Bots** — Binance MCP / Bybit MCP / Coinbase Base for exchange execution from natural language
- **Prediction-Market Agents** — Polymarket Predictions MCP and UMA Rocks for forecasting workflows
- **DAO Governance Bots** — DAO Proposals MCP for monitoring & voting workflows across major DAOs
- **AI Payments** — x402, Lightning Network, and Base USDC Transfer MCPs for autonomous-agent micropayments



