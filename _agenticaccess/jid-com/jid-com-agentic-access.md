---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: jid-com-monitors-api-openapi.yml
  format: yaml
  label: jid-com Monitors API
  slug: jid-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-monitors-api-openapi.yml
- filename: jid-com-qualify-api-openapi.yml
  format: yaml
  label: jid-com Qualify API
  slug: jid-com-qualify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-qualify-api-openapi.yml
- filename: jid-com-screen-api-openapi.yml
  format: yaml
  label: jid-com Screen API
  slug: jid-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-screen-api-openapi.yml
- filename: jid-com-search-api-openapi.yml
  format: yaml
  label: jid-com Search API
  slug: jid-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-search-api-openapi.yml
- filename: jid-com-signal-api-openapi.yml
  format: yaml
  label: jid-com Signal API
  slug: jid-com-signal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-signal-api-openapi.yml
- filename: jid-com-verify-api-openapi.yml
  format: yaml
  label: jid-com Verify API
  slug: jid-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jid-com/openapi/jid-com-verify-api-openapi.yml
consequence_counts:
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jid Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'jid-com exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: jid-com
provider_slug: jid-com
slug: jid-com-agentic-access
source_filename: jid-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/jid-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 9\n    acting: 6\n  by_consequence:\n    read: 9\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: get\n  operationId: searchBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}/verify\n  method: get\n  operationId: verifyBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}\n  method:\
  \ get\n  operationId: getBusinessFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/{receipt_id}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screen\n  method: get\n  operationId: screenGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screen\n  method: post\n  operationId: screen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-check\n  method: post\n  operationId:\
  \ emailCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signal\n  method: get\n  operationId: signal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outcomes\n  method: post\n  operationId: recordOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/results\n  method: get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/qualify\n  method: post\n  operationId: qualifyCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/activities\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/jid-com/agentic-access/jid-com-agentic-access.yml
summary_line: 15 operations · 6 acting
tags:
- Trust
- Artificial Intelligence
- Compliance
- Data
- Verification
---
