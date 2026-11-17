# SolGuard NG — Solana Wallet Safety Checker (v0.1 prototype)

Paste any Solana wallet address and get a plain-language safety report.
**Read-only by design:** no wallet connection, no signing, no seed phrase — ever.

## What it checks

- Active token **delegates (approvals)** — someone who can move tokens without asking again
- **Frozen** token accounts, and held tokens whose issuer kept a **freeze authority**
- Held tokens whose issuer kept a **mint authority** (supply can be printed)
- **Spam/dust** tokens (single-unit, zero-decimal — the fake-airdrop pattern)
- Failed-transaction ratio in recent activity
- A weighted risk score with a clear verdict and the action to take

## Run it

Open `index.html` in any browser (phone is fine). It talks directly to the
public Solana RPC (`api.mainnet-beta.solana.com`) — no build step, no server,
no dependencies.

## Why

Built for Nigerian and African Solana users: most first losses come from scam
tokens and risky approvals, not hacks. Explorers show raw data; SolGuard NG
explains it. Part of a Solana Foundation Nigeria Grant application
(Superteam Earn) — see the goal workspace for the application pack.

## Licence

MIT — see LICENSE.
