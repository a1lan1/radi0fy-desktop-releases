# Radi0fy Desktop Releases

Public release artifacts for the Radi0fy macOS desktop app.

This repository is used only for release binaries published from the private `radi0fy-desktop` repository. Source code lives in the private repository.

## Downloads

- [Latest release](https://github.com/a1lan1/radi0fy-desktop-releases/releases/latest)
- Apple Silicon: `Radi0fy-<version>-arm64.dmg`
- Intel: `Radi0fy-<version>-x64.dmg`

## Unsigned build (macOS Gatekeeper)

Current macOS builds are not signed or notarized. After downloading and copying `Radi0fy.app` to `/Applications`, macOS may block the app as an unidentified developer build.

If you trust the official release, run this command in Terminal:

```bash
xattr -dr com.apple.quarantine /Applications/Radi0fy.app
```

Then open Radi0fy normally.

## Notes

- Run the command only for official builds downloaded from this repository's releases.
- When Apple Developer ID signing and notarization are configured in the private build pipeline, this workaround will no longer be needed.
