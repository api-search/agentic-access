# agentic-access.apis.io — Agentic Access Index

[**agentic-access.apis.io**](https://apis.io/agentic-access/) indexes a recommended `x-agentic-access` execution contract for every provider across the [APIs.io](https://apis.io) network — the action-class, consequence tier, scope, audience, short-lived token constraints, and human-in-the-loop escalation each operation should carry before it is handed to an AI agent.

**Live site:** [https://apis.io/agentic-access/](https://apis.io/agentic-access/)

Each provider page is generated from that provider's `agentic-access/<slug>-agentic-access.yml` artifact (type `AgenticAccess`), classified from its OpenAPI following [Curity's](https://curity.io) Access Intelligence model (apidays Munich 2026). `method: generated` — a governance starting point, not an authoritative provider claim; audience is bound per deployment. Records refresh on every APIs.io network build.

See the groundwork in `research/curity/agentic-governance/` (vocabulary, OpenAPI Overlay, and Spectral ruleset).
