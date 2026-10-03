<p align="center">
  <img src="taridoku.jpg" alt="Taridoku Logo" width="200"/>
</p>

# 👾 Taridoku (gh0xt) — Solidity Security Researcher & Auditor

**Open to private audits and protocol security consulting.** [Contact me on Telegram](https://t.me/taridoku).

---

## About

I audit DeFi protocols with a focus on economic flaws, access control, and cross-chain design. My approach combines manual code review, invariant-driven testing, and protocol-level reasoning.

My experience includes multiple engagements with BurraSec and confidential DeFi audits.

Podium finishes include 1st place on Neutrl Protocol and 2nd place on Centrifuge V3.1 and Flying Tulip.

## Private engagements

| Review dates | Protocol | Scope | Team | Report |
|---|---|---|---|---|
| Aug 20–21, 2026 | Centrifuge | ShareManager | BurraSec | [Report](https://github.com/centrifuge/protocol/blob/main/docs/audits/2026-08-burraSec-ShareManager.pdf) |
| Jul 28–Aug 3, 2026 | Centrifuge | v3.3, Part 2 | BurraSec | [Report](https://github.com/centrifuge/protocol/blob/main/docs/audits/2026-08-burraSec-v3.3.pdf) |
| Jul 16–17, 2026 | Centrifuge | TokenBridge | BurraSec | [Report](https://github.com/centrifuge/protocol/blob/main/docs/audits/2026-07-burraSec-bridge.pdf) |
| Jul 6–15, 2026 | Centrifuge | v3.3 — Manifest permissions & cross-chain messaging | BurraSec | [Report](https://github.com/centrifuge/protocol/blob/main/docs/audits/2026-07-burraSec-v3.3.pdf) |
| Apr 6–9, 2026 | Centrifuge | OnchainPM | BurraSec | [Report](https://github.com/centrifuge/protocol/blob/main/docs/audits/2026-04-burraSec-onchain-pm.pdf) |
| — | Undisclosed | DeFi | BurraSec | Confidential |
| — | Undisclosed | DeFi | BurraSec | Confidential |
| — | Undisclosed | DeFi | BurraSec | Confidential |
| — | Undisclosed | DeFi | BurraSec | Confidential |
| — | Undisclosed | DeFi | BurraSec | Confidential |

## Selected Findings

| Finding | Severity | Protocol | Category |
|---|---|---|---|
| [Malicious BRM permits global escrow drain](https://audits.sherlock.xyz/contests/1028/voting/274) | High | Centrifuge V3.1 | Access Control |
| [Market collateral drain with `migrateTo()`](https://audits.sherlock.xyz/contests/1073/voting/323) | High | USG – Tangent | Economic / Value Extraction |
| [Order double-linked list broken — `prevOrderId` not persisted](https://code4rena.com/audits/2025-07-gte-spot-clob-and-router/submissions/S-287) | High | GTE Spot CLOB | State / Data Integrity |
| [Protocol-wide fee bypass via logical error in ValueFacet](https://audits.sherlock.xyz/contests/858/voting/258) | High | Burve | Economic / Fee Logic |
| [FULL_RESTRICTED users stake bypass](https://audits.sherlock.xyz/contests/1065/voting/230) | Medium | Neutrl Protocol | Access Control |
| [Blacklist bypass in `mTokenGateway.outHere`](https://audits.sherlock.xyz/contests/1029/voting/310) | Medium | Malda | Access Control |
| [Stale window check causes rollover-time DoS](https://audits.sherlock.xyz/contests/1029/voting/403) | Medium | Malda | Timing / DoS |
| [First depositor captures unearned rewards after zero-supply window](https://audits.sherlock.xyz/contests/1073/voting/630) | Medium | USG – Tangent | Economic / First-Depositor |
| [Stranded ETH on batched `crosschainTransferShares`](https://audits.sherlock.xyz/contests/1028/voting/397) | Medium | Centrifuge V3.1 | Value Forwarding |

## Audit Contests

| Date | Protocol | Type | Platform | Findings |
|---|---|---|---|---|
| Mar '26 | [Current Finance](https://audits.sherlock.xyz/contests/1256?filter=questions) | Lending / Collateral | Sherlock | [ 1H, 1M](https://audits.sherlock.xyz/contests/1256?filter=results) |
| Jan '26 | [Fluid Dex V2](https://audits.sherlock.xyz/contests/1225?filter=questions) | DEX | Sherlock | [ 1H, 1M ](https://audits.sherlock.xyz/contests/1225) |
| Jan '26 | Flying Tulip| AMM / DeFi | Sherlock | — |
| Oct '25 | [Centrifuge Protocol V3.1](https://audits.sherlock.xyz/contests/1028) | Cross-chain / RWA | Sherlock | [1 H, 1 M](https://audits.sherlock.xyz/contests/1028?filter=results) |
| Sep '25 | [Ammplify](https://audits.sherlock.xyz/contests/1054) | AMM | Sherlock | [2 M](https://audits.sherlock.xyz/contests/1054?filter=results) |
| Aug '25 | [USG – Tangent](https://audits.sherlock.xyz/contests/1073) | Lending / Collateral | Sherlock | [1 H, 2 M](https://audits.sherlock.xyz/contests/1073) |
| Aug '25 | [Kuru Contracts](https://cantina.xyz/competitions/cdce21ba-b787-4df4-9c56-b31d085388e7) | DEX / CLOB | Cantina | [2 H](https://cantina.xyz/code/cdce21ba-b787-4df4-9c56-b31d085388e7/overview/leaderboard)|
| Aug '25 | [Neutrl Protocol](https://audits.sherlock.xyz/contests/1065) | Staking / Compliance | Sherlock | [1 M](https://audits.sherlock.xyz/contests/1065/voting/230) |
| Jul '25 | [Malda](https://audits.sherlock.xyz/contests/1029) | Cross-chain Lending | Sherlock | [3 M](https://audits.sherlock.xyz/contests/1029) |
| Jul '25 | [GTE Spot CLOB](https://code4rena.com/audits/2025-07-gte-spot-clob-and-router) | DEX / Order Book | Code4rena | [1 H](https://code4rena.com/reports/2025-07-gte-spot-clob-and-router) |
| May '25 | [Superform Core](https://cantina.xyz/competitions/ba62fa4e-f933-4eec-b9ac-868325f4a694) | Cross-chain Vaults | Cantina | [1 H, 1 M](https://cantina.xyz/code/ba62fa4e-f933-4eec-b9ac-868325f4a694/overview/leaderboard) |
| Apr '25 | [Burve](https://audits.sherlock.xyz/contests/858) | DeFi / Vaults | Sherlock | [1 H](https://audits.sherlock.xyz/contests/858/voting/258) |

## Triage engagements

| Role | Platform | Engagement |
|---|---|---|
| Triager | BurraSec | - |
| Triager | Pashov | - |
| Lead judge | Sherlock | Metric contest |

## Bug bounty

| Platform | Protocol | Confirmed severity |
|---|---|---|
| Sherlock | Undisclosed | Low |
| Public good | Undisclosed | Medium |
| Public good | Undisclosed | Medium |

## Finding Patterns

The vulnerabilities I find tend to cluster around recurring themes:

- **Access control architecture** — Structural gaps in how protocols scope trust boundaries: blacklist bypasses, restricted-user escalations, compromised-module drain vectors.
- **Economic & value extraction** — First-depositor attacks, fee bypass logic, collateral drain through migration and routing paths.
- **State & data integrity** — Broken invariants in core data structures, stranded value from incorrect forwarding, timing-dependent DoS at state transitions.

## Technical Stack

| Domain | |
|---|---|
| **Smart Contracts** | Solidity ·  Noir |
| **Testing & Fuzzing** | Foundry (forge, cast, chisel) · Invariant testing · Stateful fuzzing |
| **Formal Verification** | Certora · Halmos |
| **Ecosystems** | EVM |

## Current Work

Exploring **Noir** — zero-knowledge circuit language for private smart contract development.
- [Private token contract](https://github.com/Taridoku/Token)
- Private project
- [Reparo](https://github.com/Taridoku/reparo)


## Articles 
| Article | Domain | Link |
|---|---|---|
| Witty Authwits | Aztec smart contract development | [Link](https://x.com/Taridoku/status/2052542557918232876?s=20) |
| The two clocks on private execution | Aztec smart contract development | [Link](https://x.com/Taridoku/status/2057001073336828370?s=20) |
| Reparo | Aztec smart contract development | [Link](https://x.com/taridoku/status/2106234873904009533?s=46) |

## Contact

**X:** [@Taridoku](https://x.com/Taridoku) · **Discord:** [taridoku](https://discordapp.com/users/taridoku) · **Telegram:** [@taridoku](https://t.me/taridoku)

---

*Open to private audits, protocol security consultations, and security tooling collaborations.*
