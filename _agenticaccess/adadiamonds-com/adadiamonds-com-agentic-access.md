---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 25
api_specs:
- filename: adadiamonds-com-agentic-checkout-acp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (ACP) API
  slug: adadiamonds-com-agentic-checkout-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-acp-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (hosted link) API
  slug: adadiamonds-com-agentic-checkout-hosted-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (UCP) API
  slug: adadiamonds-com-agentic-checkout-ucp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
- filename: adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic commerce discovery API
  slug: adadiamonds-com-agentic-commerce-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
- filename: adadiamonds-com-appointments-api-openapi.yml
  format: yaml
  label: Ada Diamonds Appointments API
  slug: adadiamonds-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-appointments-api-openapi.yml
- filename: adadiamonds-com-bulk-api-openapi.yml
  format: yaml
  label: Ada Diamonds Bulk API
  slug: adadiamonds-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-bulk-api-openapi.yml
- filename: adadiamonds-com-catalog-api-openapi.yml
  format: yaml
  label: Ada Diamonds Catalog API
  slug: adadiamonds-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-catalog-api-openapi.yml
- filename: adadiamonds-com-content-api-openapi.yml
  format: yaml
  label: Ada Diamonds Content API
  slug: adadiamonds-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-content-api-openapi.yml
- filename: adadiamonds-com-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Discovery API
  slug: adadiamonds-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-discovery-api-openapi.yml
- filename: adadiamonds-com-mcp-api-openapi.yml
  format: yaml
  label: Ada Diamonds MCP API
  slug: adadiamonds-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-mcp-api-openapi.yml
- filename: adadiamonds-com-onboarding-api-openapi.yml
  format: yaml
  label: Ada Diamonds Onboarding API
  slug: adadiamonds-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-onboarding-api-openapi.yml
- filename: adadiamonds-com-search-api-openapi.yml
  format: yaml
  label: Ada Diamonds Search API
  slug: adadiamonds-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-search-api-openapi.yml
consequence_counts:
  physical: 9
  read: 25
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adadiamonds Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ucp/checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/ucp/checkout-sessions/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ucp/checkout-sessions/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ucp/checkout-sessions/{id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout_links
operation_count: 41
overview: 'Ada Diamonds exposes 41 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 7 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ada Diamonds
provider_slug: adadiamonds-com
slug: adadiamonds-com-agentic-access
source_filename: adadiamonds-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/adadiamonds-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 25\n    acting: 16\n  by_consequence:\n    read: 25\n    write: 7\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1\n  method: get\n  operationId: getV1Probe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1\n  method: get\n  operationId: getApiV1Root\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diamonds\n  method: get\n  operationId: listDiamonds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diamonds/{id}\n  method: get\n  operationId: getDiamond\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/engagement-rings\n  method: get\n  operationId: listEngagementRings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/engagement-rings/{slug}\n  method: get\n  operationId: getEngagementRing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jewelry\n  method: get\n  operationId: listJewelry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jewelry/{slug}\n  method: get\n  operationId: getJewelryItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/knowledge-base\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/knowledge-base/{slug}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/showrooms\n  method: get\n  operationId: listShowrooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batch\n  method: post\n  operationId: batchRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports/{id}\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/consultations\n  method: post\n  operationId: requestConsultation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - appointments:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/register\n  method: get\n  operationId: describeRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/register\n  method: post\n  operationId: registerAgentAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing.md\n  method: get\n  operationId: getPricingMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?mode=agent\n  method: get\n  operationId: getAgentModeView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{section}/llms.txt\n  method: get\n  operationId: getSectionLlmsTxt\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ask\n  method: get\n  operationId: ask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ask\n  method: post\n  operationId: askPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/checkout_links\n  method: post\n  operationId: createCheckoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog:read\n    - content:read\n- path: /api/acp/checkout_sessions\n  method: post\n  operationId: acpCreateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}\n  method: get\n  operationId: acpGetCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cart:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acp/checkout_sessions/{id}\n  method: post\n  operationId: acpUpdateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}/complete\n  method: post\n  operationId: acpCompleteCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}/cancel\n  method: post\n  operationId: acpCancelCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ucp/checkout-sessions\n  method: post\n  operationId: ucpCreateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ucp/checkout-sessions/{id}\n  method: get\n  operationId: ucpGetCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cart:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ucp/checkout-sessions/{id}\n  method: put\n  operationId:\
  \ ucpUpdateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ucp/checkout-sessions/{id}/complete\n  method: post\n  operationId: ucpCompleteCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ucp/checkout-sessions/{id}/cancel\n  method: post\n  operationId: ucpCancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - cart:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/acp.json\n  method: get\n  operationId: acpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ucp\n  method: get\n  operationId: ucpProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/acp-products.jsonl\n  method: get\n  operationId: acpProductFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/apps/{view}\n  method: get\n\
  \  operationId: getMcpAppView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog:read\n    - content:read\n"
source_yaml_url: https://artifacts.apis.io/adadiamonds-com/agentic-access/adadiamonds-com-agentic-access.yml
summary_line: 41 operations · 16 acting
tags:
- Jewelry
- Lab Diamonds
- Engagement Rings
- New York
- E-Commerce
---
