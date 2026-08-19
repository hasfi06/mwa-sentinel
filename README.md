# MWA Sentinel

Security audit and hardening toolkit for Mobile Wallet Adapter (MWA) integrations across the Solana Mobile ecosystem.

## Problem

Mobile Wallet Adapter (MWA) is the protocol Android dApps use to communicate with Solana wallets via a local socket / deep-link handshake. It's relatively new, many dApp Store apps implement it independently, and there is currently no public checklist, audit tooling, or reference guide to catch common misconfigurations before an app ships.

Common risk areas include:
- Insecure deep-link / intent handling (Android intent spoofing & hijacking)
- Session or signing-request replay
- Insufficient origin validation between dApp and wallet

## What this project delivers

1. **Security audit** of a sample of popular dApp Store apps' MWA integrations, focused on the risk areas above.
2. **Responsible disclosure report** — vendors notified first, then a general public writeup of common misconfiguration patterns (anonymized where appropriate).
3. **Open-source MWA Integration Security Checklist** — a practical, developer-facing guide any team can use to self-review their MWA implementation before dApp Store submission.

## Status

🚧 Early stage — this repo will host the checklist, audit findings summary, and any tooling produced as the work progresses.

## Author

[hasfi06](https://github.com/hasfi06)

## License

MIT
