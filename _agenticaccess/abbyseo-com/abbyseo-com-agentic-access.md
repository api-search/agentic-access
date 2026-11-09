---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: abbyseo-com-email-results-api-openapi.yml
  format: yaml
  label: Abby SEO Email Results API
  slug: abbyseo-com-email-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abbyseo-com/openapi/abbyseo-com-email-results-api-openapi.yml
- filename: abbyseo-com-scan-api-openapi.yml
  format: yaml
  label: Abby SEO Scan API
  slug: abbyseo-com-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abbyseo-com/openapi/abbyseo-com-scan-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abbyseo Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Abby SEO exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abby SEO
provider_slug: abbyseo-com
slug: abbyseo-com-agentic-access
source_filename: abbyseo-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/abbyseo-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/scan\n  method: get\n  operationId: submitScanGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scan\n  method: post\n  operationId: submitScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan/{scan_id}/status\n  method: get\n  operationId: getScanStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scan/{scan_id}\n  method: get\n  operationId: getScanResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/email-results/{scan_id}\n  method: post\n  operationId: emailResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/abbyseo-com/agentic-access/abbyseo-com-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- SEO
- Audit
- Tool
- Free
- Websites
- Analytics
---
