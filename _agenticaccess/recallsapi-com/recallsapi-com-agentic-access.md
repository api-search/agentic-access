---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 18
api_specs:
- filename: recallsapi-com-account-api-openapi.yml
  format: yaml
  label: recallsapi-com Account API
  slug: recallsapi-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-account-api-openapi.yml
- filename: recallsapi-com-alerts-api-openapi.yml
  format: yaml
  label: recallsapi-com Alerts API
  slug: recallsapi-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-alerts-api-openapi.yml
- filename: recallsapi-com-billing-api-openapi.yml
  format: yaml
  label: recallsapi-com Billing API
  slug: recallsapi-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-billing-api-openapi.yml
- filename: recallsapi-com-catalogs-api-openapi.yml
  format: yaml
  label: recallsapi-com Catalogs API
  slug: recallsapi-com-catalogs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-catalogs-api-openapi.yml
- filename: recallsapi-com-check-api-openapi.yml
  format: yaml
  label: recallsapi-com Check API
  slug: recallsapi-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-check-api-openapi.yml
- filename: recallsapi-com-credits-api-openapi.yml
  format: yaml
  label: recallsapi-com Credits API
  slug: recallsapi-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-credits-api-openapi.yml
- filename: recallsapi-com-health-api-openapi.yml
  format: yaml
  label: recallsapi-com Health API
  slug: recallsapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-health-api-openapi.yml
- filename: recallsapi-com-keys-api-openapi.yml
  format: yaml
  label: recallsapi-com Keys API
  slug: recallsapi-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-keys-api-openapi.yml
- filename: recallsapi-com-mcp-api-openapi.yml
  format: yaml
  label: recallsapi-com MCP API
  slug: recallsapi-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-mcp-api-openapi.yml
- filename: recallsapi-com-recalls-api-openapi.yml
  format: yaml
  label: recallsapi-com Recalls API
  slug: recallsapi-com-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-recalls-api-openapi.yml
- filename: recallsapi-com-receipts-api-openapi.yml
  format: yaml
  label: recallsapi-com Receipts API
  slug: recallsapi-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-receipts-api-openapi.yml
- filename: recallsapi-com-signals-api-openapi.yml
  format: yaml
  label: recallsapi-com Signals API
  slug: recallsapi-com-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-signals-api-openapi.yml
- filename: recallsapi-com-vehicles-api-openapi.yml
  format: yaml
  label: recallsapi-com Vehicles API
  slug: recallsapi-com-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-vehicles-api-openapi.yml
- filename: recallsapi-com-well-known-api-openapi.yml
  format: yaml
  label: recallsapi-com .well Known API
  slug: recallsapi-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recallsapi-com/openapi/recallsapi-com-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Recallsapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 31
overview: 'recallsapi-com exposes 31 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: recallsapi-com
provider_slug: recallsapi-com
slug: recallsapi-com-agentic-access
source_filename: recallsapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/recallsapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 18\n    acting: 13\n  by_consequence:\n    read: 18\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/unsubscribe/{token}\n  method: get\n  operationId: unsubscribePage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/alerts/unsubscribe/{token}\n  method: post\n  operationId: unsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check\n  method: get\n  operationId: checkProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/{id}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/verify\n\
  \  method: post\n  operationId: verifyReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/recallsapi-keys.json\n  method: get\n  operationId: receiptKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/batch\n  method: post\n  operationId: checkProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recalls\n  method: get\n  operationId: searchRecalls\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/{id}\n  method: get\n  operationId: getRecall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: searchSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}\n  method: get\n  operationId: getSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vin}\n  method: get\n  operationId: checkVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles\n  method: get\n \
  \ operationId: checkVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs\n  method: post\n  operationId: createCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{id}/items\n  method: post\n  operationId: addItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{id}/items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/{id}/matches\n  method: get\n  operationId: listMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/{id}/signals\n  method: get\n  operationId: listCatalogSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/{id}/signals/{signalId}/dismiss\n  method: post\n  operationId: dismissCatalogSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/topup\n  method: post\n  operationId: creditTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits\n  method: get\n  operationId: creditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/{id}\n  method: patch\n  operationId: updateCatalogAlertEmail\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{id}\n  method: delete\n  operationId: deleteCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{id}/matches/{itemId}/{recallId}/dismiss\n  method: post\n  operationId: dismissMatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/billing/checkout\n  method: post\n  operationId: checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: billingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/recallsapi-com/agentic-access/recallsapi-com-agentic-access.yml
summary_line: 31 operations · 13 acting
tags:
- Company
- Recall
- E-Commerce
- Safety
- US-Agencies
---
