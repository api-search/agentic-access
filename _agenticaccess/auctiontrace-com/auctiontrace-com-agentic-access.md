---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 16
api_specs:
- filename: auctiontrace-com-buyer-client-api-openapi.yml
  format: yaml
  label: AuctionTrace Buyer Client API
  slug: auctiontrace-com-buyer-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-buyer-client-api-openapi.yml
- filename: auctiontrace-com-buyer-kit-api-openapi.yml
  format: yaml
  label: AuctionTrace Buyer Kit API
  slug: auctiontrace-com-buyer-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-buyer-kit-api-openapi.yml
- filename: auctiontrace-com-catalog-api-openapi.yml
  format: yaml
  label: AuctionTrace Catalog API
  slug: auctiontrace-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-catalog-api-openapi.yml
- filename: auctiontrace-com-datasets-api-openapi.yml
  format: yaml
  label: AuctionTrace Datasets API
  slug: auctiontrace-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-datasets-api-openapi.yml
- filename: auctiontrace-com-healthz-api-openapi.yml
  format: yaml
  label: AuctionTrace Healthz API
  slug: auctiontrace-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-healthz-api-openapi.yml
- filename: auctiontrace-com-human-checkout-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Checkout API
  slug: auctiontrace-com-human-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-checkout-api-openapi.yml
- filename: auctiontrace-com-human-interest-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Interest API
  slug: auctiontrace-com-human-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-interest-api-openapi.yml
- filename: auctiontrace-com-human-offers-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Offers API
  slug: auctiontrace-com-human-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-offers-api-openapi.yml
- filename: auctiontrace-com-human-orders-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Orders API
  slug: auctiontrace-com-human-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-orders-api-openapi.yml
- filename: auctiontrace-com-offer-feedback-api-openapi.yml
  format: yaml
  label: AuctionTrace Offer Feedback API
  slug: auctiontrace-com-offer-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-offer-feedback-api-openapi.yml
- filename: auctiontrace-com-outcome-assessment-api-openapi.yml
  format: yaml
  label: AuctionTrace Outcome Assessment API
  slug: auctiontrace-com-outcome-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-outcome-assessment-api-openapi.yml
- filename: auctiontrace-com-trade-list-api-openapi.yml
  format: yaml
  label: AuctionTrace Trade List API
  slug: auctiontrace-com-trade-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-trade-list-api-openapi.yml
consequence_counts:
  physical: 6
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Auctiontrace Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/human-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/human-checkout/webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/human-orders/{orderId}/assessment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/human-orders/{orderId}/submission
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/offer-feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/outcome-assessment/validate
operation_count: 23
overview: 'AuctionTrace exposes 23 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 1 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AuctionTrace
provider_slug: auctiontrace-com
slug: auctiontrace-com-agentic-access
source_filename: auctiontrace-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/auctiontrace-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 16\n    acting: 7\n  by_consequence:\n    read: 16\n    physical: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buyer-client/README.md\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buyer-kit/README.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/human-offers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade-list/README.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/outcome-assessment/schema\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/outcome-assessment/coverage\n  method: get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/outcome-assessment/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-interest\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/offer-feedback/schema\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v1/offer-feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-checkout/webhook\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-orders/{orderId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/human-orders/{orderId}/assessment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/human-orders/{orderId}/assessment\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-orders/{orderId}/submission\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/human-orders/{orderId}/result\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/human-orders/{orderId}/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/auctiontrace-es-book-pressure-20250729-20260630-v1/manifest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/datasets/auctiontrace-es-book-pressure-20250729-20260630-v1/access\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/auctiontrace-es-book-pressure-20250729-20260630-v1/access/coinbase\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/auctiontrace-com/agentic-access/auctiontrace-com-agentic-access.yml
summary_line: 23 operations · 7 acting
tags:
- Company
- Trading
- Analytics
- Finance
- ES-Strategy
---
