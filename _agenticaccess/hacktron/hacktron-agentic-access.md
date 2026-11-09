---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 28
api_specs:
- filename: hacktron-rest-api-cost-estimations-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Cost Estimations API
  slug: hacktron-rest-api-cost-estimations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-cost-estimations-api-openapi.yml
- filename: hacktron-rest-api-findings-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Findings API
  slug: hacktron-rest-api-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-findings-api-openapi.yml
- filename: hacktron-rest-api-hfw-api-openapi.yml
  format: yaml
  label: Hacktron REST API - HFW API
  slug: hacktron-rest-api-hfw-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-hfw-api-openapi.yml
- filename: hacktron-rest-api-repos-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Repos API
  slug: hacktron-rest-api-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-repos-api-openapi.yml
- filename: hacktron-rest-api-scans-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Scans API
  slug: hacktron-rest-api-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-scans-api-openapi.yml
consequence_counts:
  read: 28
  safety-critical: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Hacktron Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cost-estimations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cost-estimations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /findings/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /findings/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /findings/{id}/comments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /findings/{id}/comments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /hfw/verdicts/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /hfw/verdicts/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /scans
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /scans
operation_count: 38
overview: 'Hacktron exposes 38 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hacktron
provider_slug: hacktron
slug: hacktron-agentic-access
source_filename: hacktron-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/hacktron-openapi.json, openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    acting: 10\n    connected: 28\n  by_consequence:\n    safety-critical: 10\n    read: 28\n  human_in_the_loop_required: 10\noperations:\n- path: /scans\n  method: post\n  operationId: RestScanController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /scans\n  method: get\n  operationId: RestScanController_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/status\n  method: get\n  operationId: RestScanController_getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/findings/export\n  method: get\n  operationId: RestScanController_exportFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/findings\n  method: get\n  operationId: RestScanController_listScanFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}\n  method: get\n  operationId: RestScanController_getById\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings\n  method: get\n  operationId: RestFindingController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/export\n  method: get\n  operationId: RestFindingController_exportFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/{id}\n  method: patch\n  operationId: RestFindingController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /findings/{id}\n  method: get\n\
  \  operationId: RestFindingController_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/{id}/comments\n  method: post\n  operationId: RestFindingController_addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cost-estimations\n  method: post\n  operationId: RestCostEstimationController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /cost-estimations\n  method: get\n  operationId: RestCostEstimationController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-estimations/{id}\n  method: get\n  operationId: RestCostEstimationController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos\n  method: get\n  operationId: RestRepoController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hfw/verdicts/batch\n  method: post\n  operationId: RestHfwController_getBatchVerdicts\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /hfw/osv/feed\n  method: get\n  operationId: RestHfwController_getOsvFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hfw/verdict/{ecosystem}/{packageName}\n  method: get\n  operationId: RestHfwController_getPackageVerdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hfw/verdict/{ecosystem}/{scope}/{packageName}\n  method: get\n  operationId: RestHfwController_getScopedNpmPackageVerdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans\n  method: post\n  operationId: RestScanController_create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /scans\n  method: get\n  operationId: RestScanController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/status\n  method: get\n  operationId: RestScanController_getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/findings/export\n  method: get\n  operationId: RestScanController_exportFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}/findings\n  method:\
  \ get\n  operationId: RestScanController_listScanFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{id}\n  method: get\n  operationId: RestScanController_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings\n  method: get\n  operationId: RestFindingController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/export\n  method: get\n  operationId: RestFindingController_exportFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/{id}\n  method: patch\n  operationId: RestFindingController_update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /findings/{id}\n  method: get\n  operationId: RestFindingController_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findings/{id}/comments\n  method: post\n  operationId: RestFindingController_addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cost-estimations\n  method: post\n  operationId: RestCostEstimationController_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cost-estimations\n  method: get\n  operationId: RestCostEstimationController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-estimations/{id}\n  method: get\n  operationId: RestCostEstimationController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos\n  method: get\n  operationId: RestRepoController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /hfw/verdicts/batch\n  method: post\n  operationId: RestHfwController_getBatchVerdicts\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /hfw/osv/feed\n  method: get\n  operationId: RestHfwController_getOsvFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hfw/verdict/{ecosystem}/{packageName}\n  method: get\n  operationId: RestHfwController_getPackageVerdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hfw/verdict/{ecosystem}/{scope}/{packageName}\n  method: get\n  operationId:\
  \ RestHfwController_getScopedNpmPackageVerdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/hacktron/agentic-access/hacktron-agentic-access.yml
summary_line: 38 operations · 10 acting · 10 human-in-the-loop
tags:
- Artificial Intelligence
- Automation
- Integration
- IoT
- Enterprise
---
