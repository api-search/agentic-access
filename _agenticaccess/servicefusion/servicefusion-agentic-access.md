---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 15
api_specs:
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Customers API
  slug: servicefusion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Contacts API
  slug: servicefusion-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Jobs API
  slug: servicefusion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Estimates API
  slug: servicefusion-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Invoices API
  slug: servicefusion-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Products and Services API
  slug: servicefusion-products-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Payments API
  slug: servicefusion-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Techs and Users API
  slug: servicefusion-techs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Calendar Tasks API
  slug: servicefusion-calendar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
consequence_counts:
  physical: 2
  read: 15
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Servicefusion Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
operation_count: 24
overview: 'Service Fusion exposes 24 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Service Fusion
provider_slug: servicefusion
slug: servicefusion-agentic-access
source_filename: servicefusion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/servicefusion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 15\n    acting: 9\n  by_consequence:\n    read: 15\n    write: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/contacts\n  method: get\n  operationId: listCustomerContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/contacts\n  method: post\n  operationId: createCustomerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates\n  method: get\n  operationId: listEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates\n  method: post\n  operationId: createEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/{id}\n  method: get\n  operationId: getEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method:\
  \ post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /techs\n  method: get\n  operationId: listTechs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /techs/{id}\n  method: get\n  operationId: getTech\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar-tasks\n  method: get\n  operationId: listCalendarTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar-tasks\n  method: post\n  operationId: createCalendarTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/agentic-access/servicefusion-agentic-access.yml
summary_line: 24 operations · 9 acting
tags:
- Field Service Management
- FSM
- Home Services
- Contractors
- Scheduling
- Dispatch
- Invoicing
---
