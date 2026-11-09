---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 18
api_specs:
- filename: buckybuild-com-addresses-api-openapi.yml
  format: yaml
  label: Bucky Addresses API
  slug: buckybuild-com-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-addresses-api-openapi.yml
- filename: buckybuild-com-citations-api-openapi.yml
  format: yaml
  label: Bucky Citations API
  slug: buckybuild-com-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-citations-api-openapi.yml
- filename: buckybuild-com-coverage-api-openapi.yml
  format: yaml
  label: Bucky Coverage API
  slug: buckybuild-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-coverage-api-openapi.yml
- filename: buckybuild-com-credentials-api-openapi.yml
  format: yaml
  label: Bucky Credentials API
  slug: buckybuild-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-credentials-api-openapi.yml
- filename: buckybuild-com-feasibility-api-openapi.yml
  format: yaml
  label: Bucky Feasibility API
  slug: buckybuild-com-feasibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-feasibility-api-openapi.yml
- filename: buckybuild-com-marketplace-api-openapi.yml
  format: yaml
  label: Bucky Marketplace API
  slug: buckybuild-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-marketplace-api-openapi.yml
- filename: buckybuild-com-sites-api-openapi.yml
  format: yaml
  label: Bucky Sites API
  slug: buckybuild-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-sites-api-openapi.yml
- filename: buckybuild-com-usage-api-openapi.yml
  format: yaml
  label: Bucky Usage API
  slug: buckybuild-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-usage-api-openapi.yml
consequence_counts:
  read: 18
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buckybuild Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Bucky exposes 24 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bucky
provider_slug: buckybuild-com
slug: buckybuild-com-agentic-access
source_filename: buckybuild-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buckybuild-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 18\n    acting: 6\n  by_consequence:\n    read: 18\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/marketplace/v2/builds\n  method: get\n  operationId: GetApiMarketplaceV2Builds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/v2/division-counts\n  method: get\n  operationId: GetApiMarketplaceV2DivisionCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/marketplace/v2/items\n  method: get\n  operationId: GetApiMarketplaceV2Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/v2/items/count\n  method: get\n  operationId: GetApiMarketplaceV2ItemsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/v2/items/{id}\n  method: get\n  operationId: GetApiMarketplaceV2ItemsByidBy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/marketplace/v2/map-markers\n  method: get\n  operationId: GetApiMarketplaceV2MapMarkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/addresses/retrieve\n  method: post\n  operationId: PostApiV1AddressesRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/addresses/suggest\n  method: post\n  operationId: PostApiV1AddressesSuggest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/citations/bylaw-sections\n  method: get\n  operationId: GetApiV1CitationsBylawSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage/divisions\n  method: get\n  operationId: GetApiV1CoverageDivisions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage/divisions/{slug}\n  method: get\n  operationId: GetApiV1CoverageDivisionsByslugBy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credentials/self\n  method: get\n  operationId: GetApiV1CredentialsSelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/feasibility/analyses\n  method: get\n  operationId: GetApiV1FeasibilityAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/feasibility/analyses\n  method: post\n  operationId: PostApiV1FeasibilityAnalyses\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/feasibility/analyses/{analysisId}\n  method: get\n  operationId: GetApiV1FeasibilityAnalysesByanalysisIdBy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/feasibility/analyses/{analysisId}/interpretations\n  method: post\n  operationId: PostApiV1FeasibilityAnalysesByanalysisIdByInterpretations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/check\n  method: get\n  operationId: GetApiV1SitesCheck\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/check\n  method: post\n  operationId: PostApiV1SitesCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/context\n  method: get\n  operationId: GetApiV1SitesContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/context\n  method: post\n  operationId: PostApiV1SitesContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/resolve\n  method: get\n  operationId: GetApiV1SitesResolve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/resolve\n  method: post\n  operationId: PostApiV1SitesResolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage/balance\n  method: get\n  operationId: GetApiV1UsageBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/receipts\n  method: get\n  operationId: GetApiV1UsageReceipts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/buckybuild-com/agentic-access/buckybuild-com-agentic-access.yml
summary_line: 24 operations · 6 acting
tags:
- Real Estate
- Zoning
- Mapping
- Data API
- Visualization
- Company
---
