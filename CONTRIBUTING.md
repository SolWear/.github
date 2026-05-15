# Contributing

Thanks for taking a look at SolWear. The project spans firmware, Android NFC relay, service tooling, website, and hardware assets, so changes should keep the full device flow in mind.

## Working Locally

- Keep changes scoped to the component you are working on.
- Update docs when behavior, hardware assumptions, or setup steps change.
- Avoid committing local device state, build output, credentials, logs, APKs, binaries, or generated caches.
- Treat wallet, signing, NFC, RPC, and flashing paths as security-sensitive.

## Pull Requests

Before opening a pull request, include:

- What changed and why
- How it was tested
- Any hardware used for verification
- Security impact, especially for wallet storage, transaction signing, NFC, device flashing, or website input handling

## Component Checks

Use the checks that match your change:

```bash
# Firmware
idf.py build

# Android
./gradlew assembleDebug

# Website
npm run build
```
