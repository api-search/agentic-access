---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
consequence_counts:
  read: 1
  write: 1
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lamina Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Lamina Labs exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lamina Labs
provider_slug: lamina-labs
slug: lamina-labs-agentic-access
source_filename: lamina-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: mcp/lamina-labs-mcp.yml\nmodel: x-agentic-access (Curity Access Intelligence vocabulary)\ndisclaimer: A governance starting point derived from the provider's published MCP tool\n  annotations and OAuth scopes, not an authoritative provider claim. `audience` is left\n  null to bind per deployment.\nsummary:\n  operations: 2\n  by_action_class: {connected: 1, acting: 1}\n  by_consequence: {read: 1, write: 1}\n  human_in_the_loop: 0\n  audit_required: 1\noperations:\n- operation: simi_get_video\n  surface: mcp\n  scope: jobs:read\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    scope: jobs:read\n    audience: null\n    token: {max-ttl: 3600}\n    audit: optional\n    human-in-the-loop: not-required\n  rationale: Provider annotates this tool readOnlyHint true, idempotentHint true,\n    destructiveHint false. It returns signed media URLs, so the response is sensitive\n    even though the call is read-only.\n\
  - operation: simi_submit_video\n  surface: mcp\n  scope: jobs:create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    scope: jobs:create\n    audience: null\n    token: {max-ttl: 900}\n    audit: required\n    human-in-the-loop: not-required\n  rationale: Creates a billable video generation job. Provider annotates idempotentHint\n    false, so a retry produces a second job; a governing agent should de-duplicate and\n    treat repeat submission as a cost event.\n  cautions:\n  - No idempotency key exists, so at-least-once agent retry semantics will double-charge\n    and double-generate.\n  - openWorldHint is true on both tools; outputs are model-generated video and should not\n    be treated as authoritative content.\nnotes:\n- The provider's authorization server supports dynamic client registration with the\n  `none` token endpoint auth method, so an agent can self-register as a public client.\n  Deployments should constrain which agents may complete that flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamina-labs/refs/heads/main/agentic-access/lamina-labs-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Machine Learning
- Education
- Media
- Model Context Protocol
- Content Generation
---
