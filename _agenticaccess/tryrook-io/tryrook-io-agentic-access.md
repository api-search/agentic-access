---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: tryrook-io-client-uuid-api-openapi.yml
  format: yaml
  label: ROOK Client Uuid API
  slug: tryrook-io-client-uuid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tryrook-io/openapi/tryrook-io-client-uuid-api-openapi.yml
- filename: tryrook-io-extraction-app-api-openapi.yml
  format: yaml
  label: ROOK Extraction App API
  slug: tryrook-io-extraction-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tryrook-io/openapi/tryrook-io-extraction-app-api-openapi.yml
- filename: tryrook-io-user-id-api-openapi.yml
  format: yaml
  label: ROOK User Id API
  slug: tryrook-io-user-id-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tryrook-io/openapi/tryrook-io-user-id-api-openapi.yml
- filename: tryrook-io-user-profile-api-openapi.yml
  format: yaml
  label: ROOK User Profile API
  slug: tryrook-io-user-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tryrook-io/openapi/tryrook-io-user-profile-api-openapi.yml
- filename: tryrook-io-webhooks-api-openapi.yml
  format: yaml
  label: ROOK Webhooks API
  slug: tryrook-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tryrook-io/openapi/tryrook-io-webhooks-api-openapi.yml
consequence_counts:
  read: 1
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tryrook Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/user_id/{userId}/data_sources/revoke_auth
operation_count: 6
overview: 'ROOK exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ROOK
provider_slug: tryrook-io
slug: tryrook-io-agentic-access
source_filename: tryrook-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/tryrook-io-client-uuid-api-openapi.yml, openapi/tryrook-io-extraction-app-api-openapi.yml,\n  openapi/tryrook-io-user-id-api-openapi.yml, openapi/tryrook-io-user-profile-api-openapi.yml,\n  openapi/tryrook-io-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /client_uuid/$ROOK_CLIENT_UUID/user_id/$USER_ID\n  method: post\n  operationId: post_client_uuid_ROOK_CLIENT_UUID_user_id_USER_ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/extraction_app/binding\n  method: post\n  operationId: post_api_v1_extraction_app_binding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user_id/{userId}/data_source/{dataSource}/authorizer\n  method: get\n  operationId: get_api_v1_user_id_userId_data_source_dataSource_authorizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user_id/{userId}/data_sources/revoke_auth\n  method: post\n  operationId: post_api_v1_user_id_userId_data_sources_revoke_auth\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/user_profile\n  method: post\n  operationId: post_api_v2_user_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/rook\n  method: post\n  operationId: post_webhooks_rook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/tryrook-io/agentic-access/tryrook-io-agentic-access.yml
summary_line: 6 operations · 5 acting · 1 human-in-the-loop
tags:
- Health
- Data Integration
- Wearables
- Healthcare
---
