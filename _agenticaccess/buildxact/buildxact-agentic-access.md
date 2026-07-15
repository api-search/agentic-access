---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: buildxact-public-api-openapi.yml
  format: yaml
  label: Buildxact Public API
  slug: buildxact-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/openapi/buildxact-public-api-openapi.yml
- filename: buildxact-webhooks-asyncapi.yml
  format: yaml
  label: Buildxact Webhooks
  slug: buildxact-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/asyncapi/buildxact-webhooks-asyncapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buildxact Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Buildxact exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Buildxact
provider_slug: buildxact
slug: buildxact-agentic-access
source_filename: buildxact-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/buildxact-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/auth/refresh-token\n  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates\n  method: get\n  operationId: listEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates\n  method: post\n  operationId: createEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{estimateId}\n  method: get\n  operationId: getEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /estimates/{estimateId}\n  method: patch\n  operationId: updateEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{estimateId}\n  method: delete\n  operationId: deleteEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{estimateId}/items\n  method: get\n  operationId: listEstimateItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/{estimateId}/items\n\
  \  method: post\n  operationId: addEstimateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{estimateId}/items/{itemId}\n  method: get\n  operationId: getEstimateItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/{estimateId}/items/{itemId}\n  method: patch\n  operationId: updateEstimateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{estimateId}/items/{itemId}\n  method:\
  \ delete\n  operationId: deleteEstimateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tax-rates\n  method: get\n  operationId: listTaxRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/agentic-access/buildxact-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Construction
- Residential Construction
- Construction Management
- Estimating
- Takeoffs
- Job Management
- Project Management
- Quoting
- Scheduling
- Purchase Orders
- Invoicing
- Supplier Integration
- Material Pricing
- Builders
- Remodelers
- Trades
- SaaS
- Australia
- Autodesk
---
