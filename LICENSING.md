# CeloHT Licensing Policy

This file explains which license applies where, and why — copy it to the root of the **.github** repo so it's discoverable org-wide, and link to it from every repo's README.

## Code repositories — Apache License 2.0

`celoht-docs`, `CeloHT`, `celoht-research`, `celoht-siteweb`, `celoht-dapp`, `celoht-smart-contracts`

Apache 2.0 is used for all code and documentation repositories because, unlike MIT, it includes an explicit patent grant and patent-retaliation clause. For a project building smart contracts and financial-infrastructure tooling, that patent protection matters more than MIT's slightly shorter text — it protects both CeloHT and anyone who builds on top of it from later patent claims tied to contributed code.

## Brand & creative assets — Creative Commons BY 4.0

`celoht-brand`

Software licenses (MIT, Apache) are written for *code* — they don't cleanly cover a logo, a color palette, or brand guidelines, and using one there creates real ambiguity about what "modify and redistribute" means for a trademark-adjacent asset. CC BY 4.0 is the standard choice for this kind of creative/identity content: it lets people reference and cite the brand (e.g., in press coverage or academic research about CeloHT) while requiring attribution, and it doesn't imply a stranger can freely restyle and reuse the CeloHT logo as if it were open-source code. Pair it with a short **brand usage guide** in the same repo (what's allowed vs. what needs written permission) — CC BY covers copyright, not trademark, so both belong in that repo. `.github` was previously also marked MIT; since it contains no original code, it should switch to Apache 2.0 to match the rest of the org and avoid a second inconsistency.

## Before you change anything

Relicensing after the fact is only simple while you're the sole author (currently true here). Do it now — the longer repos sit with mismatched or missing licenses, the more friction any future co-author or contributor adds to fixing it later, since every contributor whose code is already in the repo would technically need to agree to a license change.

## Action items

1. Add the enclosed `LICENSE` (Apache 2.0) to the `CeloHT` repo — it currently has none despite a badge claiming Apache 2.0.
2. Replace the `LICENSE` in `.github` with Apache 2.0 (was MIT).
3. Replace the `LICENSE` in `celoht-brand` with CC BY 4.0 (was MIT) and add `BRAND_USAGE.md`.
4. Add a one-line "Licensed under Apache 2.0 — see LICENSE" note to every README that doesn't already have one, so it isn't only implied by a badge.
