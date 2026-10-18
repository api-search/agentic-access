---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 18
api_specs:
- filename: paidhandshake-capabilities-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Capabilities API
  slug: paidhandshake-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-capabilities-api-openapi.yml
- filename: paidhandshake-checkout-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Checkout API
  slug: paidhandshake-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-checkout-api-openapi.yml
- filename: paidhandshake-inventory-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Inventory API
  slug: paidhandshake-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-inventory-api-openapi.yml
- filename: paidhandshake-machine-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Machine API
  slug: paidhandshake-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-machine-api-openapi.yml
- filename: paidhandshake-proof-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Proof API
  slug: paidhandshake-proof-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-proof-api-openapi.yml
- filename: paidhandshake-quote-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Quote API
  slug: paidhandshake-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-quote-api-openapi.yml
- filename: paidhandshake-sample-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Sample API
  slug: paidhandshake-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-sample-api-openapi.yml
- filename: paidhandshake-search-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Search API
  slug: paidhandshake-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-search-api-openapi.yml
- filename: paidhandshake-well-known-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange .well Known API
  slug: paidhandshake-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-well-known-api-openapi.yml
- filename: paidhandshake-x402-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange X402 API
  slug: paidhandshake-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-x402-api-openapi.yml
consequence_counts:
  physical: 2
  read: 18
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Paidhandshake Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/machine/v1/watches/{watch_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/machine/v1/wallet/topup/x402
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout
operation_count: 25
overview: 'PaidHandshake Exchange exposes 25 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 4 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PaidHandshake Exchange
provider_slug: paidhandshake
slug: paidhandshake-agentic-access
source_filename: paidhandshake-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/paidhandshake-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 18\n    acting: 7\n  by_consequence:\n    read: 18\n    physical: 2\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inventory\n  method: get\n  operationId: getLiveInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/proof\n  method: get\n  operationId: getFulfillmentProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sample\n  method: get\n  operationId: getFreeDataSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: getX402Manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/v1/status\n  method: get\n  operationId: getX402Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/v1/item\n  method: get\n  operationId: buyVerifiedItemX402\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/v1/bundle\n  method: get\n  operationId: buyVerifiedBundleX402\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/wallet/topup/x402\n  method: post\n  operationId: fundMachineWalletX402\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/search\n  method: post\n  operationId: searchMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/search/{search_id}\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote/{search_id}\n  method: get\n  operationId: getUnlockQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/machine/v1/onboarding\n  method: get\n  operationId: getMachineOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/enroll\n  method: post\n  operationId: enrollMachineBuyer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/machine/v1/quote\n  method: post\n  operationId: quoteMachineJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/capabilities\n  method: get\n  operationId: getMachineCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/jobs\n  method: post\n  operationId: submitMachineJob\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/machine/v1/jobs/{job_id}\n  method: get\n  operationId: getMachineJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/wallet\n  method: get\n  operationId: getMachineWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/watches\n  method: get\n  operationId: listMachineWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/watches\n  method: post\n  operationId:\
  \ createMachineWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/machine/v1/watches/{watch_id}\n  method: get\n  operationId: getMachineWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/v1/watches/{watch_id}/enable\n  method: post\n  operationId: enableMachineWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/machine/v1/watches/{watch_id}/disable\n  method: post\n  operationId: disableMachineWatch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/agentic-access/paidhandshake-agentic-access.yml
summary_line: 25 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Marketplace
- Data
- Automation
---
