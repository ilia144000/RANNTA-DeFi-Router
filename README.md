<p align="center">
  <img src="./banner.svg" width="100%" />
</p>

# RANNTA DeFi Router — Liquidity Intelligence Layer for TON

> **Alpha Release — Public Shell Only**  
> Core routing logic, liquidity models, and scoring algorithms remain private.

Created and maintained by **ilia144000** — Founder of RANNTA Protocol.

---

## 🔍 Overview

The **RANNTA DeFi Router** introduces a missing DeFi primitive inside  
**The Open Network (TON): a unified intelligence layer for multi-DEX  
price discovery, routing, and liquidity evaluation.**

TON currently relies on two major DEXs — **STON.fi** and **DeDust** — but lacks:

- a shared routing layer  
- a unified price engine  
- liquidity scoring  
- large-swap impact heuristics  
- a public routing API  

The RANNTA Router fills this gap by providing:

- `/prices` — consolidated TON/USDT price feed  
- `/route` — best-path routing across DEXs  
- `/health` — operational check  
- lightweight monitoring UI  

> ⚠ Only the integration layer is public.  
> Strategic routing logic, weighting models, and predictive heuristics  
> remain proprietary to the RANNTA Protocol.

---

## 🚦 API Examples

### GET /health
```json
{
  "ok": true,
  "service": "RANNTA DeFi Router",
  "version": "phase-4"
}
```

### GET /prices
```json
{
  "pair": "TON/USDT",
  "bestPrice": "...",
  "sources": [
    {
      "pair": "TON/USDT",
      "price": "...",
      "reserves": {}
    }
  ]
}
```

### GET /route?from=TON&to=USDT&amount=100
```json
{
  "bestDex": "STON.fi",
  "estimatedOut": "...",
  "impact": "...",
  "route": [
    {
      "dex": "STON.fi",
      "path": ["TON", "USDT"]
    }
  ]
}
```

---

## 🧩 Architecture (Public Layer Only)

```bash
Client / Wallet / Marketplace
      │
      ▼
RANNTA Router API
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
```

---

## 🚀 Use Cases

- **ArcWallet Gen-5** — in-wallet smart routing  
- **RANNTAverse Marketplace** — optimal TON ↔ RANNTA swap paths  
- **Bots & dashboards** — unified price feed  
- **Developers** — predictable routing API for TON  

---

## 📜 Licensing & Restrictions

This repository exposes only the **public shell** of the RANNTA Router.  
Private routing logic and liquidity algorithms are intellectual property of  
the RANNTA Protocol.

### ❌ You may NOT:
- reverse-engineer private routing logic  
- build derivative routing engines for commercial use  
- use the RANNTA identity for competing products  
- package, republish, or resell the routing logic  

### ✔ You MAY:
- use public API endpoints (`/health`, `/prices`, `/route`)  
- build UI integrations  
- contribute improvements to non-core components  

For commercial licensing or partnership inquiries, contact the maintainer.

---

© 2025 **RANNTA Protocol** — All Rights Reserved.
