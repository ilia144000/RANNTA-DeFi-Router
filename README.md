<p align="center">
  <img src="./banner.svg" width="100%" />
</p>

# RANNTA DeFi Router — Liquidity Intelligence Layer for TON

> **Alpha Release — Public Shell Only**  
> Core algorithms, liquidity scoring models, and routing logic remain private.

Created and maintained by **ilia144000** — Founder of **RANNTA Protocol**.

---

## 🔍 Overview

The **RANNTA DeFi Router** introduces a missing protocol primitive for  
**The Open Network (TON): a unified intelligence layer for multi-DEX  
price discovery, best-path routing, and liquidity analysis.**

TON currently operates with two major DEXs — **STON.fi** and **DeDust** —  
yet lacks a shared routing surface, a consolidated price engine,  
or any mechanism for wallets and dApps to evaluate swap efficiency.

RANNTA Router fills this structural gap with a lightweight, extensible public service:

- `/prices` → unified TON/USDT pricing  
- `/route` → best-path analysis across DEXs  
- `/health` → service status  
- minimal monitoring UI  

> ⚠️ **Important**  
> This repository exposes only the **integration layer**.  
> All strategic routing logic, liquidity weighting, predictive heuristics,  
> and split execution mechanisms remain private and proprietary.

---

## 🧠 Why This Project Exists — TON’s Missing DeFi Component

As TON grows, several core DeFi primitives remain absent:

1. No aggregator or unified price engine  
2. No routing intelligence for wallets  
3. No cross-DEX liquidity scoring  
4. No public API for consolidated market insight  
5. No heuristics for large-swap impact or slippage prediction  

These limitations affect:

- wallets  
- NFT marketplaces  
- analytics dashboards  
- algorithmic trading bots  
- TON DeFi developers  

The **RANNTA Router** is designed to become the shared, scalable  
**liquidity intelligence layer** for the TON ecosystem.

---

## 🧩 Architecture (Public Layer)

Client / Wallet / Marketplace
│
▼
RANNTA Router API (public)
├── /health
├── /prices
└── /route
│
▼
Abstraction Layer (open)
│
▼
RANNTA Liquidity Core (private)
├── multi-DEX indexer
├── liquidity scoring engine
├── split-route planner
├── RANNTA optimization logic
└── predictive heuristics

---

## 🚀 Use Cases

- **ArcWallet Gen-5** — in-wallet smart routing integration  
- **RANNTAverse Marketplace** — optimal TON ↔ RANNTA swap paths for NFT payments  
- **Bots & dashboards** — unified real-time price feed  
- **Developers** — stable routing API for TON DeFi tooling  

---

GET /health
{
  "ok": true,
  "service": "RANNTA DeFi Router",
  "version": "phase-4"
}

GET /prices
{
  "pair": "TON/USDT",
  "bestPrice": "...",
  "sources": [...]
}

GET /route?from=TON&to=USDT&amount=...
{
  "bestDex": "STON.fi",
  "estimatedOut": "...",
  "impact": "...",
  "route": [...]
}



Copyright © 2025 by ilia144000
All Rights Reserved.

This repository represents only the public shell of the RANNTA Router.
The full routing engine — including scoring models, indexing logic, and
optimization algorithms — is proprietary to the RANNTA Protocol.

You may not:

use the private algorithms commercially

clone, replicate, or reverse-engineer the routing logic

build derivative routing engines without explicit written permission

use the RANNTA name or identity for competing products

You may:

use the public API in your wallet/dApp

build integrations on top of /health, /prices, /route

contribute improvements to the UI layer or public interface

For partnership or commercial licensing, contact the maintainer.

⚡ Status

Current Release: Phase-4 (Monitoring UI)
Upcoming:

Phase-5 → Split execution engine

Phase-6 → Predictive liquidity model

Phase-7 → RANNTA-native optimization layer

✨ About RANNTA

RANNTA is a symbolic, narrative-driven, and technically advanced
protocol on The Open Network (TON) — building a new class of
intelligence-powered financial and creative tools.

The RANNTA DeFi Router is one of its foundational infrastructural components,
serving ArcWallet, RANNTAverse Marketplace, and future TON-native systems.
