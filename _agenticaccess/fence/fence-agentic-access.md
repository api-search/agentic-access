---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: fence-authentication-api-openapi.yml
  format: yaml
  label: Fence Authentication API
  slug: fence-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-authentication-api-openapi.yml
- filename: fence-declaration-monitoring-api-openapi.yml
  format: yaml
  label: Fence Declaration monitoring API
  slug: fence-declaration-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-declaration-monitoring-api-openapi.yml
- filename: fence-documents-api-openapi.yml
  format: yaml
  label: Fence Documents API
  slug: fence-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-documents-api-openapi.yml
- filename: fence-payments-api-openapi.yml
  format: yaml
  label: Fence Payments API
  slug: fence-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-payments-api-openapi.yml
- filename: fence-portfolio-declarations-api-openapi.yml
  format: yaml
  label: Fence Portfolio declarations API
  slug: fence-portfolio-declarations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-portfolio-declarations-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fence Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{deal_id}/payments/bulk
operation_count: 12
overview: 'Fence exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fence
provider_slug: fence
slug: fence-agentic-access
source_filename: fence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/fence-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 6\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/login/access-token\n  method: post\n  operationId: obtainAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/portfolio_declarations/\n  method: post\n  operationId: createPortfolioDeclaration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/portfolio_declarations/{portfolio_declaration_id}/assets\n  method: post\n  operationId: addPortfolioDeclarationAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/portfolio_declarations/{portfolio_declaration_id}/declare\n  method: post\n  operationId: declarePortfolioDeclaration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/declarations\n  method: get\n  operationId: listDeclarationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/declarations\n  method: post\n  operationId: createFastTrackDeclaration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/declarations/{declaration_id}\n  method: get\n  operationId: getDeclarationRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/declarations/{declaration_id}/assets\n  method: get\n  operationId: listDeclarationRunAssets\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/declarations/{declaration_id}/assets/{portfolio_declaration_asset_id}\n  method: get\n  operationId: getDeclarationRunAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{deal_id}/documents\n  method: get\n  operationId: getDocumentUploadStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{deal_id}/documents\n  method: post\n  operationId: registerDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/{deal_id}/payments/bulk\n  method: post\n  operationId: bulkCreatePayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fence/agentic-access/fence-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Company
- Fintech
- Asset-Backed Finance
- Real-Time
---
