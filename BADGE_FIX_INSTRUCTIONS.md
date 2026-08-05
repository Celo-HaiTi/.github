# Fix for celoht-smart-contracts/README.md badges

The current README badges point to the wrong org path (`celo-ht` instead of `Celo-HaiTi`), so they can never reflect real build status. Find-and-replace these two lines near the top of `README.md`:

**Find:**
```
[![CI](https://github.com/celo-ht/celoht-smart-contracts/actions/workflows/ci.yml/badge.svg)](.github/workflows/ci.yml)
[![CodeQL](https://github.com/celo-ht/celoht-smart-contracts/actions/workflows/codeql.yml/badge.svg)](.github/workflows/codeql.yml)
```

**Replace with:**
```
[![CI](https://github.com/Celo-HaiTi/celoht-smart-contracts/actions/workflows/ci.yml/badge.svg)](https://github.com/Celo-HaiTi/celoht-smart-contracts/actions/workflows/ci.yml)
[![CodeQL](https://github.com/Celo-HaiTi/celoht-smart-contracts/actions/workflows/codeql.yml/badge.svg)](https://github.com/Celo-HaiTi/celoht-smart-contracts/actions/workflows/codeql.yml)
```

This only works once the `ci.yml` and `codeql.yml` workflow files (included in this package, under `.github/workflows/`) have actually been added to the repo and have run at least once — a badge for a workflow that has never run shows as "no status," not a false pass, so there's no risk of the badge lying in the meantime.

## Important honesty note on CodeQL + Solidity

CodeQL does **not** natively analyze Solidity — the `codeql.yml` included here will scan your JavaScript/TypeScript tooling (tests, scripts, Hardhat config) but not the `.sol` contract logic itself. For actual Solidity security analysis, add **Slither** (free, open-source) as a second workflow:

```yaml
# .github/workflows/slither.yml
name: Slither
on: [pull_request, push]
jobs:
  analyze:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: crytic/slither-action@v0.4.0
```

Neither CodeQL nor Slither is a substitute for the third-party human audit recommended in the main audit report before mainnet deployment — they catch a different, narrower class of issues (common patterns, not business-logic flaws), but both are free and worth having as a first line of defense starting today.
