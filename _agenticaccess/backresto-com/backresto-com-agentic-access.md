---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 18
api_specs:
- filename: backresto-com-agent-api-openapi.yml
  format: yaml
  label: BackResto Agent API
  slug: backresto-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-agent-api-openapi.yml
- filename: backresto-com-allergens-api-openapi.yml
  format: yaml
  label: BackResto Allergens API
  slug: backresto-com-allergens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-allergens-api-openapi.yml
- filename: backresto-com-audit-api-openapi.yml
  format: yaml
  label: BackResto Audit API
  slug: backresto-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-audit-api-openapi.yml
- filename: backresto-com-health-api-openapi.yml
  format: yaml
  label: BackResto Health API
  slug: backresto-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-health-api-openapi.yml
- filename: backresto-com-meta-api-openapi.yml
  format: yaml
  label: BackResto Meta API
  slug: backresto-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-meta-api-openapi.yml
- filename: backresto-com-mobile-api-openapi.yml
  format: yaml
  label: BackResto Mobile API
  slug: backresto-com-mobile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-mobile-api-openapi.yml
- filename: backresto-com-module-assets-api-openapi.yml
  format: yaml
  label: BackResto module assets API
  slug: backresto-com-module-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-module-assets-api-openapi.yml
- filename: backresto-com-module-shadow-ingestion-api-openapi.yml
  format: yaml
  label: BackResto module shadow ingestion API
  slug: backresto-com-module-shadow-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-module-shadow-ingestion-api-openapi.yml
- filename: backresto-com-partner-restaurants-api-openapi.yml
  format: yaml
  label: BackResto partner restaurants API
  slug: backresto-com-partner-restaurants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-partner-restaurants-api-openapi.yml
- filename: backresto-com-received-module-snapshots-api-openapi.yml
  format: yaml
  label: BackResto received module snapshots API
  slug: backresto-com-received-module-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-received-module-snapshots-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Backresto Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/complete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/complete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/upload-url
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/upload-url
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/mutations/{mutationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/mutations/{mutationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mobile/sessions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mobile/sessions
operation_count: 28
overview: 'BackResto exposes 28 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 2 write, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BackResto
provider_slug: backresto-com
slug: backresto-com-agentic-access
source_filename: backresto-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/api_backresto.json, openapi/backresto-com-api-openapi.json, openapi/backresto-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 18\n    acting: 10\n  by_consequence:\n    read: 18\n    safety-critical: 8\n    write: 2\n  human_in_the_loop_required: 8\noperations:\n- path: /health/live\n  method: get\n  operationId: HealthController_getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: HealthController_getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/version\n  method: get\n  operationId: HealthController_getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mobile/sessions\n  method: post\n  operationId: MobileSessionController_exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants\n  method: get\n  operationId: PartnerRestaurantsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/mutations/{mutationId}\n\
  \  method: put\n  operationId: ShadowIngestController_ingest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{restaurantId}/collections\n  method: get\n  operationId: ShadowRecordsController_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records\n  method: get\n  operationId: ShadowRecordsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records/{recordId}\n\
  \  method: get\n  operationId: ShadowRecordsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/upload-url\n  method: post\n  operationId: ModuleAssetIngestController_reserve\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/complete\n  method: post\n  operationId: ModuleAssetIngestController_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets\n  method: get\n  operationId: ModuleAssetReadController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/live\n  method: get\n  operationId: HealthController_getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: HealthController_getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/version\n  method:\
  \ get\n  operationId: HealthController_getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mobile/sessions\n  method: post\n  operationId: MobileSessionController_exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants\n  method: get\n  operationId: PartnerRestaurantsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/mutations/{mutationId}\n  method: put\n  operationId: ShadowIngestController_ingest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{restaurantId}/collections\n  method: get\n  operationId: ShadowRecordsController_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records\n  method: get\n  operationId: ShadowRecordsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records/{recordId}\n  method: get\n  operationId: ShadowRecordsController_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/upload-url\n  method: post\n  operationId: ModuleAssetIngestController_reserve\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ingest/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets/{assetId}/complete\n  method: post\n  operationId: ModuleAssetIngestController_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{restaurantId}/collections/{collection}/records/{recordId}/assets\n  method: get\n  operationId: ModuleAssetReadController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/haccp-audit\n  method: post\n  operationId: submitHaccpExpressAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/allergen-table/parse\n  method: post\n  operationId: parseAllergenMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/markdown/{path}\n  method: get\n  operationId: getPageAsMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/backresto-com/agentic-access/backresto-com-agentic-access.yml
summary_line: 28 operations · 10 acting · 8 human-in-the-loop
tags:
- Food
- Restaurant
- HACCP
- Compliance
- Safety
- French
---
