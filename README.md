# Nido's Home — releases

Public distribution for the Nido's Home desktop app. Source lives elsewhere.

- **App releases** (`v*` tags) carry the updater manifest `latest.json` and the signed bundles. The app's updater reads `releases/latest/download/latest.json`.
- **Component assets** (large data files the app downloads on request, each pinned by SHA-256) are published as **pre-releases** under non-`v*` tags, so they can never become "latest" and hide the updater manifest.
