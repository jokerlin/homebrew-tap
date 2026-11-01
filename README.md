# jokerlin/homebrew-tap

Homebrew formulae and casks for [Skill Manager](https://github.com/jokerlin/skill-manager).

```sh
brew tap jokerlin/tap
brew trust jokerlin/tap                    # Homebrew 7 and later load third-party taps only after you trust them
brew install --cask skill-manager          # the macOS app (it contains the skm CLI)
brew install skill-manager-cli             # only the skm CLI and TUI (macOS and Linux)
```

| Name | Type | Installs |
| --- | --- | --- |
| `skill-manager` | cask | `Skill Manager.app`. The app updates itself from signed GitHub releases, so `brew upgrade` skips it. |
| `skill-manager-cli` | formula | `skm`. It conflicts with the homebrew-core `skm` (an SSH key manager), because both install a `skm` binary. |

The release workflow in [jokerlin/skill-manager](https://github.com/jokerlin/skill-manager) writes these files with `scripts/homebrew.sh` after each release. Do not edit them by hand: open issues and pull requests in [jokerlin/skill-manager](https://github.com/jokerlin/skill-manager).
