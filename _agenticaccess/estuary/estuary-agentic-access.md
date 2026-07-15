---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Captures API
  slug: estuary-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Materializations API
  slug: estuary-materializations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Collections API
  slug: estuary-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Catalog Drafts API
  slug: estuary-catalog-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Publications API
  slug: estuary-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Connectors API
  slug: estuary-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Tenants & Billing API
  slug: estuary-tenants-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Auth & Tokens API
  slug: estuary-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Estuary Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /refresh_tokens/{id}
operation_count: 22
overview: 'Estuary exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Estuary
provider_slug: estuary
slug: estuary-agentic-access
source_filename: estuary-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/estuary-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 9\n    connected: 13\n  by_consequence:\n    write: 8\n    read: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /rpc/generate_access_token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refresh_tokens\n  method: get\n  operationId: listRefreshTokens\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refresh_tokens\n  method: post\n  operationId: createRefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refresh_tokens/{id}\n  method: delete\n  operationId: deleteRefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user_grants\n  method: get\n  operationId: listUserGrants\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /role_grants\n  method: get\n  operationId: listRoleGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_specs\n  method: get\n  operationId: listLiveSpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_specs/{id}\n  method: get\n  operationId: getLiveSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_spec_flows\n  method: get\n  operationId: listLiveSpecFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drafts\n  method: get\n  operationId: listDrafts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drafts\n  method: post\n  operationId: createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drafts/{id}\n  method: delete\n  operationId: deleteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /draft_specs\n  method: get\n  operationId: listDraftSpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /draft_specs\n  method: post\n  operationId: upsertDraftSpec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publications\n  method: get\n  operationId: listPublications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publications\n  method: post\n  operationId: createPublication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovers\n  method: post\n  operationId:\
  \ createDiscover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connector_tags\n  method: get\n  operationId: listConnectorTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants\n  method: get\n  operationId: listTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog_stats\n  method: get\n  operationId: listCatalogStats\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rpc/billing_report_202308\n  method: post\n  operationId: billingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/agentic-access/estuary-agentic-access.yml
summary_line: 22 operations · 9 acting · 1 human-in-the-loop
tags:
- Data Integration
- Streaming ETL
- Change Data Capture
- CDC
- Real-Time Data
- Data Pipelines
---
