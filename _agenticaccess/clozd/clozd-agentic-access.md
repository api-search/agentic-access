---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: clozd-programs-api-openapi.yml
  format: yaml
  label: Clozd /programs API
  slug: clozd-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-api-openapi.yml
- filename: clozd-programs-program-id-competitors-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/competitors API
  slug: clozd-programs-program-id-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-competitors-api-openapi.yml
- filename: clozd-programs-program-id-deals-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals API
  slug: clozd-programs-program-id-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-api-openapi.yml
- filename: clozd-programs-program-id-deals-deal-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/:deal ID API
  slug: clozd-programs-program-id-deals-deal-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-deal-id-api-openapi.yml
- filename: clozd-programs-program-id-deals-import-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/import API
  slug: clozd-programs-program-id-deals-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-import-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints API
  slug: clozd-programs-program-id-touchpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints/:touchpoint ID API
  slug: clozd-programs-program-id-touchpoints-touchpoint-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clozd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Clozd exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clozd
provider_slug: clozd
slug: clozd-agentic-access
source_filename: clozd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/clozd-data-api-v1-openapi.yml, openapi/clozd-data-api-v2-openapi.yml, openapi/clozd-data-api-v3-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 4\n    connected: 8\n  by_consequence:\n    write: 4\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /programs/{program_id}/deals/import\n  method: post\n  operationId: post-deals-op\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /programs/{program_id}/deals/{deal_id}\n\
  \  method: get\n  operationId: get-deal-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/deals\n  method: get\n  operationId: get-deals-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/deals\n  method: post\n  operationId: post-deals-op\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /programs\n  method: get\n  operationId: get-programs-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/competitors\n\
  \  method: get\n  operationId: get-competitors-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/deals/{deal_id}\n  method: get\n  operationId: get-deal-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/deals\n  method: get\n  operationId: get-deals-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/deals\n  method: post\n  operationId: post-deals-op\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /programs/{program_id}/touchpoints/{touchpoint_id}\n  method: get\n  operationId: get-touchpoint-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/touchpoints\n  method: get\n  operationId: get-touchpoints-op\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{program_id}/touchpoints\n  method: post\n  operationId: post-touchpoints-op\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/agentic-access/clozd-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- win-loss-analysis
- customer-feedback
- decision-intelligence
- sales-intelligence
- market-research
- competitive-intelligence
- voice-of-customer
- revenue-intelligence
- saas
- mcp
- agent-native
---
