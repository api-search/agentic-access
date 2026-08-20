---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: chargebee-customers-api-openapi.yml
  format: yaml
  label: Chargebee Customers API
  slug: chargebee-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-customers-api-openapi.yml
- filename: chargebee-invoices-api-openapi.yml
  format: yaml
  label: Chargebee Invoices API
  slug: chargebee-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-invoices-api-openapi.yml
- filename: chargebee-items-api-openapi.yml
  format: yaml
  label: Chargebee Items API
  slug: chargebee-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-items-api-openapi.yml
- filename: chargebee-orders-api-openapi.yml
  format: yaml
  label: Chargebee Orders API
  slug: chargebee-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-orders-api-openapi.yml
- filename: chargebee-payments-api-openapi.yml
  format: yaml
  label: Chargebee Payments API
  slug: chargebee-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-payments-api-openapi.yml
- filename: chargebee-plans-api-openapi.yml
  format: yaml
  label: Chargebee Plans API
  slug: chargebee-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-plans-api-openapi.yml
- filename: chargebee-quotes-api-openapi.yml
  format: yaml
  label: Chargebee Quotes API
  slug: chargebee-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-quotes-api-openapi.yml
- filename: chargebee-subscriptions-api-openapi.yml
  format: yaml
  label: Chargebee Subscriptions API
  slug: chargebee-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-subscriptions-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chargebee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Chargebee exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chargebee
provider_slug: chargebee
slug: chargebee-agentic-access
source_filename: chargebee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chargebee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: get\n  operationId: retrieveCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscription_id}\n  method: get\n  operationId: retrieveSubscription\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}\n  method: get\n  operationId: retrieveInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items\n  method: get\n  operationId:\
  \ listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: get\n  operationId: listQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/agentic-access/chargebee-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Billing
- Subscription
- Recurring Billing
- Revenue
- Payments
- Software-as-a-Service
---
