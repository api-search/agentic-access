---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Opportunities API
  slug: elead-crm-sales-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Customers API
  slug: elead-crm-sales-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Activities API
  slug: elead-crm-sales-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Product Reference Data API
  slug: elead-crm-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elead Crm Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /opportunities/{opportunityId}/email
operation_count: 14
overview: 'Elead exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elead
provider_slug: elead-crm
slug: elead-crm-agentic-access
source_filename: elead-crm-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/elead-crm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 5\n    read: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: post\n  operationId: Customers_CreateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/search\n  method: get\n  operationId: Customers_SearchCustomers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: get\n  operationId: Customers_GetCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: put\n  operationId: Customers_UpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/vehicles\n  method: get\n  operationId: Customers_GetCustomerOwnedVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n\
  \  method: post\n  operationId: Opportunities_CreateOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/search\n  method: get\n  operationId: Opportunities_Search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/searchDelta\n  method: get\n  operationId: Opportunities_SearchDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{opportunityId}/comments\n  method: post\n  operationId: Opportunities_AddComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{opportunityId}/email\n  method: post\n  operationId: Opportunities_SendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/opportunitySources\n  method: get\n  operationId: GetCompanyOpportunitySources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/vehicles/makes\n  method: get\n  operationId: GetVehicleMakes\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: post\n  operationId: Activities_CreateActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/history\n  method: get\n  operationId: Activities_GetHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/agentic-access/elead-crm-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- CRM
- Automotive
- Dealership
- Sales
- Leads
- Fortellis
- CDK Global
---
