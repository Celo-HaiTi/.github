# Production Readiness

**Repository:** `.github`  
**Reviewed:** 2026-09-06

This repository owns organization-level defaults, community health files,
policy references, issue templates, and copyable engineering guidance. It is
not an application, smart-contract package, wallet integration, backend,
indexer, or deployment system.

## IMPLEMENTED

- Canonical current organization links use `Celo-HaiTi`.
- The no-token policy and security reporting guidance are present.
- Issue templates, contribution guidance, Dependabot configuration, and
  repository metadata validation are maintained here.
- The validator checks Markdown fences, local Markdown links, YAML, JSON, and
  no-token funding constraints.
- The repository contains no runtime code, private keys, wallet operations,
  Treasury operations, contract deployment, or production data.
- Ownership metadata is honest: no unverified individual or GitHub team is
  assigned as a CODEOWNER.

## TESTNET READY

Not applicable. This repository has no blockchain runtime or testnet workload.

## PRODUCTION READY

Not applicable. Organization metadata is not a deployed production service.
The files are suitable for their intended repository-health role after local
validation passes.

## PLANNED

- Replace copyable workflow examples with repository-specific workflows in
  each owning repository where needed.
- Add an organization-owned team to CODEOWNERS when that team is formally
  created and verified.

## BLOCKED

- Organization-wide workflow execution is blocked by GitHub's repository
  layout rules: workflow YAML must live in `.github/workflows/` in the target
  repository. Root-level YAML files in this repository are guidance/templates,
  not automatically active organization workflows.
- CODEOWNERS automation is blocked until a maintainer or organization team is
  formally verified and published.
- No backend, indexer, database, or production analytics system is authorized
  by this repository.

## MOCK / DEMO

None.

## HISTORICAL / DEPRECATED

- `Celo-HT` references retained in policy or roadmap text are explicitly
  labeled legacy or historical.
- Alfajores and cUSD are not current CeloHT network or asset standards; current
  guidance uses Celo Sepolia (`11142220`) and USDm.

## Validation

Run:

```bash
bash validate.sh
```

No deployment, secret, private-key, or production infrastructure action is
required or performed by this repository.