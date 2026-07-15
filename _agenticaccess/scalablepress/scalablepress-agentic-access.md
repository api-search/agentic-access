---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 14
api_specs:
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Product API
  slug: scalablepress-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Quote API
  slug: scalablepress-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Order API
  slug: scalablepress-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Event API
  slug: scalablepress-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Design API
  slug: scalablepress-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Mockup API
  slug: scalablepress-mockup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Billing API
  slug: scalablepress-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
consequence_counts:
  physical: 5
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scalablepress Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/billing/invoice/{invoiceId}/pay/paypal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/order/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/order/{orderId}/changeAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/order/{orderId}/reprint
operation_count: 24
overview: 'Scalable Press exposes 24 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 5 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scalable Press
provider_slug: scalablepress
slug: scalablepress-agentic-access
source_filename: scalablepress-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scalablepress-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 14\n    acting: 10\n  by_consequence:\n    read: 14\n    write: 5\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/categories/{categoryId}\n  method: get\n  operationId: listCategoryProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/products/{productId}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/{productId}/availability\n  method: get\n  operationId: getProductAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/{productId}/items\n  method: get\n  operationId: getProductItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/quote\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/quote/bulk\n  method: post\n  operationId: createBulkQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/quote/{orderToken}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/order\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/order/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/order/{orderId}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/order/{orderId}/reprint\n  method: post\n  operationId: reprintOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/order/{orderId}/changeAddress\n  method: post\n  operationId: changeOrderAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/event\n  method: get\n  operationId: queryEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/event/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/design\n  method: post\n  operationId: createDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/design/{designId}\n  method: get\n  operationId: getDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/design/{designId}\n  method: delete\n  operationId: deleteDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/customization\n  method: get\n  operationId: getCustomizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/mockup\n  method: post\n  operationId: createMockup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/billing/invoice\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/invoice/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/billing/invoice/{invoiceId}/pay/paypal\n  method: post\n  operationId: payInvoicePaypal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/agentic-access/scalablepress-agentic-access.yml
summary_line: 24 operations · 10 acting
tags:
- Print on Demand
- Fulfillment
- Apparel
- Custom Printing
- E-Commerce
- Wholesale
---
