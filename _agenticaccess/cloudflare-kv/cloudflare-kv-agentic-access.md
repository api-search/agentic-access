---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare KV REST API
  slug: cloudflare-kv-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/main/openapi.yaml
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudflare Kv Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Cloudflare KV exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudflare KV
provider_slug: cloudflare-kv
slug: cloudflare-kv-agentic-access
source_filename: cloudflare-kv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudflare-kv-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 5\n    acting: 9\n  by_consequence:\n    read: 5\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{account_id}/storage/kv/namespaces\n  method: get\n  operationId: workers-kv-namespace-list-namespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/storage/kv/namespaces\n  method: post\n  operationId: workers-kv-namespace-create-a-namespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}\n  method: delete\n  operationId: workers-kv-namespace-remove-a-namespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}\n  method: get\n  operationId: workers-kv-namespace-get-a-namespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}\n  method: put\n  operationId:\
  \ workers-kv-namespace-rename-a-namespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/bulk\n  method: delete\n  operationId: workers-kv-namespace-delete-multiple-key-value-pairs-deprecated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/bulk\n  method: put\n  operationId: workers-kv-namespace-write-multiple-key-value-pairs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/bulk/delete\n  method: post\n  operationId: workers-kv-namespace-delete-multiple-key-value-pairs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/bulk/get\n  method: post\n  operationId: workers-kv-namespace-get-multiple-key-value-pairs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/keys\n  method: get\n  operationId: workers-kv-namespace-list-a-namespace'-s-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/metadata/{key_name}\n  method: get\n  operationId: workers-kv-namespace-read-the-metadata-for-a-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/values/{key_name}\n  method: delete\n  operationId: workers-kv-namespace-delete-key-value-pair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/values/{key_name}\n  method: get\n  operationId: workers-kv-namespace-read-key-value-pair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/storage/kv/namespaces/{namespace_id}/values/{key_name}\n  method: put\n  operationId: workers-kv-namespace-write-key-value-pair-with-metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-kv/refs/heads/main/agentic-access/cloudflare-kv-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Key-Value Store
- Edge Computing
- Cloudflare Workers
- Distributed Storage
- Global Database
- Cache
- Configuration Management
---
