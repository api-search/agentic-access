---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Transactions API
  slug: wompi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Tokenization API
  slug: wompi-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Sources API
  slug: wompi-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi PSE API
  slug: wompi-pse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Links API
  slug: wompi-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Merchants & Acceptance Tokens API
  slug: wompi-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
consequence_counts:
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Payment writes (transactions, voids, payment sources, payment links) move money and are high-consequence; keep human-in-the-loop and short token TTLs. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Wompi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Wompi exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 6 write.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wompi
provider_slug: wompi
slug: wompi-agentic-access
source_filename: wompi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/wompi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Payment writes (transactions, voids, payment sources, payment links)\n  move money and are high-consequence; keep human-in-the-loop and short token TTLs.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 6\n    connected: 5\n  by_consequence:\n    write: 6\n    read: 5\n  human_in_the_loop_required: 3\noperations:\n- path: /merchants/{public_key}\n  method: get\n  operationId: getMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/cards\n  method: post\n  operationId: tokenizeCard\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - sensitive-data\n    audit: required\n- path: /tokens/nequi\n  method: post\n  operationId: tokenizeNequi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - sensitive-data\n    audit: required\n- path: /tokens/nequi/{token_id}\n  method: get\n  operationId: getNequiToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_sources\n  method: post\n  operationId: createPaymentSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - high-value\n      - recurring-mandate\n    audit: required\n- path: /transactions\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}/void\n  method: post\n  operationId: voidTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: required\n      triggers:\n      - money-movement\n      - reversal\n    audit: required\n- path: /pse/financial_institutions\n  method: get\n  operationId: listPseFinancialInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_links/{id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/agentic-access/wompi-agentic-access.yml
summary_line: 11 operations · 6 acting · 3 human-in-the-loop
tags:
- Payments
- Fintech
- Colombia
- LatAm
- Payment Gateway
- PSE
- Nequi
---
