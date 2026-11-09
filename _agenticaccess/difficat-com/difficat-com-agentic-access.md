---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: difficat-com-balance-api-openapi.yml
  format: yaml
  label: DiffiCat Balance API
  slug: difficat-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-balance-api-openapi.yml
- filename: difficat-com-compares-api-openapi.yml
  format: yaml
  label: DiffiCat Compares API
  slug: difficat-com-compares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-compares-api-openapi.yml
- filename: difficat-com-discover-api-openapi.yml
  format: yaml
  label: DiffiCat Discover API
  slug: difficat-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-discover-api-openapi.yml
- filename: difficat-com-feedback-api-openapi.yml
  format: yaml
  label: DiffiCat Feedback API
  slug: difficat-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-feedback-api-openapi.yml
- filename: difficat-com-jobs-api-openapi.yml
  format: yaml
  label: DiffiCat Jobs API
  slug: difficat-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-jobs-api-openapi.yml
- filename: difficat-com-screenshots-api-openapi.yml
  format: yaml
  label: DiffiCat Screenshots API
  slug: difficat-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-screenshots-api-openapi.yml
- filename: difficat-com-snapshots-api-openapi.yml
  format: yaml
  label: DiffiCat Snapshots API
  slug: difficat-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-snapshots-api-openapi.yml
consequence_counts:
  physical: 5
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Difficat Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compares
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /discover
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /jobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /jobs/recover
operation_count: 17
overview: 'DiffiCat exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DiffiCat
provider_slug: difficat-com
slug: difficat-com-agentic-access
source_filename: difficat-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/difficat-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    physical: 5\n    write: 3\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /discover\n  method: post\n  operationId: discoverPages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenshots\n  method: post\n  operationId: captureScreenshot\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: post\n  operationId: startComparison\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: sendFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/recover\n  method: post\n  operationId: recoverComparison\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getComparison\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/files/{filename}\n  method: get\n  operationId: getScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/cancel\n  method: post\n  operationId: cancelComparison\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snapshots\n  method: get\n  operationId: listSnapshots\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapshots/{id}\n  method: get\n  operationId: getSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapshots/{id}/pages/{n}\n  method: get\n  operationId: getSnapshotPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapshots/{id}/files/{filename}\n  method: get\n  operationId: getSnapshotFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapshots/{id}/compare\n  method: post\n  operationId: compareSnapshotLive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compares\n  method: post\n  operationId: compareSnapshots\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/difficat-com/agentic-access/difficat-com-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Company
- Website Migration
- Visual Regression
- Testing
- QA
- SEO
- MCP
- AI Agents
- x402
---
