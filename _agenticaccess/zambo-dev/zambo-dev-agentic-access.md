---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 22
api_specs:
- filename: zambo-dev-capabilities-api-openapi.yml
  format: yaml
  label: zambo-dev Capabilities API
  slug: zambo-dev-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-capabilities-api-openapi.yml
- filename: zambo-dev-day-pass-api-openapi.yml
  format: yaml
  label: zambo-dev Day Pass API
  slug: zambo-dev-day-pass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-day-pass-api-openapi.yml
- filename: zambo-dev-discovery-api-openapi.yml
  format: yaml
  label: zambo-dev Discovery API
  slug: zambo-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-discovery-api-openapi.yml
- filename: zambo-dev-geo-api-openapi.yml
  format: yaml
  label: zambo-dev GEO API
  slug: zambo-dev-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-geo-api-openapi.yml
- filename: zambo-dev-handover-api-openapi.yml
  format: yaml
  label: zambo-dev Handover API
  slug: zambo-dev-handover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-handover-api-openapi.yml
- filename: zambo-dev-provibecode-api-openapi.yml
  format: yaml
  label: zambo-dev Provibe Code API
  slug: zambo-dev-provibecode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-provibecode-api-openapi.yml
- filename: zambo-dev-today-api-openapi.yml
  format: yaml
  label: zambo-dev Today API
  slug: zambo-dev-today-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-today-api-openapi.yml
- filename: zambo-dev-universal-api-openapi.yml
  format: yaml
  label: zambo-dev Universal API
  slug: zambo-dev-universal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-universal-api-openapi.yml
- filename: zambo-dev-zambo-api-openapi.yml
  format: yaml
  label: zambo-dev Zambo API
  slug: zambo-dev-zambo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-zambo-api-openapi.yml
- filename: zambo-dev-zambot-api-openapi.yml
  format: yaml
  label: zambo-dev ZAMBOT API
  slug: zambo-dev-zambot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-zambot-api-openapi.yml
- filename: zambo-dev-zambro-api-openapi.yml
  format: yaml
  label: zambo-dev ZAMBRO API
  slug: zambo-dev-zambro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zambo-dev/openapi/zambo-dev-zambro-api-openapi.yml
consequence_counts:
  physical: 2
  read: 22
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Zambo Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/handover/{id}/manage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/today/limits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/day-pass
operation_count: 35
overview: 'zambo-dev exposes 35 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 10 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: zambo-dev
provider_slug: zambo-dev
slug: zambo-dev-agentic-access
source_filename: zambo-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/zambo-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 13\n    connected: 22\n  by_consequence:\n    write: 10\n    read: 22\n    physical: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/zambo\n  method: post\n  operationId: zamboUniversal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zambo\n  method: get\n  operationId: zamboApiDocs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ask\n  method: get\n  operationId: zamboAskGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ask\n  method: post\n  operationId: zamboAskPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/intro\n  method: get\n  operationId: getIntro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/traction\n  method: get\n  operationId: getTraction\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: post\n  operationId: searchCapabilitiesPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/discovery/capabilities.json\n  method: get\n  operationId: getCanonicalCapabilityGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credithunt\n  method: get\n  operationId: creditHuntList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n \
  \ method: post\n  operationId: mcpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zambot\n  method: get\n  operationId: discoverZamboStack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/zambot/spark\n  method: post\n  operationId: zambotSpark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zambot/fix\n  method: post\n  operationId: zambotFix\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zambot/stats\n  method: get\n  operationId: zambotStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/zambro/analyze\n  method: post\n  operationId: zambrosAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/provibe\n  method: post\n  operationId: provibeAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geo/ping\n  method: get\n  operationId: geoPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geo/faq\n  method: get\n  operationId: geoFaq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent402/day-pass\n  method: get\n  operationId: agent402DayPassDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/x402/day-pass\n  method: get\n  operationId: day_pass_challenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/day-pass\n  method: post\n  operationId: day_pass\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/discovery\n  method: get\n  operationId: x402Discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /handover/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/handover/{id}/respond\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/handover/{id}/manage\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/handover/{id}/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/handover/track\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /track/{handle}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/today\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/today/memory\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/today/memory\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/today/limits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/today/limits\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/zambo-dev/agentic-access/zambo-dev-agentic-access.yml
summary_line: 35 operations · 13 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- MCP
- Platform
- AI Tools
- Verifiable Receipts
- Cross‑AI Continuity
---
