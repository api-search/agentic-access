---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Eligibility & Coverage API
  slug: eligibility-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Coverage Scan API
  slug: coverage-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Benefits API
  slug: benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Cost Estimation API
  slug: cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Medicaid API
  slug: medicaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
consequence_counts:
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nirvana Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Nirvana Health exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nirvana Health
provider_slug: nirvana
slug: nirvana-agentic-access
source_filename: nirvana-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nirvana-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/discover\n  method: post\n  operationId: discover_v1_discover_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scan\n  method: post\n  operationId: scan_v1_scan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate\n  method: post\n  operationId: estimate_v1_estimate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/medicaid\n  method: post\n  operationId: medicaid_v1_medicaid_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/agentic-access/nirvana-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Healthcare
- Insurance
- Eligibility
- Benefits
- Cost Estimation
- Behavioral Health
---
