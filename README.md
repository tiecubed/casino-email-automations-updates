# Casino Email Automations — public update channel

This repository distributes Windows x64 application releases and SHA-256 manifests only. The application source is maintained separately.

For each stable `vMAJOR.MINOR.PATCH` release, assets must include exactly:

- `CasinoEmailAutomations.exe`
- `SHA256SUMS.txt` containing the SHA-256 for that exact executable

The app checks this public feed at startup and then every 24 hours while running. It verifies the manifest and downloaded file before replacing the executable. A checksum detects transfer corruption; it is not a code signature.
