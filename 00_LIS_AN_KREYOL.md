# CeloHT — Lis Konplè Fichye Ranpli Yo (Kreyòl)

Chak dosye anba a swiv menm non repo GitHub li ale ladan an. Kopye chak fichye nan repo ki koresponn lan, epi fè yon commit.

---

## 🔴 KRITIK — fè sa yo jodi a

### 1. Lyen ki t ap voye moun sou yon lòt òganizasyon
**Fichye:** `.github/profile/README.md`
**Kote pou mete l:** repo `.github`, nan chemen `profile/README.md`
**Sa l fè:** Ranplase ansyen paj akèy òganizasyon an (ki te gen lyen ki voye sou `github.com/Celo-HT`, yon kont ki pa gen anyen pou wè ak ou) ak yon vèsyon kote "Documentation", "Research", ak "Brand" pwente sou vrè repo `Celo-HaiTi` yo.

### 2. LICENSE ki manke nan repo CeloHT
**Fichye:** `CeloHT/LICENSE`
**Kote pou mete l:** repo `CeloHT`, nan rasin lan (`/LICENSE`)
**Sa l fè:** Badj lan te deja di Apache 2.0 men fichye a pa t egziste. Kounye a li egziste, e li menm tèks ak lòt repo yo pou konsistans.

---

## 🟠 WOULEMENT ENPÒTAN

### 3. Dependabot (siveyans depandans otomatik)
**Fichye:** `.github/.github/dependabot.yml`
**Kote pou mete l:** kopye **nan CHAK repo** kòd (celoht-siteweb, celoht-dapp, celoht-smart-contracts, celoht-docs), nan chemen `.github/dependabot.yml`
**Enpòtan:** Kontrèman ak template issue/PR yo, dependabot.yml PA pwopaje otomatikman soti nan repo `.github` — se pou ou mete l manyèlman nan chak repo.

### 4. CI (tès otomatik lè w push kòd)
**Fichye yo:**
- `celoht-siteweb/.github/workflows/ci.yml`
- `celoht-dapp/.github/workflows/ci.yml`
- `celoht-smart-contracts/.github/workflows/ci.yml`
- `celoht-smart-contracts/.github/workflows/codeql.yml`
- `celoht-smart-contracts/.github/workflows/slither.yml`

**Kote pou mete l:** menm chemen an, nan chak repo ki gen non an.
**Sa l fè:** Kounye a chak fwa yon moun (ou menm oswa yon kontribitè) push kòd, GitHub ap otomatikman verifye li bati epi tès yo pase. Sa se egzakteman sa zouti otomatik envestisè/gran itilize pou premye tès yo — kounye a w ap pase yo.

### 5. Template Issue ak Pull Request
**Fichye yo:**
- `.github/.github/ISSUE_TEMPLATE/bug_report.md`
- `.github/.github/ISSUE_TEMPLATE/feature_request.md`
- `.github/.github/PULL_REQUEST_TEMPLATE.md`
- `.github/.github/CODEOWNERS`

**Kote pou mete l:** nan repo `.github`, egzakteman nan chemen `.github/ISSUE_TEMPLATE/...`, `.github/PULL_REQUEST_TEMPLATE.md`, ak `.github/CODEOWNERS` (remake: se `.github` ki anndan `.github`, pa `Profile` ni `docs` kòm te genyen anvan).
**Enpòtan:** Yon fwa yo nan bon chemen sa a nan repo `.github`, GitHub ap otomatikman pataje yo ak TOUT lòt repo ki pa gen pwòp vèsyon pa yo — sa vle di ou pa oblije kopye yo nan chak repo endividyèlman (kontrèman ak dependabot.yml).

### 6. Lisans konsistan + rezon ki dèyè chwa a
**Fichye yo:** `LICENSING.md`, `celoht-brand/LICENSE`, `celoht-brand/BRAND_USAGE.md`
**Kote pou mete l:** `LICENSING.md` nan repo `.github` (oswa `CeloHT`); `LICENSE` ak `BRAND_USAGE.md` nan repo `celoht-brand`.
**Sa l fè:** Estanda tout repo kòd yo sou Apache 2.0, epi bay `celoht-brand` yon lisans ki fèt pou logo/branding (CC BY 4.0) pito ke MIT ki fèt pou kòd.

### 7. Odit kontra entelijan
**Fichye:** `celoht-smart-contracts/BADGE_FIX_INSTRUCTIONS.md`
**Sa l fè:** Korije badj CI/CodeQL ki te gen move lyen, epi ajoute Slither (zouti gratis pou analize Solidity — CodeQL li menm pa gade Solidity, se yon bagay w dwe konnen).
**⚠️ Sa mwen PA ka fè pou ou:** Yon vrè odit sekirite pa yon moun/konpayi endepandan. Slither ak CodeQL bon pou premye kouch pwoteksyon, men yo pa ranplase yon vrè odit imèn anvan mainnet. Sa a se yon depans/tan reyèl ou dwe planifye ak yon oditè eksteryè.

---

## 🟡 MWAYEN

### 8. CONTRIBUTING.md pou celoht-dapp
**Fichye:** `celoht-dapp/CONTRIBUTING.md` — te sèl repo kote l te manke.

### 9. Premye Issues pou nouvo kontribitè
**Fichye:** `GOOD_FIRST_ISSUES.md` — 10 tikè pare pou ou kopye dirèkteman nan GitHub Issues, tagye `good-first-issue`.

### 10. Premye vèsyon ofisyèl (release)
**Fichye:** `RELEASE_NOTES_v0.1.0_template.md` — enstriksyon egzat + tèks pou tagye `v0.1.0` sou twa repo kòd yo.

### 11. NO_TOKEN_POLICY.md nan celoht-siteweb ak celoht-dapp
**Fichye yo:** `celoht-siteweb/NO_TOKEN_POLICY.md`, `celoht-dapp/NO_TOKEN_POLICY.md`
**Sa l fè:** Yon lyen kout ki voye moun sou vèsyon konplè a nan repo CeloHT, pou moun ki li sèlman youn nan repo sa yo toujou jwenn règ la fasil.

---

## ⚠️ SA MWEN PA KA RANPLI POU OU (bezwen ou menm, oswa yon zouti/moun eksteryè)

Sa yo se bagay yon rapò dokiman pa ka envante — yo mande swa yon desizyon biznis ou menm sèl ka pran, swa yon aksyon sou yon sistèm mwen pa gen aksè ekri ladan (sit web ou, blockchain la), oswa yon ekspètiz espesyalize:

1. **Wiki repo CeloHT a** — swa ranpli l ak kontni reyèl, swa dezaktive l nan Settings repo a. Chwa senp, men se ou ki dwe fè l nan GitHub Settings.
2. **Rezilta PageSpeed/Lighthouse pou celoht.com** — sit la bloke robo otomatik, w ap oblije ale sou pagespeed.web.dev ou menm, kole lyen celoht.com, epi anrejistre rezilta yo tankou yon fichye nan celoht-docs.
3. **Videyo demo dApp la sou testnet** — yon anrejistreman 60 segond ki montre koneksyon wallet → tranzaksyon → konfimasyon. Sa mande w ouvri yon wallet Valora/MiniPay ou menm sou Alfajores testnet.
4. **Adrès trezò piblik la sou chain** — si w vle transparans total (ki koresponn ak politik San-Token an), se ou ki dwe pibliye vrè adrès pòtfèy la; mwen pa ka envante l.
5. **Vrè odit sekirite kontra entelijan yo** — mande yon oditè Solidity endepandan (menm yon revizyon lejè, tankou nan Code4rena, Sherlock, oswa yon freelanser byen kote sou Solidity) anvan mainnet.
6. **Konfimasyon branch-protection/secret-scanning aktive** — Ale nan Settings → Branches ak Settings → Code security nan chak repo, aktive "Require pull request before merging" ak "Secret scanning."

---

## Rezime — sekans rekòmande

1. Jodi a: fè fix #1 ak #2 (yo pran 5 minit total).
2. Semèn sa a: mete fichye #3 rive #7.
3. Semèn pwochèn: #8, #9, #10, #11 + dezaktive/ranpli Wiki a.
4. Mwa pwochen: planifye vrè odit kontra a ak anrejistreman demo a — sa yo se sa envestisè seryè yo mande anvan yo mete lajan.
