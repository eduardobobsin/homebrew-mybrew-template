# mybrew instance

Homebrew bottles for Intel Macs on macOS Sequoia, built on demand by
[mybrew](https://github.com/eduardobobsin/mybrew) for formulae that no longer ship one.

**Setup:** name this repository `homebrew-mybrew`, keep it public, then follow
[docs/SETUP.md](https://github.com/eduardobobsin/mybrew/blob/main/docs/SETUP.md).

```bash
brew tap <you>/mybrew && brew trust --tap <you>/mybrew
brew install <you>/mybrew/mybrew
mybrew install <formula>
```

This repository holds state only: `Formula/` (built formulae with their bottle blocks),
`registry/bottles.json` (what has been built) and the build workflow. All behavior lives in the
engine, pinned in `.github/workflows/build.yml`.
