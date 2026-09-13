# MeshMachine releases

Public Sparkle update feed and signed release builds for [MeshMachine](https://github.com/humbertowgw-maker/meshmachine) (private source repo).

This repo contains **built binaries only** — no application source code. `appcast.xml` is updated automatically by the main repo's `scripts/release-macos.sh`; release `.zip` files are attached to [Releases](https://github.com/humbertowgw-maker/meshmachine-releases/releases).

Each release is signed with an EdDSA key whose private half lives only in the release machine's Keychain and is never committed anywhere. The public half is embedded in the shipped app's `Info.plist` (`SUPublicEDKey`) so Sparkle can verify every update before installing it.
