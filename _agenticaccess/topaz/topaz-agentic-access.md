---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: topaz-openapi.yml
  format: yaml
  label: Topaz Authorizer API
  slug: topaz-authorizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topaz/refs/heads/main/openapi/topaz-openapi.yml
- filename: topaz-openapi.yml
  format: yaml
  label: Topaz Directory Objects API
  slug: topaz-directory-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topaz/refs/heads/main/openapi/topaz-openapi.yml
- filename: topaz-openapi.yml
  format: yaml
  label: Topaz Directory Relations API
  slug: topaz-directory-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topaz/refs/heads/main/openapi/topaz-openapi.yml
- filename: topaz-openapi.yml
  format: yaml
  label: Topaz Directory Checks API
  slug: topaz-directory-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topaz/refs/heads/main/openapi/topaz-openapi.yml
consequence_counts:
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Topaz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Topaz exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Topaz
provider_slug: topaz
slug: topaz-agentic-access
source_filename: topaz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/topaz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 8\n    connected: 7\n  by_consequence:\n    write: 8\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/authz/is\n  method: post\n  operationId: is\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authz/decisiontree\n  method: post\n  operationId: decisionTree\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authz/query\n  method: post\n  operationId: query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/policies/{id}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v3/directory/object/{object_type}/{object_id}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/directory/object/{object_type}/{object_id}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/directory/objects/{object_type}\n  method: get\n  operationId: getObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/directory/object\n  method: post\n  operationId: setObject\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/directory/relation\n  method: get\n  operationId: getRelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/directory/relation\n  method: post\n  operationId: setRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/directory/relation\n  method: delete\n  operationId: deleteRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/directory/relations\n  method: get\n  operationId: getRelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/directory/check\n  method: post\n  operationId: check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/directory/graph\n  method: get\n  operationId: getGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topaz/refs/heads/main/agentic-access/topaz-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Access Control
- Authorization
- Fine-Grained Authorization
- Open Source
- RBAC
- ReBAC
- Zanzibar
- OPA
- Policy as Code
---
