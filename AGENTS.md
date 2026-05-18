# Agent Instructions

- At the end of every code change, run `vp build` so the built files are refreshed for local testing.
- When asked to update the Homebrew tap after a signed macOS build, use the signed zip from `out/make/zip/darwin/arm64/Codiff-darwin-arm64-<version>.zip`, make sure the matching `v<version>` GitHub Release asset exists and downloads from `https://github.com/nkzw-tech/codiff/releases/download/v<version>/Codiff-darwin-arm64-<version>.zip`, update `nkzw-tech/homebrew-tap` (`Casks/codiff.rb`) with the new `version` and SHA-256, then run `brew audit --cask nkzw-tech/tap/codiff` and `brew style --cask nkzw-tech/tap/codiff` through the tapped checkout before pushing.
