# Foundry Relay architecture (Draft 0.1)

**Status: Proposed / Backlog. No implementation has begun.**

## Product
A Windows-first, ad-free, local-first IRC/IRCv3 desktop client with interchangeable Classic Desktop, Cyber-Terminal, and Modern Minimal skins. Future protocol adapters are a design goal, not a V1 promise.

## Proposed stack
- Rust asynchronous core and IRC adapter
- Tauri 2 desktop shell
- TypeScript presentation and skin engine
- SQLite local profiles, messages and preferences
- OS-backed credential storage

## Boundaries
UI -> typed application commands/events -> Relay core -> protocol adapter -> network. The UI must not depend on IRC-specific wire formats. Adapters expose capabilities, and unsupported features must not be simulated. Protocol-specific data can be preserved separately.

## Security and privacy
Validate TLS certificates; support SASL; protect stored credentials; treat remote messages and theme metadata as untrusted; prohibit arbitrary executable theme code in V1; no ads, mandatory account, or behavioral analytics. IRC TLS is not end-to-end encryption.

## Skins
Three built-in presentations share state and commands. Reduced motion, readable contrast and keyboard navigation are required. Third-party executable extensions are deferred.

## Open questions
Final dependency selection, storage retention defaults, IRCv3 feature subset, license selection, plugin sandbox design and supported OS versions remain subject to architecture review.
