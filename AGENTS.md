# Portfobit Public Documentation Instructions

## Public Repository Boundary

- This repository is public. Do not add private repository paths, internal network
  topology, credentials, tokens, keys, undisclosed domains, user data, or
  unreleased product plans.
- Document only behavior that is shipped or explicitly being prepared for public
  release. Do not present prototypes, drafts, or internal implementation details
  as current capabilities.
- Keep this repository self-contained. Documentation, validation, and builds must
  not read files from local sibling repositories.

## Product And API Rules

- The current public product is crypto-only and CEX-first.
- Portfobit never supports withdrawals, transfers to external addresses, or P2P
  transfers.
- CEX orders and same-exchange internal transfers are protected operations.
  Documentation must state the explicit user-confirmation and trading-OTP
  authorization requirements.
- `openapi/portfobit-openapi.yaml` is this repository's local contract for the
  published REST API and must remain consistent with the prose API reference.
- When changing navigation, links, or paths, verify that every public entry point
  remains reachable.

## Validation

- Check `git status` before editing and preserve unrelated work.
- Use the validation command documented in `README.md#local-preview` before
  committing.
- Run `git diff --check`, then review the diff for local absolute paths and
  sensitive information.
