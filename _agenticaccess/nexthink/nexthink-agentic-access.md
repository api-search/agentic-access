---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: nexthink-nql-api-openapi.json
  format: json
  label: Nexthink NQL API
  slug: nexthink-nql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-nql-api-openapi.json
- filename: nexthink-remote-actions-api-openapi.json
  format: json
  label: Nexthink Remote Actions API
  slug: nexthink-remote-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-remote-actions-api-openapi.json
- filename: nexthink-workflows-openapi.json
  format: json
  label: Nexthink Workflows API
  slug: nexthink-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-workflows-openapi.json
- filename: nexthink-enrichment-api-openapi.json
  format: json
  label: Nexthink Enrichment API
  slug: nexthink-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-enrichment-api-openapi.json
- filename: nexthink-campaigns-api-openapi.json
  format: json
  label: Nexthink Campaigns API
  slug: nexthink-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-campaigns-api-openapi.json
- filename: nexthink-data-management-api-openapi.json
  format: json
  label: Nexthink Data Management API
  slug: nexthink-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-data-management-api-openapi.json
- filename: nexthink-spark-api-openapi.json
  format: json
  label: Nexthink Spark API
  slug: nexthink-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-spark-api-openapi.json
consequence_counts:
  read: 6
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nexthink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Nexthink exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nexthink
provider_slug: nexthink
slug: nexthink-agentic-access
source_filename: nexthink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/nexthink-campaigns-api-openapi.json, openapi/nexthink-data-management-api-openapi.json,\n  openapi/nexthink-enrichment-api-openapi.json, openapi/nexthink-nql-api-openapi.json, openapi/nexthink-remote-actions-api-openapi.json,\n  openapi/nexthink-spark-api-openapi.json, openapi/nexthink-workflows-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/euf/campaign/trigger\n  method: post\n  operationId: triggerCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data-management/device/deletions\n  method: post\n  operationId: deleteDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/data/fields\n  method: post\n  operationId: enrichmentDataFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/nql/execute\n  method: post\n  operationId: execute\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/nql/execute\n  method: post\n  operationId: execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/nql/export\n  method: get\n  operationId: export-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nql/export\n  method: post\n  operationId: export-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/nql/status/{exportId}\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/act/execute\n  method: post\n  operationId: executeRA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/act/remote-action\n  method: get\n  operationId: getAllRemoteActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/act/remote-action/details\n\
  \  method: get\n  operationId: getRemoteActionByNqlId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spark/handoff\n  method: post\n  operationId: handleHandoffRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workflows/execute\n  method: post\n  operationId: executeEA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workflows/execute\n  method: post\n  operationId: executeEAWithExternalIds\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workflows/workflows/{workflowUuid}/execution/{executionUuid}/trigger\n  method: post\n  operationId: triggerThinklet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workflows\n  method: get\n  operationId: getAllWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workflows/details\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/agentic-access/nexthink-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Company
- Business Applications
- Digital Employee Experience
- Endpoint Analytics
- IT Operations
- Automation
- Observability
- DEX
---
