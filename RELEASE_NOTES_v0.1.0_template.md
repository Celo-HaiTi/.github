# How to tag v0.1.0 on a repo (celoht-siteweb, celoht-dapp, celoht-smart-contracts)

```bash
git tag -a v0.1.0 -m "CeloHT [repo-name] v0.1.0 — Foundation phase"
git push origin v0.1.0
```

Then on GitHub: **Releases → Draft a new release → choose the v0.1.0 tag** and paste this, adjusted per repo:

---

## v0.1.0 — Foundation Phase

First tagged release of `[repo-name]`, marking the end of the initial build during CeloHT's Foundation phase (2026 Q2–Q3, see [ROADMAP.md](https://github.com/Celo-HaiTi/celoht-docs/blob/main/ROADMAP.md)).

### Included
- [ list the 3–5 real things that exist right now — e.g. "Wallet connect flow (Valora, MiniPay, WalletConnect)", "AccessManager, EducationRegistry, AgentRegistry, TreeRegistry, DonationVault, ImpactRegistry contracts", "Bilingual (Kreyòl/English) marketing site" ]

### Known limitations
- Not yet audited for mainnet use (contracts) — see `celoht-smart-contracts` security roadmap
- [ any other honest, current limitation ]

### Status
Foundation phase — pre-pilot. See the [Roadmap](https://github.com/Celo-HaiTi/celoht-docs/blob/main/ROADMAP.md) for what "Validation" (next phase) requires before this becomes production/mainnet software.

---

**Why this matters for investors:** a tagged release gives anyone reviewing the project a fixed, citable point in time to reference ("as of v0.1.0...") instead of an ever-changing `main` branch. It costs nothing and is one of the first things a technical reviewer looks for.
