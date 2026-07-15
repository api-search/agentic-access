---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Events API
  slug: fingerprint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Events Search API
  slug: fingerprint-events-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Visitors API
  slug: fingerprint-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Related Visitors API
  slug: fingerprint-related-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Smart Signals API
  slug: fingerprint-smart-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Webhooks
  slug: fingerprint-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Sealed Results
  slug: fingerprint-sealed-results
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fingerprint Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Fingerprint exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fingerprint
provider_slug: fingerprint
slug: fingerprint-agentic-access
source_filename: fingerprint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fingerprint-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /events/{request_id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{request_id}\n  method: put\n  operationId: updateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/search\n  method: get\n  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visitors/{visitor_id}\n  method: get\n  operationId: getVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visitors/{visitor_id}\n  method: delete\n  operationId: deleteVisitorData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /related-visitors\n  method: get\n  operationId: getRelatedVisitors\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/agentic-access/fingerprint-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Device Identification
- Fraud Prevention
- Bot Detection
- Smart Signals
- Identity
---
