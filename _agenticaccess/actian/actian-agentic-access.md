---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 11
api_specs:
- filename: actian-access-tokens-api-openapi.yml
  format: yaml
  label: Actian Corporation Access Tokens API
  slug: actian-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-access-tokens-api-openapi.yml
- filename: actian-admin-user-api-openapi.yml
  format: yaml
  label: Actian Corporation Admin User API
  slug: actian-admin-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-admin-user-api-openapi.yml
- filename: actian-collections-api-openapi.yml
  format: yaml
  label: Actian Corporation Collections API
  slug: actian-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-collections-api-openapi.yml
- filename: actian-count-api-openapi.yml
  format: yaml
  label: Actian Corporation Count API
  slug: actian-count-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-count-api-openapi.yml
- filename: actian-filters-api-openapi.yml
  format: yaml
  label: Actian Corporation Filters API
  slug: actian-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-filters-api-openapi.yml
- filename: actian-points-api-openapi.yml
  format: yaml
  label: Actian Corporation Points API
  slug: actian-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-points-api-openapi.yml
- filename: actian-scroll-api-openapi.yml
  format: yaml
  label: Actian Corporation Scroll API
  slug: actian-scroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-scroll-api-openapi.yml
- filename: actian-search-api-openapi.yml
  format: yaml
  label: Actian Corporation Search API
  slug: actian-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actian/openapi/actian-search-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Actian Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/admin/reset-password
operation_count: 29
overview: 'Actian Corporation exposes 29 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Actian Corporation
provider_slug: actian
slug: actian-agentic-access
source_filename: actian-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/authentication-api.yaml, openapi/collections-api.yaml, openapi/filters-api.yaml,\n  openapi/points-api.yaml, openapi/search-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 18\n    connected: 11\n  by_consequence:\n    write: 17\n    read: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /auth/api_key\n  method: post\n  operationId: create_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /auth/api_keys\n  method: get\n  operationId: list_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/api_key/{token_id}\n  method: delete\n  operationId: delete_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/api_key/{token_id}/rotate\n  method: post\n  operationId: rotate_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/admin\n  method:\
  \ post\n  operationId: create_admin_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/admin/reset-password\n  method: post\n  operationId: reset_admin_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/admin/login\n  method: post\n  operationId: admin_login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/admin/exists\n  method: get\n  operationId: check_admin_exists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/enabled\n  method: patch\n  operationId: set_auth_enabled\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections\n  method: get\n  operationId: list_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}\n  method: get\n  operationId: get_collection_info\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}\n  method: put\n  operationId: create_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}\n  method: patch\n  operationId: update_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}\n  method: delete\n  operationId: delete_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/exists\n  method: get\n  operationId: collection_exists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filters/examples\n  method: get\n  operationId: filter_examples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/points\n  method: put\n  operationId: upsert_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /collections/{collection_name}/points\n  method: post\n  operationId: get_points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/points/{id}\n  method: get\n  operationId: get_point\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/points/delete\n  method: post\n  operationId: delete_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/vectors\n  method: put\n  operationId: update_vectors\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/payload\n  method: post\n  operationId: set_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/payload\n  method: put\n  operationId: overwrite_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /collections/{collection_name}/points/payload/delete\n  method: post\n  operationId: delete_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/payload/clear\n  method: post\n  operationId: clear_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/search\n  method: post\n  operationId: search_points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /collections/{collection_name}/points/search/batch\n  method: post\n  operationId: search_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/points/scroll\n  method: post\n  operationId: scroll_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_name}/points/count\n  method: post\n  operationId: count_points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/actian/agentic-access/actian-agentic-access.yml
summary_line: 29 operations · 18 acting · 1 human-in-the-loop
tags:
- Company
- Data
- Integration
- Analytics
- Artificial Intelligence
- Enterprise
---
