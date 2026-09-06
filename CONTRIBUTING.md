# Contributing to CeloHT

Mèsi paske w enterese kontribye nan CeloHT! / Thank you for wanting to contribute to CeloHT.

## Before you start

- Read the [Code of Conduct](CODE_OF_CONDUCT.md) and [Security Policy](SECURITY.md).
- This repository contains **no token, coin, or financial instrument of its own** — see the org-wide [No-Token Policy](https://github.com/Celo-HaiTi/CeloHT/blob/main/NO_TOKEN_POLICY.md). Contributions that add token/coin functionality will not be accepted.
- Check the relevant repository's open issues tagged `good-first-issue` if this is your first contribution.

## Local setup

Each CeloHT repository documents its own setup and test commands. Do not assume
that a documentation, website, admin, dApp, or smart-contract repository uses
the same toolchain. Read that repository's README before installing dependencies.

## Making a change

1. Fork the repo and create a branch: `git checkout -b fix/short-description`
2. Make your change, with tests where applicable.
3. Run the repository's documented lint, typecheck, build, and test commands before opening a PR.
4. Open a pull request using the template — link the issue it closes.
5. A maintainer will review; expect requested changes on the first pass, that's normal.

## Reporting a bug or requesting a feature

Use the issue templates — they'll show up automatically when you click "New issue."

## Testnet before mainnet

All contract-related contributions must be demonstrated working on Celo Sepolia
(chain ID `11142220`) before being considered for a mainnet-facing change.
