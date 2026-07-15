---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Bookings & Trips API
  slug: travelperk-bookings-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Invoices API
  slug: travelperk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Expenses API
  slug: travelperk-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Travelers & Members API
  slug: travelperk-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Cost Centers API
  slug: travelperk-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Webhooks API
  slug: travelperk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
consequence_counts:
  read: 11
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Travelperk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'TravelPerk exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TravelPerk
provider_slug: travelperk
slug: travelperk-agentic-access
source_filename: travelperk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/travelperk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 11\n    acting: 9\n  by_consequence:\n    read: 11\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /trips\n  method: get\n  operationId: listTrips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{id}\n  method: get\n  operationId: getTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{trip_id}/custom-fields\n  method: get\n  operationId:\
  \ getTripCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{serial_number}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{serial_number}/pdf\n  method: get\n  operationId: downloadInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/lines\n  method: get\n  operationId: listInvoiceLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles\n  method: get\n  operationId: listInvoiceProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost_centers\n  method: get\n  operationId: listCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost_centers\n  method: post\n  operationId: createCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/bulk_update\n  method: patch\n  operationId: bulkUpdateCostCenters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/{id}\n  method: get\n  operationId: getCostCenter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost_centers/{id}\n  method: patch\n  operationId: updateCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/{id}/users\n  method: put\n  operationId: setCostCenterUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/Users\n  method: post\n  operationId: createScimUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/Users/{id}\n  method: put\n  operationId: replaceScimUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/Users/{id}\n  method: patch\n  operationId: updateScimUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/Schemas/User\n  method: get\n  operationId: getUserSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/agentic-access/travelperk-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- Business Travel
- Travel Management
- Expenses
- Invoices
- Bookings
---
