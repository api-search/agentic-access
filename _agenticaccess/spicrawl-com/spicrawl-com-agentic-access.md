---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 17
api_specs:
- filename: spicrawl-com-batch-api-openapi.yml
  format: yaml
  label: spicrawl-com Batch API
  slug: spicrawl-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-batch-api-openapi.yml
- filename: spicrawl-com-browser-api-openapi.yml
  format: yaml
  label: spicrawl-com Browser API
  slug: spicrawl-com-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-browser-api-openapi.yml
- filename: spicrawl-com-fleet-api-openapi.yml
  format: yaml
  label: spicrawl-com Fleet API
  slug: spicrawl-com-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-fleet-api-openapi.yml
- filename: spicrawl-com-health-api-openapi.yml
  format: yaml
  label: spicrawl-com Health API
  slug: spicrawl-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-health-api-openapi.yml
- filename: spicrawl-com-requests-api-openapi.yml
  format: yaml
  label: spicrawl-com Requests API
  slug: spicrawl-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-requests-api-openapi.yml
- filename: spicrawl-com-scrape-api-openapi.yml
  format: yaml
  label: spicrawl-com Scrape API
  slug: spicrawl-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-scrape-api-openapi.yml
- filename: spicrawl-com-sessions-api-openapi.yml
  format: yaml
  label: spicrawl-com Sessions API
  slug: spicrawl-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-sessions-api-openapi.yml
- filename: spicrawl-com-usage-api-openapi.yml
  format: yaml
  label: spicrawl-com Usage API
  slug: spicrawl-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicrawl-com/openapi/spicrawl-com-usage-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Spicrawl Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/batch/{batchID}/close
operation_count: 27
overview: 'spicrawl-com exposes 27 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 9 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: spicrawl-com
provider_slug: spicrawl-com
slug: spicrawl-com-agentic-access
source_filename: spicrawl-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/spicrawl-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 17\n    acting: 10\n  by_consequence:\n    read: 17\n    write: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/scrape\n  method: get\n  operationId: scrapeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape\n  method: post\n  operationId: scrapePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: batchCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: get\n  operationId: batchList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/{batchID}\n  method: get\n  operationId: batchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/{batchID}/results\n  method: get\n  operationId: batchResults\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/{batchID}/tasks/{seq}/content\n  method: get\n  operationId: batchTaskContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/{batchID}/cancel\n  method: post\n  operationId: batchCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/{batchID}/retry\n  method: post\n  operationId: batchRetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /v1/batch/{batchID}/items\n  method: post\n  operationId: batchAppend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/{batchID}/close\n  method: post\n  operationId: batchClose\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions\n  method: post\n  operationId: sessionsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId: sessionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionID}\n  method: get\n  operationId: sessionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionID}\n  method: delete\n  operationId: sessionsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{sessionID}/context\n  method: get\n  operationId: sessionsGetContext\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionID}/release\n  method: post\n  operationId: sessionsRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/browser\n  method: get\n  operationId: browserConnect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/browser/token\n  method: post\n  operationId: browserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/requests\n  method: get\n  operationId: requestsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests/{id}\n  method: get\n  operationId: requestsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usageGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/summary\n  method: get\n  operationId: usageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/reconciliation\n  method: get\n  operationId: usageReconciliation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workers\n  method: get\n  operationId: fleetListWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: healthReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/spicrawl-com/agentic-access/spicrawl-com-agentic-access.yml
summary_line: 27 operations · 10 acting · 1 human-in-the-loop
tags:
- Company
- Web Scraping
- Data Extraction
- Automation
- Artificial Intelligence
---
