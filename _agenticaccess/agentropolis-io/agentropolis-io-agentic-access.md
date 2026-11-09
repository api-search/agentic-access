---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 40
api_specs:
- filename: agentropolis-io-badge-api-openapi.yml
  format: yaml
  label: Agentropolis Badge API
  slug: agentropolis-io-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-badge-api-openapi.yml
- filename: agentropolis-io-badges-api-openapi.yml
  format: yaml
  label: Agentropolis Badges API
  slug: agentropolis-io-badges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-badges-api-openapi.yml
- filename: agentropolis-io-business-model-api-openapi.yml
  format: yaml
  label: Agentropolis Business Model API
  slug: agentropolis-io-business-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-business-model-api-openapi.yml
- filename: agentropolis-io-buyers-api-openapi.yml
  format: yaml
  label: Agentropolis Buyers API
  slug: agentropolis-io-buyers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-buyers-api-openapi.yml
- filename: agentropolis-io-call-api-openapi.yml
  format: yaml
  label: Agentropolis Call API
  slug: agentropolis-io-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-call-api-openapi.yml
- filename: agentropolis-io-categories-api-openapi.yml
  format: yaml
  label: Agentropolis Categories API
  slug: agentropolis-io-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-categories-api-openapi.yml
- filename: agentropolis-io-go-api-openapi.yml
  format: yaml
  label: Agentropolis Go API
  slug: agentropolis-io-go-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-go-api-openapi.yml
- filename: agentropolis-io-listings-api-openapi.yml
  format: yaml
  label: Agentropolis Listings API
  slug: agentropolis-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-listings-api-openapi.yml
- filename: agentropolis-io-market-api-openapi.yml
  format: yaml
  label: Agentropolis Market API
  slug: agentropolis-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-market-api-openapi.yml
- filename: agentropolis-io-reports-api-openapi.yml
  format: yaml
  label: Agentropolis Reports API
  slug: agentropolis-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-reports-api-openapi.yml
- filename: agentropolis-io-roadmap-api-openapi.yml
  format: yaml
  label: Agentropolis Roadmap API
  slug: agentropolis-io-roadmap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-roadmap-api-openapi.yml
- filename: agentropolis-io-search-api-openapi.yml
  format: yaml
  label: Agentropolis Search API
  slug: agentropolis-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-search-api-openapi.yml
- filename: agentropolis-io-sellers-api-openapi.yml
  format: yaml
  label: Agentropolis Sellers API
  slug: agentropolis-io-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-sellers-api-openapi.yml
- filename: agentropolis-io-sources-api-openapi.yml
  format: yaml
  label: Agentropolis Sources API
  slug: agentropolis-io-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-sources-api-openapi.yml
- filename: agentropolis-io-sponsored-api-openapi.yml
  format: yaml
  label: Agentropolis Sponsored API
  slug: agentropolis-io-sponsored-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-sponsored-api-openapi.yml
- filename: agentropolis-io-stats-api-openapi.yml
  format: yaml
  label: Agentropolis Stats API
  slug: agentropolis-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-stats-api-openapi.yml
- filename: agentropolis-io-tools-api-openapi.yml
  format: yaml
  label: Agentropolis Tools API
  slug: agentropolis-io-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-tools-api-openapi.yml
- filename: agentropolis-io-trust-api-openapi.yml
  format: yaml
  label: Agentropolis Trust API
  slug: agentropolis-io-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentropolis-io/openapi/agentropolis-io-trust-api-openapi.yml
consequence_counts:
  read: 40
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentropolis Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'Agentropolis exposes 52 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentropolis
provider_slug: agentropolis-io
slug: agentropolis-io-agentic-access
source_filename: agentropolis-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentropolis-io-openapi.json, openapi/agentropolis-io.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 40\n    acting: 12\n  by_consequence:\n    read: 40\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/listings/{id}/kit.json\n  method: get\n  operationId: getKitManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/call/{id}\n  method: post\n  operationId: callKit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sources\n  method: get\n  operationId: sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trust/method\n  method: get\n  operationId: trustMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/business-model\n  method: get\n  operationId: businessModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roadmap\n  method: get\n  operationId: roadmap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{week}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/badges\n  method: get\n  operationId: badges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badge/{file}\n  method: get\n  operationId: badgeSvg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/reports\n  method: get\n  operationId: marketReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sponsored\n  method: get\n  operationId: sponsored\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/login\n  method: post\n  operationId: sellerLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/me\n  method: get\n  operationId: sellerMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/claim\n  method: get\n  operationId: listClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/claim\n  method: post\n  operationId: createClaim\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/claim/{id}/check\n  method: post\n  operationId: checkClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /go/{id}\n  method: get\n  operationId: clickThrough\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/verify\n  method: post\n  operationId: sellerVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/me/analytics\n  method: get\n  operationId: sellerAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/kit-builder\n  method: post\n  operationId: kitBuilder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/buyers/account\n  method: get\n  operationId: buyerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings/{id}/kit.json\n  method: get\n  operationId: getKitManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/call/{id}\n  method: post\n  operationId: callKit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/sources\n  method: get\n  operationId: sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trust/method\n  method: get\n  operationId: trustMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/business-model\n  method: get\n  operationId: businessModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roadmap\n  method: get\n  operationId: roadmap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: stats\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{week}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/badges\n  method: get\n  operationId: badges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badge/{file}\n  method: get\n  operationId: badgeSvg\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/reports\n  method: get\n  operationId: marketReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sponsored\n  method: get\n  operationId: sponsored\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/login\n  method: post\n  operationId: sellerLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/me\n  method: get\n  operationId: sellerMe\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/claim\n  method: get\n  operationId: listClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/claim\n  method: post\n  operationId: createClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/claim/{id}/check\n  method: post\n  operationId: checkClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /go/{id}\n  method: get\n  operationId: clickThrough\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sellers/verify\n  method: post\n  operationId: sellerVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sellers/me/analytics\n  method: get\n  operationId: sellerAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/kit-builder\n  method: post\n  operationId: kitBuilder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/buyers/account\n  method: get\n  operationId: buyerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentropolis-io/agentic-access/agentropolis-io-agentic-access.yml
summary_line: 52 operations · 12 acting
tags:
- Artificial Intelligence
- Agents
- Marketplace
- Search
- Tools
---
