<p align="center">
  <img src="./banner.svg" width="100%" />
</p>

# RANNTA DeFi Router — Liquidity Intelligence Layer for TON

> **Alpha Release — Public Shell Only**  
> Core routing logic, liquidity models, and scoring algorithms remain private.

Created and maintained by **ilia144000** — Founder of **RANNTA Protocol**.

---

## 🔍 Overview

The **RANNTA DeFi Router** introduces a missing DeFi primitive in  
**The Open Network (TON): a unified intelligence layer for multi-DEX  
price discovery, routing, and liquidity evaluation.**

TON currently relies on two major DEXs — **STON.fi** and **DeDust** —  
yet lacks a shared routing surface, a consolidated price engine,  
and mechanisms for wallets or dApps to assess swap efficiency.

RANNTA Router fills this structural gap through a lightweight, extensible public service:

- `/prices` → unified TON/USDT pricing  
- `/route` → best-path routing across DEXs  
- `/health` → operational heartbeat  
- minimal monitoring UI  

> ⚠️ Only the **integration layer** is public.  
> All strategic logic — liquidity weighting, heuristics, multi-route splitting,  
> and predictive modeling — is proprietary to the RANNTA Protocol.

---

## 🧠 Why This Project Exists — TON’s Missing DeFi Component

As TON accelerates in adoption, several critical DeFi components remain absent:

1. No intelligent swap aggregator  
2. No unified and reliable pricing engine  
3. No liquidity scoring or market-depth analysis  
4. No predictive modeling for slippage or large swaps  
5. No open routing API for developers and analytics platforms  

These gaps impact:

- wallets  
- NFT marketplaces  
- DeFi dashboards  
- trading bots  
- TON ecosystem developers  

The **RANNTA Router** is designed to become a shared, scalable  
**liquidity intelligence layer** for the TON network.

---

## 🧩 Architecture (Public Layer Only)

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
├── optimization heuristics
└── predictive liquidity model

yaml
Copy code

---

## 🚀 Use Cases

- **ArcWallet Gen-5** — smart routing built into the wallet  
- **RANNTAverse Marketplace** — optimal TON ↔ RANNTA swap paths  
- **Bots & dashboards** — consolidated real-time pricing  
- **Developers** — stable, predictable routing API for TON  

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

GET /route?from=TON&to=USDT&amount=100
{
  "bestDex": "STON.fi",
  "estimatedOut": "...",
  "impact": "...",
  "route": [...]
}

📜 Licensing & Restrictions

This repository exposes only the public shell of the RANNTA Router.
Private routing logic and liquidity algorithms are the
intellectual property of the RANNTA Protocol.

❌ You may NOT:

copy or reverse-engineer private routing logic

build derivative routing engines for commercial use

use the RANNTA identity for competing products

package, republish, or resell the routing logic

✔ You MAY:

use public API endpoints (/health, /prices, /route)

build UI integrations

contribute improvements to non-core open components
