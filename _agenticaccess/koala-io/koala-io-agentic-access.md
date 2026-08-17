---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: koala-io-accounts-api-openapi.yml
  format: yaml
  label: Koala Accounts API
  slug: koala-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-accounts-api-openapi.yml
- filename: koala-io-collection-api-openapi.yml
  format: yaml
  label: Koala Collection API
  slug: koala-io-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-collection-api-openapi.yml
- filename: koala-io-deletion-api-openapi.yml
  format: yaml
  label: Koala Deletion API
  slug: koala-io-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-deletion-api-openapi.yml
- filename: koala-io-sdk-api-openapi.yml
  format: yaml
  label: Koala SDK API
  slug: koala-io-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-sdk-api-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Koala Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /batch
operation_count: 7
overview: 'Koala exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 3 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Koala
provider_slug: koala-io
slug: koala-io-agentic-access
source_filename: koala-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/koala-io-account-ingestion-api-openapi.yml, openapi/koala-io-accounts-api-openapi.yml,\n  openapi/koala-io-collection-api-openapi.yml, openapi/koala-io-deletion-api-openapi.yml, openapi/koala-io-profile-ingestion-api-openapi.yml,\n  openapi/koala-io-sdk-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    physical: 2\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/batch\n  method: post\n  operationId: sendAccountBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/projects/{publicApiKey}/accounts/batch\n  method: post\n  operationId: collectAccountBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/projects/{publicApiKey}/batch\n  method: post\n  operationId: collectBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deletion-requests\n  method: post\n\
  \  operationId: createDeletionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deletion-requests/{deletionRequestId}\n  method: get\n  operationId: getDeletionRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch\n  method: post\n  operationId: sendProfileBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/projects/{publicApiKey}\n\
  \  method: get\n  operationId: getProjectBootstrap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/agentic-access/koala-io-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Buyer Intent
- Visitor Identification
- De-anonymization
- Enrichment
- Go-to-Market
- Sales Intelligence
- B2B
---
