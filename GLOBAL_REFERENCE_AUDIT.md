# Global Reference Audit

## Canonical vocabulary

- Active project: `CeloHT`
- Canonical GitHub organization: `Celo-HaiTi`
- Canonical currency terminology: `USDm`

## Enforcement rule

CURRENT CORPUS REQUIREMENT:

The current editable repository corpus must use only canonical active
terminology. Obsolete terminology must not be retained merely because it
appears in historical context. Immutable Git history is excluded from this
requirement.

Historical Git history may retain obsolete terminology, but current editable
files must follow the canonical vocabulary.

The audit treats these as current corpus violations:

- `cUSD`
- `Celo-HT`
- `github.com/Celo-HT/` and `github.com/Celo-HT`

They are not acceptable merely because they occur in a historical note,
migration note, changelog, example, URL, generated document, or compatibility
description. Rewrite current visible content to use `USDm`, `CeloHT`, and
`Celo-HaiTi` as appropriate. Do not invent history or compatibility claims.

## Immutable history

Immutable Git history may contain old terminology because rewriting Git history
is outside normal documentation cleanup. This includes old commits, commit
messages, immutable commit hashes, and historical Git objects.

## Current editable corpus

The current editable corpus includes current README files, Markdown, source,
documentation, configuration, website content, examples, links, navigation,
tables, text diagrams, changelogs, and generated documentation whose source can
be corrected. It must contain zero obsolete visible terminology.

The two enforcement manifests, `CANONICAL_IDENTITY.md` and
`GLOBAL_REFERENCE_AUDIT.md`, are policy metadata and necessarily declare the
patterns they prohibit. The validator excludes only those manifests from its
content scan; every other current editable file is scanned.

## Audit procedure

For every match, record the repository, file, line, exact text, and semantic
category before editing. Check whether a URL target exists before changing a
link. In particular, the verified smart-contract repository URL is:

`https://github.com/Celo-HaiTi/celoht-smart-contracts`

Do not replace, remove, rename, or alter `CeloHT` or `Celo-HaiTi`.
Do not rewrite immutable Git history.