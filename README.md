# Scoop bucket for Passport

[Scoop](https://scoop.sh) manifests for Passport on Windows (x64 and arm64).

```powershell
scoop bucket add libatomic https://github.com/libatomic/scoop-bucket
scoop install libatomic/passport
```

| App | Description |
|---|---|
| `passport` | Passport desktop: the whole Passport on one computer. `passport up --headless` runs it; the window (`passport-desktop`, Start menu "Passport") is a preview on Windows. |

Upgrade with `scoop update passport`.

Downloads come from [libatomic/passport-releases](https://github.com/libatomic/passport-releases). Manifests are written by Passport desktop's release workflow on each release; edits here are replaced by the next one.

Windows builds are not signed yet, so SmartScreen may ask before the first run. Trusting Passport's local certificate automatically is macOS only for now: import the file `passport ca --path` prints into your browser.
