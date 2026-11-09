---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 24
api_specs:
- filename: axiomrelay-io-agents-api-openapi.yml
  format: yaml
  label: Axiom Relay Agents API
  slug: axiomrelay-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-agents-api-openapi.yml
- filename: axiomrelay-io-capabilities-api-openapi.yml
  format: yaml
  label: Axiom Relay Capabilities API
  slug: axiomrelay-io-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-capabilities-api-openapi.yml
- filename: axiomrelay-io-commerce-api-openapi.yml
  format: yaml
  label: Axiom Relay Commerce API
  slug: axiomrelay-io-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-commerce-api-openapi.yml
- filename: axiomrelay-io-commons-api-openapi.yml
  format: yaml
  label: Axiom Relay Commons API
  slug: axiomrelay-io-commons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-commons-api-openapi.yml
- filename: axiomrelay-io-communications-api-openapi.yml
  format: yaml
  label: Axiom Relay Communications API
  slug: axiomrelay-io-communications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-communications-api-openapi.yml
- filename: axiomrelay-io-directory-api-openapi.yml
  format: yaml
  label: Axiom Relay Directory API
  slug: axiomrelay-io-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-directory-api-openapi.yml
- filename: axiomrelay-io-evidence-api-openapi.yml
  format: yaml
  label: Axiom Relay Evidence API
  slug: axiomrelay-io-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-evidence-api-openapi.yml
- filename: axiomrelay-io-health-api-openapi.yml
  format: yaml
  label: Axiom Relay Health API
  slug: axiomrelay-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-health-api-openapi.yml
- filename: axiomrelay-io-payments-api-openapi.yml
  format: yaml
  label: Axiom Relay Payments API
  slug: axiomrelay-io-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-payments-api-openapi.yml
- filename: axiomrelay-io-platform-api-openapi.yml
  format: yaml
  label: Axiom Relay Platform API
  slug: axiomrelay-io-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-platform-api-openapi.yml
- filename: axiomrelay-io-treasury-api-openapi.yml
  format: yaml
  label: Axiom Relay Treasury API
  slug: axiomrelay-io-treasury-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-treasury-api-openapi.yml
consequence_counts:
  physical: 5
  read: 24
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Axiomrelay Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/settlements/observations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders/{id}/payments/stripe/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders/{id}/payments/usdc
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders/{id}/payments/usdc/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payments/stripe/webhook
operation_count: 41
overview: 'Axiom Relay exposes 41 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 11 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Axiom Relay
provider_slug: axiomrelay-io
slug: axiomrelay-io-agentic-access
source_filename: axiomrelay-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/axiomrelay-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 24\n    acting: 17\n  by_consequence:\n    read: 24\n    write: 11\n    physical: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/capabilities\n  method: get\n  operationId: listCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capabilities/{id}\n  method: get\n  operationId: describeCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api/v1/capabilities/{id}/invoke\n  method: post\n  operationId: invokeCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/services\n  method: get\n  operationId: browseServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/services/{slug}\n  method: get\n  operationId: getServiceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory\n  method: get\n  operationId: searchDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/{entry}\n  method: get\n  operationId: getDirectoryEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quotes\n  method: post\n  operationId: createProductQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders\n  method: post\n  operationId: createProductOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commerce/merchants\n  method: get\n  operationId: listCommerceMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commerce/settlement-profiles\n  method: get\n  operationId: listSettlementProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/settlements/observations\n  method: post\n  operationId: observeSandboxSettlement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/orders/{id}\n  method: get\n \
  \ operationId: getCommerceOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{id}/payments/stripe/checkout\n  method: post\n  operationId: createStripeCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders/{id}/payments/usdc\n  method: post\n  operationId: prepareBaseUsdcPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/orders/{id}/payments/usdc\n  method: get\n  operationId: getBaseUsdcPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{id}/payments/usdc/transactions\n  method: post\n  operationId: submitBaseUsdcTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payments/stripe/webhook\n  method: post\n  operationId: ingestStripeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payments/readiness\n  method: get\n  operationId: getPaymentReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounting/export\n  method: get\n  operationId: exportInternalTestAccounting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/verify\n  method: post\n  operationId: verifyReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/first-cohort\n\
  \  method: get\n  operationId: getFirstAgentCohort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/concierge/answer\n  method: post\n  operationId: askAxiomConcierge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/beacon/scout\n  method: post\n  operationId: runBeaconScout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/api-doctor\n  method: post\n  operationId: runApiDoctor\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/endpoint-scout\n  method: post\n  operationId: runEndpointScout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/domain-scout\n  method: post\n  operationId: runDomainScout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/mer-receipt-clerk\n\
  \  method: post\n  operationId: runMerReceiptClerk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/render\n  method: post\n  operationId: renderMerHumanProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/rooms\n  method: get\n  operationId: listRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rooms/{slug}\n  method: get\n  operationId: getRoom\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/communications/adapters\n  method: get\n  operationId: listCommunicationAdapters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-access\n  method: get\n  operationId: getAgentAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/integrations\n  method: get\n  operationId: listRuntimeIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events\n  method: get\n  operationId: listPublicEcosystemEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: readWebhookContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/release\n  method: get\n  operationId: getReleaseManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/readiness\n  method: get\n  operationId: getPlatformReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/publication\n  method: get\n  operationId: getPublicPlatformProjection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/axiomrelay-io/agentic-access/axiomrelay-io-agentic-access.yml
summary_line: 41 operations · 17 acting · 1 human-in-the-loop
tags:
- Agents
- Commerce
- Marketplace
- Infrastructure
---
