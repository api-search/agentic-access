---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: konfetti-account-api-openapi.yml
  format: yaml
  label: konfetti Account API
  slug: konfetti-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-account-api-openapi.yml
- filename: konfetti-auth-api-openapi.yml
  format: yaml
  label: konfetti Auth API
  slug: konfetti-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-auth-api-openapi.yml
- filename: konfetti-catalog-api-openapi.yml
  format: yaml
  label: konfetti Catalog API
  slug: konfetti-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-catalog-api-openapi.yml
- filename: konfetti-checkout-api-openapi.yml
  format: yaml
  label: konfetti Checkout API
  slug: konfetti-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-checkout-api-openapi.yml
- filename: konfetti-requests-api-openapi.yml
  format: yaml
  label: konfetti Requests API
  slug: konfetti-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-requests-api-openapi.yml
consequence_counts:
  physical: 2
  read: 12
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Konfetti Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/cart/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/store/coupon/{code}/validate
operation_count: 21
overview: 'konfetti exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: konfetti
provider_slug: konfetti
slug: konfetti-agentic-access
source_filename: konfetti-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/konfetti-account-api-openapi.yml, openapi/konfetti-auth-api-openapi.yml, openapi/konfetti-catalog-api-openapi.yml,\n  openapi/konfetti-checkout-api-openapi.yml, openapi/konfetti-requests-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 12\n    acting: 9\n  by_consequence:\n    read: 12\n    write: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/user/profile\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/register\n  method: post\n  operationId: registerCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/oauth/token\n  method: post\n  operationId: issueAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/events/{permalink}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/events/{permalink}/similar\n  method: get\n  operationId: listSimilarEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/events/{id}/pricings\n  method: post\n  operationId: calculateEventPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/events/{id}/add-ons\n  method: get\n  operationId: listEventAddOns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/events/{id}/calendar\n  method: get\n  operationId: getEventCalendar\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/categories\n  method: get\n  operationId: listStoreCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/suppliers/{id}/subdomain\n  method: get\n  operationId: getSupplierSubdomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/metrics/{resource}/{id}\n  method: get\n  operationId: recordMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/store/coupon/{code}/validate\n  method: post\n  operationId: validateCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/cart/validate\n  method: post\n  operationId: validateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/events/{id}/subscribe\n  method: post\n  operationId: subscribeToEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/date-requests\n  method: post\n  operationId: createDateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/date-requests/{id}/similar-events\n  method: get\n  operationId: listDateRequestSimilarEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/private-event-requests\n  method: post\n  operationId: createPrivateEventRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/customers/subscribe-newsletter\n  method: post\n  operationId: subscribeNewsletter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/agentic-access/konfetti-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Company
- Marketplace
- Experience
- Booking
- Event
- Workshops
- Ticketing
- Gift Cards
- Travel And Leisure
- Germany
- Commerce
---
