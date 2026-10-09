---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: datacircle-datacircle-api-openapi.yml
  format: yaml
  label: Datacircle Datacircle API
  slug: datacircle-datacircle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-datacircle-api-openapi.yml
- filename: datacircle-harvestapi-api-openapi.yml
  format: yaml
  label: Datacircle Harvest API
  slug: datacircle-harvestapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-harvestapi-api-openapi.yml
- filename: datacircle-up2data-api-openapi.yml
  format: yaml
  label: Datacircle Up2 Data API
  slug: datacircle-up2data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-up2data-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Datacircle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /me/api-key/reset/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/
operation_count: 8
overview: 'Datacircle exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 1 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Datacircle
provider_slug: datacircle
slug: datacircle-agentic-access
source_filename: datacircle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/datacircle-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    safety-critical: 1\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /me/invites/\n  method: get\n  operationId: getInviteLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/api-key/reset/\n  method: post\n  operationId: resetApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /balance/\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/download-link/\n\
  \  method: post\n  operationId: getFileDownloadLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/enrich\n  method: post\n  operationId: enrichLinkedinProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/profile\n  method: get\n  operationId: getLinkedinProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/agentic-access/datacircle-agentic-access.yml
summary_line: 8 operations · 3 acting · 1 human-in-the-loop
tags:
- Company
- B2B Data
- Data Enrichment
- LinkedIn
- Profiles
- MCP
- Data Co-op
---
