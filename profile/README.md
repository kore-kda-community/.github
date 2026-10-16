# Welcome to kore-kda-community

Kadena AI ecosystem tools and releases.

## What We Build

AI-focused development (community-based effort) for the Kadena Chainweb blockchain.

## Repositories of Interest

- [`org-bootstrap`](https://github.com/kore-kda-community/org-bootstrap) — Go rewrite: org-bootstrap, org-audit, org-release — one toolchain for GitHub org setup and release pipelines


## Download Builds

Binaries for all projects: **https://github.com/kore-kda-community/releases**

### Homebrew

```bash
brew trust kore-kda-community/tap
brew tap kore-kda-community/tap
brew install <formula>
```

## Getting Help

Open an issue in the relevant repository.

## For Developers: Bootstrap Your Own Org

Running your own org and want the same structure? The tool we use to set this up lives in our shared tooling org:

**[homebrew-tap-app](https://github.com/kore-kda-community/homebrew-tap-app)** — a single script that scaffolds:

- **.github** — org profile README + shared community health files
- **releases** — central hub where every tagged build lands
- **homebrew-tap** — package manager formulae, auto-bumped by CI
- **Source repos** — one per project, with branch layout for project work
- **Release workflow** — GoReleaser config + GitHub Actions; tag -> build -> publish -> formula bump, fully automated
- **Release schedule** — driven by tags, so git tag vX.Y.Z && git push --tags is the whole workflow

Clone it, point it at your org, run ./run.sh. Safe to re-run.

