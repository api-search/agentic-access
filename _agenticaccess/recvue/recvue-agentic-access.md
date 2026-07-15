---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Revenue Recognition API
  slug: recvue-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Billing API
  slug: recvue-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Billing Schedules API
  slug: recvue-billing-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Orders API
  slug: recvue-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Usage and Deliveries API
  slug: recvue-usage-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Pricing API
  slug: recvue-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Customers and Accounts API
  slug: recvue-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Invoices and Adjustments API
  slug: recvue-invoices-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
consequence_counts:
  physical: 5
  read: 8
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Recvue Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orders/{orderId}/terminate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/activate
operation_count: 21
overview: 'RecVue exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 7 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RecVue
provider_slug: recvue
slug: recvue-agentic-access
source_filename: recvue-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/recvue-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 13\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n    physical: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/scim/oauth/token\n  method: post\n  operationId: issueAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}\n  method: put\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/activate\n  method: post\n  operationId: activateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/terminate\n  method:\
  \ post\n  operationId: terminateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billruns\n  method: get\n  operationId: getBillRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billruns\n  method: post\n  operationId: createBillRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billingschedules\n  method: get\n  operationId: getBillingSchedules\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billingschedules\n  method: post\n  operationId: createBillingSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricelists\n  method: get\n  operationId: getPriceLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/batches\n  method: post\n  operationId: loadUsageBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /deliveries\n  method: get\n  operationId: getDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: getCustomerAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomerAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /revenue/contract-amendment-setup\n  method: get\n  operationId: getRevenueContractAmendmentSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /revenue/contract-amendment-setup\n  method: post\n  operationId: createRevenueContractAmendmentSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /programs/execute\n  method: post\n  operationId: executeConcurrentProgram\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/agentic-access/recvue-agentic-access.yml
summary_line: 21 operations · 13 acting · 1 human-in-the-loop
tags:
- Revenue Recognition
- ASC 606
- Billing
- Order-to-Cash
- Revenue Management
- Usage-Based Billing
- Partner Settlements
- IFRS 15
- Subscription Billing
- Enterprise
---
