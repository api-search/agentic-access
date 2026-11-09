---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 6
api_specs:
- filename: cyberelf-link-catalog-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Catalog API
  slug: cyberelf-link-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-catalog-api-openapi.yml
- filename: cyberelf-link-counterexample-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Counterexample API
  slug: cyberelf-link-counterexample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-counterexample-api-openapi.yml
- filename: cyberelf-link-examples-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Examples API
  slug: cyberelf-link-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-examples-api-openapi.yml
- filename: cyberelf-link-gate-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Gate API
  slug: cyberelf-link-gate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-gate-api-openapi.yml
- filename: cyberelf-link-health-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Health API
  slug: cyberelf-link-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-health-api-openapi.yml
- filename: cyberelf-link-health-report-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Health Report API
  slug: cyberelf-link-health-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-health-report-api-openapi.yml
- filename: cyberelf-link-inspect-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Inspect API
  slug: cyberelf-link-inspect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-inspect-api-openapi.yml
- filename: cyberelf-link-leakage-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Leakage API
  slug: cyberelf-link-leakage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-leakage-api-openapi.yml
- filename: cyberelf-link-mcp-api-openapi.yml
  format: yaml
  label: Cyberelf Labs MCP API
  slug: cyberelf-link-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-mcp-api-openapi.yml
- filename: cyberelf-link-memory-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Memory API
  slug: cyberelf-link-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-memory-api-openapi.yml
- filename: cyberelf-link-open-bench-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Open Bench API
  slug: cyberelf-link-open-bench-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-open-bench-api-openapi.yml
- filename: cyberelf-link-replay-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Replay API
  slug: cyberelf-link-replay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-replay-api-openapi.yml
- filename: cyberelf-link-report-card-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Report Card API
  slug: cyberelf-link-report-card-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-report-card-api-openapi.yml
- filename: cyberelf-link-safepatch-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Safepatch API
  slug: cyberelf-link-safepatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-safepatch-api-openapi.yml
- filename: cyberelf-link-stats-api-openapi.yml
  format: yaml
  label: Cyberelf Labs Stats API
  slug: cyberelf-link-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyberelf-link/openapi/cyberelf-link-stats-api-openapi.yml
consequence_counts:
  read: 6
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cyberelf Link Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Cyberelf Labs exposes 19 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cyberelf Labs
provider_slug: cyberelf-link
slug: cyberelf-link-agentic-access
source_filename: cyberelf-link-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/whetstone.cyberelf.link.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 6\n    acting: 13\n  by_consequence:\n    read: 6\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /api/catalog\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/counterexample\n  method: post\n  operationId: counterexample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/examples\n  method: get\n  operationId: getExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gate\n  method: post\n  operationId: gate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health-report\n  method: post\n  operationId: health\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inspect\n  method: post\n  operationId: inspector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/leakage\n  method: post\n  operationId: leakage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/memory\n  method: post\n  operationId: memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open-bench/leaderboard\n  method: get\n  operationId: openBenchLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open-bench/receipt/{public_id}\n  method: get\n  operationId: openBenchReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open-bench/start\n  method: post\n  operationId: openBenchStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/open-bench/submit\n  method: post\n  operationId: openBenchSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/replay\n  method: post\n  operationId: replay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/report-card/start\n  method: post\n  operationId: reportCardStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/report-card/submit\n  method: post\n  operationId: reportCardSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/safepatch\n  method: post\n  operationId: safepatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method:\
  \ post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cyberelf-link/agentic-access/cyberelf-link-agentic-access.yml
summary_line: 19 operations · 13 acting
tags:
- Company
---
