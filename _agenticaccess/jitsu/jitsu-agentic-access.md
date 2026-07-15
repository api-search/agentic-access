---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Event Ingestion API (Track / Identify / Page)
  slug: event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Bulk / Batch API
  slug: bulk-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Configuration / Management
  slug: configuration-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
consequence_counts:
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jitsu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Jitsu exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jitsu
provider_slug: jitsu
slug: jitsu-agentic-access
source_filename: jitsu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jitsu-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/s/{type}\n  method: post\n  operationId: ingestEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/s/s2s/{type}\n  method: post\n  operationId: ingestServerEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: ingestBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/s/bulk\n  method: post\n  operationId: ingestBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/agentic-access/jitsu-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Event Data
- CDP
- Data Pipeline
- Analytics
- Open Source
- Ingestion
---
