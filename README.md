# Shui releases

Signed macOS downloads and the Sparkle update feed for Shui.

Shui is under active development. There are no public app releases yet.
Downloads will appear under Releases when the first stable build is ready.

Requirements: Apple Silicon and macOS 26 or newer.
This repository contains distribution assets only; source code is maintained separately.

## Homebrew

After the first stable release is published, install on Apple Silicon with macOS 26 or newer:

```bash
brew tap ichaida/shui-releases https://github.com/ichaida/shui-releases
brew install --cask ichaida/shui-releases/shui
```

The tap's `Casks/shui.rb` appears with the first stable release and is updated
automatically for later stable releases. Downloads use a versioned URL and an
exact SHA-256 checksum for the signed, notarized DMG. No public cask is available yet.

Shui offers in-app updates through Sparkle. To upgrade explicitly with Homebrew,
quit Shui and run:

```bash
brew update
brew upgrade --cask ichaida/shui-releases/shui
```

An ordinary bulk `brew upgrade` skips this self-updating app. Uninstalling leaves
your local conversations, settings, and identity intact.
