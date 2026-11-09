---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: sentineliq-net-agent-api-api-openapi.yml
  format: yaml
  label: sentineliq-net Agent API
  slug: sentineliq-net-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-agent-api-api-openapi.yml
- filename: sentineliq-net-mcp-api-openapi.yml
  format: yaml
  label: sentineliq-net MCP API
  slug: sentineliq-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-mcp-api-openapi.yml
- filename: sentineliq-net-property-research-api-openapi.yml
  format: yaml
  label: sentineliq-net Property Research API
  slug: sentineliq-net-property-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-property-research-api-openapi.yml
- filename: sentineliq-net-public-api-openapi.yml
  format: yaml
  label: sentineliq-net Public API
  slug: sentineliq-net-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-public-api-openapi.yml
- filename: sentineliq-net-seller-workflows-api-openapi.yml
  format: yaml
  label: sentineliq-net Seller Workflows API
  slug: sentineliq-net-seller-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-seller-workflows-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sentineliq Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/agent-api/v1/monthly-payment
operation_count: 23
overview: 'sentineliq-net exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sentineliq-net
provider_slug: sentineliq-net
slug: sentineliq-net-agentic-access
source_filename: sentineliq-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agent-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 8\n    acting: 15\n  by_consequence:\n    read: 8\n    write: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/agent-api/v1/whoami\n  method: get\n  operationId: agentApiWhoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/reet\n  method: post\n  operationId: agentApiReet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/net-sheet\n  method: post\n  operationId: agentApiNetSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/deadlines\n  method: post\n  operationId: agentApiDeadlines\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/property\n  method: get\n  operationId: agentApiProperty\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/permit-history\n  method: get\n  operationId: agentApiPermitHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/sale-history\n  method: get\n  operationId: agentApiSaleHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/comps\n  method: post\n  operationId: agentApiComps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/market\n  method: get\n  operationId: agentApiMarket\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/market-trends\n  method: get\n  operationId: agentApiMarketTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/local-context\n  method: get\n  operationId: agentApiLocalContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/site-context\n  method: get\n  operationId: agentApiSiteContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-api/v1/seller-scenarios\n  method: post\n  operationId: sellerScenarios\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/offers/compare\n  method: post\n  operationId: offerComparison\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/monthly-payment\n  method: post\n  operationId: monthlyPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/seller-packet\n  method: post\n  operationId: sellerPacket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/research-packet\n  method: post\n  operationId: researchPacket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-api/v1/property-changes\n  method: post\n  operationId: propertyChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mcp\n  method: post\n  operationId: mcpPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mcp/public\n  method: post\n  operationId: mcpPublicPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/reet\n  method: post\n  operationId: publicReet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/net-sheet\n  method: post\n  operationId: publicNetSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/deadlines\n  method: post\n  operationId: publicDeadlines\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sentineliq-net/agentic-access/sentineliq-net-agentic-access.yml
summary_line: 23 operations · 15 acting
tags:
- Company
- Real Estate
- Data API
- Washington
- AI Integration
---
