---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 13
api_specs:
- filename: monta-openapi.yml
  format: yaml
  label: Monta Charge Points
  slug: charge-points
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Charges and Sessions
  slug: charges-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Teams
  slug: teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Wallets and Transactions
  slug: wallets-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
- filename: monta-openapi.yml
  format: yaml
  label: Monta Tariffs and Plans
  slug: tariffs-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Monta Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /charges/{id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges
operation_count: 17
overview: 'Monta exposes 17 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 2 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Monta
provider_slug: monta
slug: monta-agentic-access
source_filename: monta-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/monta-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 4\n    connected: 13\n  by_consequence:\n    write: 2\n    read: 13\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /auth/token\n  method: post\n  operationId: createAccessTokenWithClientCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/refresh\n  method: post\n  operationId: createAccessTokenWithRefreshToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/information\n  method: get\n  operationId: getAuthInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charge-points\n  method: get\n  operationId: listChargePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charge-points/{id}\n  method: get\n  operationId: getChargePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /afir-charge-points\n  method: get\n  operationId: listAfirChargePoints\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evse/{id}/status\n  method: get\n  operationId: getEvseStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges\n  method: get\n  operationId: listCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges\n  method: post\n  operationId: startCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/{id}\n  method: get\n\
  \  operationId: getCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges/{id}/stop\n  method: post\n  operationId: stopCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /charges/{id}/kwh-consumption\n  method: get\n  operationId: getChargeKwhConsumption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet-transactions\n  method: get\n  operationId: listWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wallet-transactions/{id}\n  method: get\n  operationId: getWalletTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-wallet\n  method: get\n  operationId: getPersonalWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-data-locations\n  method: get\n  operationId: listOpenDataLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /detect-location\n  method: get\n  operationId: detectLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/agentic-access/monta-agentic-access.yml
summary_line: 17 operations · 4 acting · 1 human-in-the-loop
tags:
- EV Charging
- Electric Vehicles
- Charge Points
- Energy
- Mobility
---
