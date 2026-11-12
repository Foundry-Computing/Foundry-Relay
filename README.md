# Foundry Relay

**Classic internet soul. Modern capabilities. Your client, your rules.**

> **Project status: Backlog · Concept Draft 0.1 · Not in active development**

Foundry Relay is a proposed free, ad-free, local-first desktop IRC client from Foundry Computing. The vision is to bring back the personality of classic mIRC-era chat while offering modern usability, security and interchangeable skins.

## The experience

- **Classic Desktop:** nostalgic menus, beveled controls and channel windows
- **Cyber-Terminal:** keyboard-first interface, phosphor-inspired styling and optional CRT effects
- **Modern Minimal:** accessible, focused everyday chat

All three skins will share the same conversations, settings and underlying client state.

## Proposed V1.0

Windows-first IRC/IRCv3 client with multiple connections, TLS, SASL, reconnect, channels, private messages, common IRC commands, local history/search, notifications, keyboard shortcuts and three built-in skins.

**Proposed architecture:** Rust core + Tauri 2 + TypeScript UI + SQLite. The architecture is under review, not yet implemented.

## Future direction

A capability-aware adapter system could eventually connect to Matrix and other services through supported APIs. Full Discord user-client access is **not** promised. Optional FORGE integration may be explored later.

## Why this exists

Chat software should be personal, customizable and useful without requiring advertising, tracking or an account with the software vendor. Relay aims to give users control over their interface while connecting to communities on independently operated networks.

## Get involved

We welcome thoughtful issues, design feedback, architecture review and documentation contributions while the project remains in the backlog. **Please do not begin major implementation work or submit large code PRs until a development packet is opened.**

- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)
- [Code of conduct](CODE_OF_CONDUCT.md)

## License

**License selection is pending.** A public repository is not automatically open-source licensed. The project intends to choose an open-source license before implementation and external code contributions begin.

© Foundry Computing. Planning materials are published for discussion; no additional reuse license has yet been granted.
