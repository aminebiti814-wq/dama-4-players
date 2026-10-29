# Dama 4 Players

Four-player Algerian dama on a cross-shaped board, packaged as an Android app.

GitHub Actions builds the app on every push to `main` (or from the Actions tab, "Run workflow").
Download the `dama-4-players` artifact from the finished run:

- `app-release.aab` - upload this to Google Play Console
- `app-debug.apk` - install this directly on a phone to test

Signing uses four repository secrets: `DAMA_KEYSTORE_B64`, `DAMA_KEYSTORE_PASSWORD`, `DAMA_KEY_ALIAS`, `DAMA_KEY_PASSWORD`.
