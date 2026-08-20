---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 16
api_specs:
- filename: bigchange-assets-api-openapi.yml
  format: yaml
  label: BigChange Assets API
  slug: bigchange-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-assets-api-openapi.yml
- filename: bigchange-contacts-api-openapi.yml
  format: yaml
  label: BigChange Contacts API
  slug: bigchange-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-contacts-api-openapi.yml
- filename: bigchange-finance-api-openapi.yml
  format: yaml
  label: BigChange Finance API
  slug: bigchange-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-finance-api-openapi.yml
- filename: bigchange-jobs-api-openapi.yml
  format: yaml
  label: BigChange Jobs API
  slug: bigchange-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-jobs-api-openapi.yml
- filename: bigchange-persons-api-openapi.yml
  format: yaml
  label: BigChange Persons API
  slug: bigchange-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-persons-api-openapi.yml
- filename: bigchange-reference-data-api-openapi.yml
  format: yaml
  label: BigChange Reference Data API
  slug: bigchange-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-reference-data-api-openapi.yml
- filename: bigchange-resources-api-openapi.yml
  format: yaml
  label: BigChange Resources API
  slug: bigchange-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-resources-api-openapi.yml
- filename: bigchange-stock-api-openapi.yml
  format: yaml
  label: BigChange Stock API
  slug: bigchange-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-stock-api-openapi.yml
- filename: bigchange-users-api-openapi.yml
  format: yaml
  label: BigChange Users API
  slug: bigchange-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-users-api-openapi.yml
- filename: bigchange-vehicles-api-openapi.yml
  format: yaml
  label: BigChange Vehicles API
  slug: bigchange-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-vehicles-api-openapi.yml
- filename: bigchange-webhooks-api-openapi.yml
  format: yaml
  label: BigChange Webhooks API
  slug: bigchange-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bigchange Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/finance/invoices
operation_count: 28
overview: 'BigChange exposes 28 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BigChange
provider_slug: bigchange
slug: bigchange-agentic-access
source_filename: bigchange-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bigchange-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 16\n    acting: 12\n  by_consequence:\n    read: 16\n    write: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{jobId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}/schedule\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}/start\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}/result\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobTypes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/{contactId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/persons\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/persons\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/finance/invoices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/finance/invoices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/finance/quotes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/finance/quotes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/finance/purchaseOrders\n \
  \ method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stockItems\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stockItems\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/vehicles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-management/v1/assets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset-management/v1/assets\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /webhooks/v1/subscriptions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/v1/failed\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/agentic-access/bigchange-agentic-access.yml
summary_line: 28 operations · 12 acting
tags:
- Field Service Management
- Job Management
- Scheduling
- Workforce Management
- Fleet
- CRM
- Software-as-a-Service
---
