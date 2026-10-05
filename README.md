# Nido's Home — releases

Public distribution for the Nido's Home desktop app. Source lives elsewhere.

- **App releases** (`v*` tags) carry the updater manifest `latest.json` and the signed bundles. The app's updater reads `releases/latest/download/latest.json`.
- **Component assets** (large data files the app downloads on request, each pinned by SHA-256) are published as **pre-releases** under non-`v*` tags, so they can never become "latest" and hide the updater manifest.
- **The pronunciation helper** (espeak-ng, GPL-3.0-or-later) is built here, unmodified, from its upstream source by `.github/workflows/espeak-ng-macos.yml` — run by hand, publishing nothing itself. Its pre-release carries the program, the exact source tarball it was built from, and `BUILD.txt` with every command.
