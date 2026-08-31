# homebrew-tap

Homebrew tap for my command-line tools. The casks here are generated and pushed by
[GoReleaser](https://goreleaser.com) from each tool's own repository on release — edit
them there, not here.

## Install

```sh
brew tap amalucelli/tap
brew install --cask glean statusline steer
```

Or in a single step, without tapping first:

```sh
brew install --cask amalucelli/tap/statusline
```

## Tools

| Cask | Description |
|------|-------------|
| [glean](https://github.com/amalucelli/glean) | Track which files changed since a tool last processed them — incremental work for loops, CI, and agents. |
| [statusline](https://github.com/amalucelli/statusline) | A status line for Claude Code — model, context, session time, token counts, and usage limits. |
| [steer](https://github.com/amalucelli/steer) | A Claude Code hook that steers tool calls toward the right tool — a configurable rule engine over shell-aware payloads. |

The binaries are unsigned, so each cask clears the macOS quarantine attribute on install.

## Upgrade

```sh
brew update && brew upgrade --cask glean statusline steer
```

## License

MIT
