---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 23
api_specs:
- filename: depixapp-com-account-api-openapi.yml
  format: yaml
  label: DePix App Account API
  slug: depixapp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-account-api-openapi.yml
- filename: depixapp-com-agents-api-openapi.yml
  format: yaml
  label: DePix App Agents API
  slug: depixapp-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-agents-api-openapi.yml
- filename: depixapp-com-checkouts-api-openapi.yml
  format: yaml
  label: DePix App Checkouts API
  slug: depixapp-com-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-checkouts-api-openapi.yml
- filename: depixapp-com-merchant-api-openapi.yml
  format: yaml
  label: DePix App Merchant API
  slug: depixapp-com-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-merchant-api-openapi.yml
- filename: depixapp-com-meta-api-openapi.yml
  format: yaml
  label: DePix App Meta API
  slug: depixapp-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-meta-api-openapi.yml
- filename: depixapp-com-pay-api-openapi.yml
  format: yaml
  label: DePix App Pay API
  slug: depixapp-com-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-pay-api-openapi.yml
- filename: depixapp-com-products-api-openapi.yml
  format: yaml
  label: DePix App Products API
  slug: depixapp-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-products-api-openapi.yml
- filename: depixapp-com-public-api-openapi.yml
  format: yaml
  label: DePix App Public API
  slug: depixapp-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-public-api-openapi.yml
- filename: depixapp-com-support-api-openapi.yml
  format: yaml
  label: DePix App Support API
  slug: depixapp-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-support-api-openapi.yml
consequence_counts:
  physical: 8
  read: 23
  safety-critical: 2
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Depixapp Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/agents/keys/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/agents/verify-domain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkouts/{id}/simulate-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/merchants/{username}/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pay/{id}/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/products/featured
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/products/{id}/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/withdraw
operation_count: 48
overview: 'DePix App exposes 48 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 15 write, 8 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DePix App
provider_slug: depixapp-com
slug: depixapp-com-agentic-access
source_filename: depixapp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/depixapp-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    acting: 25\n    connected: 23\n  by_consequence:\n    physical: 8\n    read: 23\n    write: 15\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/deposit\n  method: post\n  operationId: createDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/vault/status\n\
  \  method: get\n  operationId: getVaultStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deposits/{id}\n  method: get\n  operationId: getDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/withdraw\n  method: post\n  operationId: createWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/withdrawals/{id}\n  method: get\n  operationId: getWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/checkouts\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkouts\n  method: get\n  operationId: listCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkouts/{id}\n  method: get\n  operationId: getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkouts/{id}/simulate-payment\n  method: post\n  operationId: simulateCheckoutPayment\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tickets\n  method: post\n  operationId: createTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tickets\n  method: get\n  operationId: listTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tickets/{id}\n  method: get\n  operationId: getTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tickets/{id}/messages\n  method: post\n  operationId: replyTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tickets/{id}/attachments\n  method: post\n  operationId: attachToTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/tickets/{id}/close\n  method: post\n  operationId: closeTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tickets/{id}/rating\n  method: post\n  operationId: rateTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/me\n  method: patch\n  operationId: updateMerchantProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/featured\n  method: post\n  operationId: setFeaturedProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/{id}\n  method: patch\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/{id}/deactivate\n  method: post\n  operationId: deactivateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/{id}/activate\n\
  \  method: post\n  operationId: activateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/{id}/checkouts\n  method: get\n  operationId: listProductCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/{id}/public\n  method: get\n  operationId: getPublicProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/{id}/checkout\n  method: post\n  operationId: createProductCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/{username}/public\n  method: get\n  operationId: getPublicMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/merchants/{username}/checkout\n  method: post\n  operationId: createMerchantCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pay/{id}\n  method: get\n  operationId: getPublicCheckout\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pay/{id}/simulate\n  method: post\n  operationId: simulatePublicCheckoutPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/domain-tlds\n  method: get\n  operationId: listAgentDomainTlds\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/verify-domain\n  method: post\n  operationId: verifyAgentDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/agents/keys\n  method: post\n  operationId: createAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/keys/revoke\n  method: post\n  operationId: revokeAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/agents/webhook-secret\n  method: post\n  operationId: rotateAgentWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/depix-pay\n  method: post\n  operationId: setAgentDepixRail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/status\n  method:\
  \ get\n  operationId: getAgentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhook-logs\n  method: get\n  operationId: listWebhookLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhook-logs/{id}\n  method: get\n  operationId: getWebhookLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/webhook-logs\n  method: get\n  operationId: listAgentWebhookLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/webhook-logs/{id}\n  method: get\n  operationId: getAgentWebhookLog\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verification\n  method: get\n  operationId: getVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verification\n  method: post\n  operationId: claimVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenapiDocument\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/depixapp-com/agentic-access/depixapp-com-agentic-access.yml
summary_line: 48 operations · 25 acting · 2 human-in-the-loop
tags:
- Company
- Payments
- Pix
- Stablecoins
- Cryptocurrency
- Bitcoin
- Liquid Network
- Brazil
- MCP
---
