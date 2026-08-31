---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 4
api_specs:
- filename: macadress-openapi.yaml
  format: yaml
  label: macadress.com API
  slug: macadresscom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-openapi.yaml
consequence_counts:
  physical: 0
  read: 4
  safety-critical: 0
  write: 0
description: 'Recommended x-agentic-access execution contracts for exposing the macadress.com API to AI agents. Classified from the published OpenAPI plus the provider''s own quota and billing rules. A governance starting point — review and bind audience per deployment.

  '
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Macadress Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'MAC Address Lookup: Find Vendor, OUI & Device Type exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 'MAC Address Lookup: Find Vendor, OUI & Device Type'
provider_slug: macadress
slug: macadress-agentic-access
source_filename: macadress-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: generated\nsource: openapi/macadress-openapi.yaml\ndescription: >\n  Recommended x-agentic-access execution contracts for exposing the macadress.com API to AI\n  agents. Classified from the published OpenAPI plus the provider's own quota and billing\n  rules. A governance starting point — review and bind audience per deployment.\nposture: >\n  This is one of the low-risk shapes: every operation is a read, nothing mutates\n  provider-side state, and the only irreversible consequence of any call is quota spend.\n  That makes the interesting control here ECONOMIC rather than safety-critical. A batch\n  lookup bills per address resolved, so a single agent call can consume 100 lookups, and a\n  free-plan agent can exhaust its whole 1,000-lookup cycle in ten calls with no way to\n  reverse it. Budget caps and retry discipline are the governance surface, not human\n  approval.\nprovider_consent_signals:\n  robots_txt: https://macadress.com/robots.txt\n\
  \  content_signal: 'search=yes, ai-input=yes, ai-train=no'\n  named_agents_allowed: [GPTBot, ChatGPT-User, ClaudeBot, anthropic-ai, Google-Extended, PerplexityBot, CCBot]\n  disallowed_paths: [/admin]\n  llms_txt: https://macadress.com/llms.txt\n  reading: >\n    The provider explicitly permits inference-time agent retrieval and explicitly refuses\n    training use, and it publishes an llms.txt naming its own surfaces. Its llms.txt also\n    states that every /lookup/:mac and /vendor/:id page is safe for an agent to fetch and\n    cite, and asks agents to prefer linking a human to the HTML page over the raw API.\n    Honour the ai-train=no signal: results retrieved here are for answering, not for\n    corpus building.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n    acting: 0\n  by_consequence:\n    read: 4\n    write: 0\n    physical: 0\n    safety-critical: 0\n  human_in_the_loop_required: 0\n  metered_operations: 3\n  unmetered_operations: 1\noperations:\n- path:\
  \ /v1/mac/{mac}\n  method: get\n  operationId: lookupMAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n      note: 'Static API key (mk_ prefix), no expiry issued by the provider; rotate on your own schedule.'\n    cost:\n      billed: true\n      unit: 1 lookup per call\n    audit: none\n- path: /v1/mac/batch\n  method: post\n  operationId: lookupMACBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    cost:\n      billed: true\n      unit: 1 lookup per address resolved, up to 100 per call\n      note: >\n        The highest-cost call on the surface. POST does not mean write here — the method is\n        chosen only because a 100-address list does not fit in a URL — but an agent retry\n        loop on this endpoint is the one way to spend real money against this API.\n    escalation:\n      human-in-the-loop: 'no'\n  \
  \    budget-cap: recommended\n      triggers:\n      - repeated-retry-after-429\n      - batch-volume-above-plan-cycle-fraction\n    audit: recommended\n- path: /v1/vendors\n  method: get\n  operationId: searchVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    cost:\n      billed: true\n      unit: 1 lookup per call\n      note: >\n        Bills as a full lookup even though it returns at most 50 rows and has no cursor.\n        An agent trying to walk the directory by repeated filtered searches will spend\n        heavily and still cannot reach beyond 50 rows per filter; direct it to the static\n        bulk downloads at https://macadress.com/downloads instead.\n    audit: none\n- path: /v1/healthz\n  method: get\n  operationId: healthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    authentication: none\n    token:\n      max-ttl: null\n    cost:\n\
  \      billed: false\n      unit: unmetered\n      note: The only free call on the surface. Safe for an agent to poll before a large job.\n    audit: none\nnon_contract_surface:\n- path: /v1/mac/extract\n  method: post\n  present_in_openapi: false\n  documented_at: https://macadress.com/docs\n  note: >\n    Fully documented but absent from the machine-readable contract, so an agent driven by\n    the OpenAPI or by the MCP tool list cannot discover it. Same read-only, per-address\n    billing profile as the batch endpoint. Recorded here so a governance review sees the\n    whole surface, not just the declared one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/agentic-access/macadress-agentic-access.yml
summary_line: 4 operations
tags:
- Networking
- Network Access Control
- Security
- SecOps
- IoT
- Device Fleet Management
- MDM
- Reference Data
- IEEE OUI Lookup
- Developer Tools
- MCP
- agent-native
---
