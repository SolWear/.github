# Security Policy

SolWear is a hardware wallet prototype. Please treat security issues seriously, even when they affect demo or development paths.

## Supported Surface

This policy covers SolWear organization repositories and prototype components:

- SolWearOS firmware and wallet/signing behavior
- Android companion NFC pairing and signing flows
- Solana transaction construction, signing relay, and broadcast flow
- Desktop service tooling that connects to the device
- Website routes that collect or process user input

## Reporting A Vulnerability

Please do not open a public issue for a vulnerability. Send a private report to the project maintainers with:

- A short summary of the issue
- Affected component or repository
- Reproduction steps or proof of concept
- Expected impact
- Suggested fix, if you have one

We will acknowledge valid reports as quickly as possible and coordinate fixes privately before public disclosure.

## Prototype Boundaries

SolWear is still in prototype form. The current code and hardware should not be treated as production custody infrastructure until the firmware, mobile relay, hardware enclosure, key storage, signing UX, and recovery model have completed independent security review.
