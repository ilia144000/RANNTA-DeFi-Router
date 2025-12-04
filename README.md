<p align="center">
  <img src="./banner.svg" width="100%" />
</p>

# RANNTA DeFi Router — Liquidity Intelligence Layer for TON

> **Alpha Release — Public Shell Only**  
> Core algorithms, liquidity scoring, and routing logic remain private.

---

## 🔍 Overview

RANNTA DeFi Router introduces a missing protocol primitive for **The Open Network (TON)**:  
a unified intelligence layer for **multi-DEX price discovery, best-path routing, and liquidity analysis**.

TON today has two major DEXs — **STON.fi** and **DeDust** — yet no shared routing surface,  
no consolidated price feed, and no mechanism for wallets or dApps to evaluate swap efficiency.

RANNTA Router fills this gap with a lightweight, extensible service:

- `/prices` → unified TON/USDT pricing  
- `/route` → best-path analysis across DEXs  
- `/health` → service status  
- Minimal UI for live monitoring  

This repository exposes only the **integration layer**.  
All strategic routing logic, liquidity weighting, predictive models, and split execution mechanisms remain private.

---

## 🧠 Why This Project Exists (TON’s Missing Component)

While TON has grown rapidly, several critical DeFi primitives are still absent:

1. **No aggregator or unified price engine**  
2. **No routing intelligence for wallets**  
3. **No cross-DEX liquidity scoring**  
4. **No public API for unified TON market insight**  
5. **No prediction/impact heuristics for large swaps**

These limitations affect:

- Wallets  
- NFT marketplaces  
- Bots & analytics tools  
- TON DeFi developers  

RANNTA Router is designed to serve as the **foundation layer** for all of the above.

---

## 🧩 Architecture (Public Layer)


Client / Wallet / Marketplace
│
▼
RANNTA Router API (public)
├── /health
├── /prices
├── /route
│
▼
Abstraction Layer (open)
│
▼
RANNTA Liquidity Core (private)
├── multi-DEX indexing
├── liquidity scoring
├── split-route planner
├── RANNTA optimization logic
├── predictive heuristics

---

## 🚀 Use Cases

- **ArcWallet Gen-5** — smart routing inside the wallet  
- **RANNTAverse Marketplace** — optimal TON ↔ RANNTA swaps for NFT payments  
- **Bots & dashboards** — price feed extraction  
- **Developers** — simple and consistent routing API  

---

## 🛡 Licensing and Intellectual Property

This repository is intentionally partial.  
The full routing engine is proprietary to the **RANNTA Protocol** to preserve:

- ecosystem advantage  
- security of liquidity models  
- revenue pathways  
- protection against cloning  

Commercial usage or derivative routing services require written approval.

---

## ⚡ Status

**Current Release:** Phase-4 UI  
**Next Phases:**  
- Phase-5: Split execution engine  
- Phase-6: Predictive liquidity model  
- Phase-7: RANNTA-native optimization layer  

---

## ✨ About RANNTA

RANNTA is a symbolic, artistic, and technical protocol on **The Open Network**,  
building financial and creative tools powered by intelligence, narrative, and community.

The DeFi Router is one of its core infrastructural components.

