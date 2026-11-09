---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: logo-dev-account-api-openapi.yml
  format: yaml
  label: Logo.dev Account API
  slug: logo-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-account-api-openapi.yml
- filename: logo-dev-brands-api-openapi.yml
  format: yaml
  label: Logo.dev Brands API
  slug: logo-dev-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-brands-api-openapi.yml
- filename: logo-dev-flags-api-openapi.yml
  format: yaml
  label: Logo.dev Flags API
  slug: logo-dev-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-flags-api-openapi.yml
- filename: logo-dev-logo-cdn-api-openapi.yml
  format: yaml
  label: Logo.dev Logo CDN API
  slug: logo-dev-logo-cdn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logo-cdn-api-openapi.yml
- filename: logo-dev-logos-api-openapi.yml
  format: yaml
  label: Logo.dev Logos API
  slug: logo-dev-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logos-api-openapi.yml
- filename: logo-dev-search-api-openapi.yml
  format: yaml
  label: Logo.dev Search API
  slug: logo-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-search-api-openapi.yml
- filename: logo-dev-subscriptions-api-openapi.yml
  format: yaml
  label: Logo.dev Subscriptions API
  slug: logo-dev-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-subscriptions-api-openapi.yml
- filename: logo-dev-transaction-enrichment-api-api-openapi.yml
  format: yaml
  label: Logo.dev Transaction Enrichment API
  slug: logo-dev-transaction-enrichment-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-transaction-enrichment-api-api-openapi.yml
- filename: logo-dev-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Logo.dev Webhook endpoints API
  slug: logo-dev-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-webhook-endpoints-api-openapi.yml
consequence_counts:
  read: 17
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Logo Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Logo.dev exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Logo.dev
provider_slug: logo-dev
slug: logo-dev-agentic-access
source_filename: logo-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/logo-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /{domain}\n  method: get\n  operationId: getLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /name/{brand}\n  method: get\n  operationId: getLogoByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticker/{ticker}\n  method: get\n  operationId:\
  \ getLogoByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /isin/{isin}\n  method: get\n  operationId: getLogoByIsin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crypto/{symbol}\n  method: get\n  operationId: getLogoByCrypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/{exchange}\n  method: get\n  operationId: getLogoByExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index/{symbol}\n  method: get\n  operationId: getLogoByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /transaction\n  method: post\n  operationId: identifyMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/brands\n  method: get\n  operationId: v2GetBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/brands/{id}\n  method: get\n  operationId: v2GetBrandById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/brands/logo\n  method: get\n  operationId: v2GetBrandLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/brands/brandmark\n  method: get\n  operationId: v2GetBrandBrandmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search\n  method: get\n  operationId: v2SearchBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/brands/{id}/subscription\n  method: get\n  operationId: v2GetBrandSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/brands/{id}/subscription\n  method: put\n  operationId: v2SubscribeToBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/brands/{id}/subscription\n  method: delete\n  operationId: v2UnsubscribeFromBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook_endpoints\n  method: post\n  operationId: v2CreateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook_endpoints\n  method: get\n  operationId: v2ListWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/webhook_endpoints/{id}\n  method: get\n  operationId: v2GetWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook_endpoints/{id}\n  method: patch\n  operationId: v2UpdateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook_endpoints/{id}\n  method: delete\n  operationId: v2DeleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/webhook_endpoints/{id}/secret\n  method: get\n  operationId: v2GetWebhookEndpointSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook_endpoints/{id}/secret\n  method: post\n  operationId: v2RotateWebhookEndpointSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account\n  method: get\n  operationId: v2GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flag\n  method: post\n  operationId: v2Flag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/logo-dev/agentic-access/logo-dev-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Logo
- Branding
- CDN
- Free Tier
---
