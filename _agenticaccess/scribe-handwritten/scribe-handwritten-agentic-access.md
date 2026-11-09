---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: scribe-handwritten-v0-endpoints-api-openapi.yml
  format: yaml
  label: Scribe Handwritten v0 Endpoints API
  slug: scribe-handwritten-v0-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-v0-endpoints-api-openapi.yml
- filename: scribe-handwritten-v1-endpoints-api-openapi.yml
  format: yaml
  label: Scribe Handwritten v1 Endpoints API
  slug: scribe-handwritten-v1-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-v1-endpoints-api-openapi.yml
- filename: scribe-handwritten-wallet-api-openapi.yml
  format: yaml
  label: Scribe Handwritten Wallet API
  slug: scribe-handwritten-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-wallet-api-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scribe Handwritten Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/campaign/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/campaign/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/on-going-campaign/{orderId}/pause
operation_count: 23
overview: 'Scribe Handwritten exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 11 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scribe Handwritten
provider_slug: scribe-handwritten
slug: scribe-handwritten-agentic-access
source_filename: scribe-handwritten-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/scribe-handwritten-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 14\n    connected: 9\n  by_consequence:\n    write: 11\n    read: 9\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/refresh-token\n  method: post\n  operationId: 586b27b86ad52275152b7639d6c00e39\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-campaigns\n  method: get\n  operationId: b3fda5926098bbcaa12f5bdfca71bfd5\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/create-campaign-id-v2\n  method: post\n  operationId: 8c098f0fe474498c369c89d2ead7efb8\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/add-campaign-v2\n  method: post\n  operationId: c9d5b3ea7b270609508f918abc5b1212\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/edit-campaign-v2\n  method: post\n  operationId: 95a5e238a93b24fcc401864962c1beee\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-campaign-detail\n  method: get\n  operationId: ce7c7b9bdb1f8f7e0d06dad6a3c63e39\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaign-detail\n  method: get\n  operationId: cda2170c74febfe97915933d66a1be5f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/add-sub-account\n  method: post\n  operationId: 04fc6b2ab6ce7d60ea5134ae7cda72ce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/delete-campaign\n  method: post\n  operationId: f4c9938b787c7975f70d7381602b125d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/add-contacts-bulk\n  method: post\n  operationId: da9e42f728c2ce5ae97a973d0d1fc8e5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/add-contacts-bulk\n  method: post\n  operationId: edbb404c86cf130a91866866437d0970\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-preview-image\n  method: post\n  operationId: 4b8c3030537f346046bfcf1caf0e89fe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/update-campaign-name\n  method: put\n  operationId: 609c0897cf8e8f8778bd2f1d49753e4d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/campaign/send\n  method: put\n  operationId: 2c0e3d12b873103a5489bd16906d1ae0\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/on-going-campaign/{orderId}/pause\n  method: post\n  operationId: 9ae414f7b655ebf5720fc865cdd85189\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaign/{orderId}/cancel\n  method: post\n  operationId: 9c2595300957d49f028ed6132b6005d5\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaign-status\n  method: get\n  operationId: aeeb0a513d8fbec0762a9f505179c8f0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/wallet-balance\n  method: get\n  operationId: getWalletBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ongoing-batch-orders\n  method: get\n  operationId: 0a8486e49c9684ac22f833fe3faeeafd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: get\n  operationId: 66daa0a1f3b7f631094d4eb5e3a10fe0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaign-recipients\n  method: get\n  operationId: 157d642656c530a2831d3bb941a60ef3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/preview\n  method: post\n  operationId: dde1fadb097ca69d08a4586cd2529a5f\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{transaction_id}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/scribe-handwritten/agentic-access/scribe-handwritten-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- Company
- Handwriting
- Digital
- Collaboration
- Productivity
---
