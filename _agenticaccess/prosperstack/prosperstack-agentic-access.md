---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 20
api_specs:
- filename: prosperstack-customer-portal-api-openapi.yml
  format: yaml
  label: ProsperStack Customer Portal API
  slug: prosperstack-customer-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-customer-portal-api-openapi.yml
- filename: prosperstack-events-api-openapi.yml
  format: yaml
  label: ProsperStack Events API
  slug: prosperstack-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-events-api-openapi.yml
- filename: prosperstack-flow-sessions-api-openapi.yml
  format: yaml
  label: ProsperStack Flow Sessions API
  slug: prosperstack-flow-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-flow-sessions-api-openapi.yml
- filename: prosperstack-flows-api-openapi.yml
  format: yaml
  label: ProsperStack Flows API
  slug: prosperstack-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-flows-api-openapi.yml
- filename: prosperstack-offer-links-api-openapi.yml
  format: yaml
  label: ProsperStack Offer Links API
  slug: prosperstack-offer-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-offer-links-api-openapi.yml
- filename: prosperstack-offers-api-openapi.yml
  format: yaml
  label: ProsperStack Offers API
  slug: prosperstack-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-offers-api-openapi.yml
- filename: prosperstack-payments-api-openapi.yml
  format: yaml
  label: ProsperStack Payments API
  slug: prosperstack-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-payments-api-openapi.yml
- filename: prosperstack-properties-api-openapi.yml
  format: yaml
  label: ProsperStack Properties API
  slug: prosperstack-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-properties-api-openapi.yml
- filename: prosperstack-subscribers-api-openapi.yml
  format: yaml
  label: ProsperStack Subscribers API
  slug: prosperstack-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-subscribers-api-openapi.yml
- filename: prosperstack-subscriptions-api-openapi.yml
  format: yaml
  label: ProsperStack Subscriptions API
  slug: prosperstack-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-subscriptions-api-openapi.yml
- filename: prosperstack-webhooks-api-openapi.yml
  format: yaml
  label: ProsperStack Webhooks API
  slug: prosperstack-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prosperstack/openapi/prosperstack-webhooks-api-openapi.yml
consequence_counts:
  read: 20
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prosperstack Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'ProsperStack exposes 29 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ProsperStack
provider_slug: prosperstack
slug: prosperstack-agentic-access
source_filename: prosperstack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/prosperstack-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 20\n    acting: 9\n  by_consequence:\n    read: 20\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: retrieveEventById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_portal/sessions\n  method:\
  \ post\n  operationId: createCustomerPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flows/{id}\n  method: get\n  operationId: retrieveFlowById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow_sessions\n  method: get\n  operationId: listFlowSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow_sessions/{id}\n  method:\
  \ get\n  operationId: retrieveFlowSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/{id}\n  method: get\n  operationId: retrieveOfferById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offer_links\n  method: get\n  operationId: listOfferLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offer_links\n  method: post\n  operationId: createOfferLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /offer_links/{id}\n  method: get\n  operationId: retrieveOfferLinkById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: get\n  operationId: retrievePaymentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /properties\n  method: post\n  operationId: createProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{id}\n  method: get\n  operationId: retrievePropertyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{id}\n  method: delete\n  operationId: deletePropertyById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers\n  method: get\n\
  \  operationId: listSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{id}\n  method: get\n  operationId: retrieveSubscriberById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{id}\n  method: patch\n  operationId: updateSubscriberById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{id}\n  method: delete\n  operationId: deleteSubscriberById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: get\n  operationId: retrieveSubscriptionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: patch\n  operationId: updateSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: retrieveWebhookById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhookById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/prosperstack/agentic-access/prosperstack-agentic-access.yml
summary_line: 29 operations · 9 acting
tags:
- Company
- Retention
- Subscription
- Analytics
- Software-as-a-Service
---
