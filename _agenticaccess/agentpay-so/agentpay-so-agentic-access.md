---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 14
api_specs:
- filename: agentpay-so-acp-api-openapi.yml
  format: yaml
  label: AgentPay Labs ACP API
  slug: agentpay-so-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-acp-api-openapi.yml
- filename: agentpay-so-agentrank-api-openapi.yml
  format: yaml
  label: AgentPay Labs Agent Rank API
  slug: agentpay-so-agentrank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-agentrank-api-openapi.yml
- filename: agentpay-so-agents-api-openapi.yml
  format: yaml
  label: AgentPay Labs Agents API
  slug: agentpay-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-agents-api-openapi.yml
- filename: agentpay-so-ap2-api-openapi.yml
  format: yaml
  label: AgentPay Labs AP2 API
  slug: agentpay-so-ap2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-ap2-api-openapi.yml
- filename: agentpay-so-commerce-api-openapi.yml
  format: yaml
  label: AgentPay Labs Commerce API
  slug: agentpay-so-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-commerce-api-openapi.yml
- filename: agentpay-so-escrow-api-openapi.yml
  format: yaml
  label: AgentPay Labs Escrow API
  slug: agentpay-so-escrow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-escrow-api-openapi.yml
- filename: agentpay-so-health-api-openapi.yml
  format: yaml
  label: AgentPay Labs Health API
  slug: agentpay-so-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-health-api-openapi.yml
- filename: agentpay-so-marketplace-api-openapi.yml
  format: yaml
  label: AgentPay Labs Marketplace API
  slug: agentpay-so-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-marketplace-api-openapi.yml
- filename: agentpay-so-merchants-api-openapi.yml
  format: yaml
  label: AgentPay Labs Merchants API
  slug: agentpay-so-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-merchants-api-openapi.yml
- filename: agentpay-so-payments-api-openapi.yml
  format: yaml
  label: AgentPay Labs Payments API
  slug: agentpay-so-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-payments-api-openapi.yml
- filename: agentpay-so-webhooks-api-openapi.yml
  format: yaml
  label: AgentPay Labs Webhooks API
  slug: agentpay-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 14
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentpay So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ap2/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/marketplace/checkout-session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/merchants/profile/wallet
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-intents/{intentId}/verify
operation_count: 33
overview: 'AgentPay Labs exposes 33 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 12 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentPay Labs
provider_slug: agentpay-so
slug: agentpay-so-agentic-access
source_filename: agentpay-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentpay-so-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 14\n    acting: 19\n  by_consequence:\n    read: 14\n    write: 12\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/merchants/register\n  method: post\n  operationId: registerMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/profile\n  method: get\n  operationId: getMerchantProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/merchants/profile/wallet\n  method: patch\n  operationId: updateMerchantWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/profile/webhook\n  method: patch\n  operationId: updateMerchantWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/rotate-key\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/merchants/stats\n  method: get\n  operationId: getMerchantStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payment-intents\n  method: post\n  operationId: createAgentPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-intents/{intentId}\n  method: get\n  operationId: getPaymentIntentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payment-intents/{intentId}/verify\n  method: post\n  operationId: submitTxHash\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/receipt/{intentId}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/verify/{txHash}\n  method: get\n  operationId: verifyByTxHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agentrank/{agentId}\n  method: get\n  operationId: getAgentRank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agentrank/leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commerce/compile\n  method: post\n  operationId: compileCommerceDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/marketplace/discover\n  method: get\n  operationId: discoverAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/featured\n  method: get\n  operationId: getFeaturedAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/hire\n  method: post\n  operationId: hireAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/marketplace/hires\n  method: get\n  operationId: listMyHires\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/escrow/create\n  method: post\n  operationId: createEscrow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/escrow/{escrowId}/approve\n  method: post\n  operationId: approveEscrow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/escrow/{escrowId}/dispute\n  method: post\n  operationId: disputeEscrow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/subscribe\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/pay\n  method: post\n  operationId: acpPay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/verify\n  method: post\n  operationId: acpVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/schema\n  method: get\n  operationId: acpSchema\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ap2/request\n  method: post\n  operationId: ap2Request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ap2/receipt\n  method: post\n  operationId: ap2Receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ap2/confirm\n  method: post\n  operationId: ap2Confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ap2/status/{id}\n  method: get\n  operationId: ap2Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/checkout-session\n  method: post\n  operationId: createMarketplaceCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentpay-so/agentic-access/agentpay-so-agentic-access.yml
summary_line: 33 operations · 19 acting
tags:
- Company
- Research
- Robotics
- Automation
- Platform
---
