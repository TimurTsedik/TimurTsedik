<img src="me.jpg" width="120" align="left" alt="Timur Tsedik" style="border-radius: 50%; margin-right: 16px;" />

# Timur Tsedik

**Ex-Head of Treasury · Python engineer · treasury & payments systems**
Ashdod, Israel · +972 55 295 3793 · timur.tsedik@gmail.com · [LinkedIn](https://www.linkedin.com/in/timur-tsedik-429b8b72/)

<br clear="left"/>

I ran bank treasury for 27 years, from FX dealer to Head of Treasury, and I've been building the software treasury runs on for almost as long. Day to day I write Python backends.

## FxPosition: real-time treasury position platform

![FxPosition 1.2.25: FX position with live P/L, limit utilization and a step-by-step P/L explanation](./fxposition-position.png)

Real-time FX, payment and cash positions for a bank treasury. It started in 1999 as my own tool and followed me through three banks; in 2023 I rebuilt it from scratch. **It is now in production rollout at a top-100 Russian bank:** ~15 currencies, market rates every 5 seconds, core banking data every 30 seconds.

- Live P/L against market rates, including synthetic crosses through a bridge currency
- Planned vs actual payment matching: partial matches, multiple candidates, no double counting
- Read-only integration with the bank's Oracle core system; rate sources with priority and failover
- Immutable audit trail; one request ID links the audit record, the logs and the background job
- Delivered as an offline kit into the bank's closed network: 26 releases in the first 6 weeks of rollout

**Stack:** Python 3.12 · FastAPI · SQLAlchemy 2 · PostgreSQL · Oracle · pytest (~3,800 tests) · mypy strict · Docker · GitHub Actions · React + TypeScript

[Product site](https://fxposition.ru/en) · [Case study: architecture and hard problems](./FX_POSITION.md) · Live demo at [fxposition.biz](https://fxposition.biz), access on request
<sub>FxPosition is a commercial product, so its source is closed. The architecture is described in the case study.</sub>

## Selected projects

| | |
|---|---|
| [key-service](https://github.com/TimurTsedik/key-service) | Envelope-encryption key service: releases a file key only after a signed grant passes ordered policy checks |
| [double-brained](https://github.com/TimurTsedik/double-brained) | A second brain in Telegram: notes and voice in, answers grounded in your own sources out |
| [simple_ai_agent_bot](https://github.com/TimurTsedik/simple_ai_agent_bot) | Telegram AI agent: voice-to-text, agentic tool loop, skills and memory, admin UI for observability |
| [media-to-wiki-convertor](https://github.com/TimurTsedik/media-to-wiki-convertor) | CLI that turns audio and video into a structured Obsidian wiki |
| [Sales Assistant](https://sales-assistant.app) | Offline Android CRM, built for one real salesperson — my wife. On-device speech recognition, no server |

## Stack

**Daily:** Python, FastAPI, Falcon, SQLAlchemy, PostgreSQL, Docker, pytest
**Also:** Oracle, MS SQL, REST integrations, LLM tooling, React + TypeScript

Open to roles in Israel where treasury and engineering meet: fintech (payments, treasury, FX, liquidity), banking software vendors, treasury technology teams.
