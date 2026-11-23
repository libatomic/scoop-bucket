# Scoop bucket for Passport

[Scoop](https://scoop.sh) manifests for Passport on Windows (x64 and arm64).

```powershell
scoop bucket add libatomic https://github.com/libatomic/scoop-bucket
scoop install libatomic/passport
```

| App | Description |
|---|---|
| `passport` | Passport desktop: the whole Passport on one computer. `passport up` opens the window (also the Start menu's "Passport"); `passport up --headless` runs without one. |

Upgrade with `scoop update passport`.

The [Passport desktop guide](https://github.com/libatomic/passport-releases/blob/master/docs/README.md) covers first launch, the command line, agents and CI.

Downloads come from [libatomic/passport-releases](https://github.com/libatomic/passport-releases). Manifests are written by Passport desktop's release workflow on each release; edits here are replaced by the next one.

Windows builds are not signed yet, so SmartScreen may ask before the first run. With Passport running, `passport trust` adds its local certificate, which is only good for `.localhost` addresses, to your trusted roots; Windows asks you to confirm.
