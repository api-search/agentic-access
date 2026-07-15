---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Bills API
  slug: bills
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Intervals API
  slug: intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Meters API
  slug: meters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bayou Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Bayou Energy exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bayou Energy
provider_slug: bayou-energy
slug: bayou-energy-agentic-access
source_filename: bayou-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bayou-energy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/bills\n  method: get\n  operationId: getCustomerBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/intervals\n  method: get\n  operationId: getCustomerIntervals\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills\n  method: post\n  operationId: createBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{id}\n  method: get\n  operationId: getBill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{id}\n  method: patch\n  operationId: updateBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{id}/unlock\n\
  \  method: post\n  operationId: unlockBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utilities\n  method: get\n  operationId: listUtilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utilities/{id}\n  method: get\n  operationId: getUtility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/agentic-access/bayou-energy-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Utility Data
- Energy
- Utility Bills
- Interval Data
- Metering
---
