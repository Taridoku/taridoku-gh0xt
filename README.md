<p align="center">
  <img src="taridoku.jpg" alt="Taridoku Logo" width="200"/>
</p>

# 👾 Taridoku (gh0xt) - **Web3 Security Researcher & Solidity Auditor**

---

## About

I audit DeFi protocols with a focus on the vulnerabilities that matter most — not just code-level bugs, but the economic and design-level flaws that lead to real exploits. My approach combines manual code review, invariant-driven testing, and protocol-level reasoning about how systems actually break under adversarial conditions.

Podium finishes include 1st place on Neutrl Protocol and 2nd place on Centrifuge V3.1 and Flying Tulip.

## Audit Contests

| Date | Protocol | Type | Platform | Findings |
|---|---|---|---|---|
| Jan '26 | [Flying Tulip](https://audits.sherlock.xyz/contests/1223) | AMM / DeFi | Sherlock | — |
| Oct '25 | [Centrifuge Protocol V3.1](https://audits.sherlock.xyz/contests/1028) | Cross-chain / RWA | Sherlock | [1 H, 1 M](https://audits.sherlock.xyz/contests/1028/voting) |
| Sep '25 | [Ammplify](https://audits.sherlock.xyz/contests/1054) | AMM | Sherlock | [2 M](https://audits.sherlock.xyz/contests/1054/voting) |
| Aug '25 | [USG – Tangent](https://audits.sherlock.xyz/contests/1073) | Lending / Collateral | Sherlock | [1 H, 2 M](https://audits.sherlock.xyz/contests/1073/voting) |
| Aug '25 | [Kuru Contracts](https://cantina.xyz/competitions/cdce21ba-b787-4df4-9c56-b31d085388e7) | DEX / CLOB | Cantina | 2 H *(not yet public)* |
| Aug '25 | [Neutrl Protocol](https://audits.sherlock.xyz/contests/1065) | Staking / Compliance | Sherlock | [1 M](https://audits.sherlock.xyz/contests/1065/voting) |
| Jul '25 | [Malda](https://audits.sherlock.xyz/contests/1029) | Cross-chain Lending | Sherlock | [3 M](https://audits.sherlock.xyz/contests/1029/voting) |
| Jul '25 | [GTE Spot CLOB](https://code4rena.com/audits/2025-07-gte-spot-clob-and-router) | DEX / Order Book | Code4rena | [1 H](https://code4rena.com/audits/2025-07-gte-spot-clob-and-router/submissions/S-287) |
| May '25 | [Superform Core](https://cantina.xyz/competitions/ba62fa4e-f933-4eec-b9ac-868325f4a694) | Cross-chain Vaults | Cantina | 1 H, 1 M *(not yet public)* |
| Apr '25 | [Burve](https://audits.sherlock.xyz/contests/858) | DeFi / Vaults | Sherlock | [1 H](https://audits.sherlock.xyz/contests/858/voting) |

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

## Finding Patterns

The vulnerabilities I find tend to cluster around recurring themes:

- **Access control architecture** — Structural gaps in how protocols scope trust boundaries: blacklist bypasses, restricted-user escalations, compromised-module drain vectors.
- **Economic & value extraction** — First-depositor attacks, fee bypass logic, collateral drain through migration and routing paths.
- **State & data integrity** — Broken invariants in core data structures, stranded value from incorrect forwarding, timing-dependent DoS at state transitions.

## Technical Stack

| Domain | |
|---|---|
| **Smart Contracts** | Solidity |
| **Testing & Fuzzing** | Foundry (forge, cast, chisel) · Invariant testing · Stateful fuzzing |
| **Formal Verification** | Certora · Halmos |
| **Ecosystems** | EVM |

## Current Work

- Exploring **Noir** — zero-knowledge circuit language for private smart contract development.

## Contact

**X:** [@Taridoku](https://x.com/Taridoku) · **Discord:** [taridoku](https://discordapp.com/users/taridoku) · **Telegram:** [@taridoku](https://t.me/taridoku)

---

*Open to private audits, protocol security consultations, and security tooling collaborations.*
