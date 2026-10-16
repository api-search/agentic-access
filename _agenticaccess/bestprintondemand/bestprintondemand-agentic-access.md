---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: bestprintondemand-account-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Account API
  slug: bestprintondemand-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-account-api-openapi.yml
- filename: bestprintondemand-batches-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Batches API
  slug: bestprintondemand-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-batches-api-openapi.yml
- filename: bestprintondemand-gender-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Gender API
  slug: bestprintondemand-gender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-gender-api-openapi.yml
- filename: bestprintondemand-webhooks-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Webhooks API
  slug: bestprintondemand-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-webhooks-api-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bestprintondemand Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'BestPrintOnDemand exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BestPrintOnDemand
provider_slug: bestprintondemand
slug: bestprintondemand-agentic-access
source_filename: bestprintondemand-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: generated\nsource: openapi/bestprintondemand-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches/{batch}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches/{batch}\n  method: delete\n  operationId: deleteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batches/{batch}/result\n  method: get\n  operationId: downloadBatchResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches/{batch}/start\n  method: post\n  operationId: startBatch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gender\n  method: get\n  operationId: getName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gender\n  method: post\n  operationId: postName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gender/bulk\n  method: post\n  operationId: bulkGender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gender/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gender/countries\n  method: post\n  operationId: postCountries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gender/email\n  method: get\n  operationId: getEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gender/email\n  method: post\n  operationId:\
  \ postEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gender/username\n  method: get\n  operationId: getUsername\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gender/username\n  method: post\n  operationId: postUsername\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/agentic-access/bestprintondemand-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Company
- API
- Print-on-Demand
- Pricing
- OpenAPI
---
