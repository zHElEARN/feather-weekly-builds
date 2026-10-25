# feather-weekly-builds

Weekly build of [Feather](https://github.com/claration/feather) `main`, published as an
AltStore/Feather source.

## Source

```
https://raw.githubusercontent.com/zHElEARN/feather-weekly-builds/main/app-repo.json
```

## How it runs

- Every Monday 00:00 UTC, or manually via **Actions → Build Feather (Weekly) → Run workflow**
- Skips when `main` has not moved since the last successful build; tick `force` to rebuild anyway
- Publishes a `weekly-YYYY.MM.DD` release and rewrites `app-repo.json` with that single version
- Keeps the last 3 releases

## Output

- `Feather.ipa` — ad-hoc signed by `make iphoneos`; re-sign with your own certificate
- Bundle identifier `thewonderofyou.Feather` (unchanged from upstream)
