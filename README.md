# feather-nightly-builds

GitHub Actions workflow that builds official [claration/Feather](https://github.com/claration/Feather) release tags with the `NIGHTLY` compilation condition enabled, publishes the IPA as a GitHub Release, and updates `app-repo.json`.

## Usage

1. Go to **Actions** → **Build Feather (NIGHTLY) from official Release** → **Run workflow**.
2. The workflow checks the latest official release. If it was already built, it stops; otherwise it builds and publishes a `<official-tag>-nightly` release.
3. Add this source in Feather:

```
https://raw.githubusercontent.com/zHElEARN/feather-nightly-builds/main/app-repo.json
```
