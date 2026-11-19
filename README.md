# scoop-bucket

[Scoop](https://scoop.sh) manifests for [meow](https://github.com/ericliswan/termeownal), Instagram DMs in your terminal. Windows support is experimental.

## Install

In PowerShell:

```powershell
scoop install git   # Scoop needs Git to add a bucket; skip if you have it
scoop bucket add ericliswan https://github.com/ericliswan/scoop-bucket
scoop install meow
meow --version
```

No Scoop yet? Install it first, in PowerShell as yourself (not as administrator):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## Update and uninstall

- Update: `scoop update meow`
- Uninstall: run `meow logout --purge` first (it deletes your saved session, its key and the message cache), then `scoop uninstall meow`.

See the [termeownal README](https://github.com/ericliswan/termeownal#installing) for more.

The manifests are written by termeownal's release workflow; don't edit them by hand.
