# Dama 4 Players

Four-player Algerian dama on a cross-shaped board, packaged as an offline Android app.

GitHub Actions builds the app on every push to `main`, or from the Actions tab
with "Run workflow". Download the `dama-4-players` artifact from a finished run:

- `app-release.aab` - upload this to Google Play Console
- `app-debug.apk` - install this directly on a phone to test

## Signing

Signing uses one repository secret named `DAMA_SIGNING`: a base64 blob holding the
upload keystore and its passwords. Without it the build still runs, but produces an
unsigned bundle that Google Play will not accept.
