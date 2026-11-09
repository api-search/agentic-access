---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 25
api_specs:
- filename: encarapi-com-archive-api-openapi.yml
  format: yaml
  label: encarapi-com Archive API
  slug: encarapi-com-archive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-archive-api-openapi.yml
- filename: encarapi-com-catalog-api-openapi.yml
  format: yaml
  label: encarapi-com Catalog API
  slug: encarapi-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-catalog-api-openapi.yml
- filename: encarapi-com-discovery-api-openapi.yml
  format: yaml
  label: encarapi-com Discovery API
  slug: encarapi-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-discovery-api-openapi.yml
- filename: encarapi-com-equipment-api-openapi.yml
  format: yaml
  label: encarapi-com Equipment API
  slug: encarapi-com-equipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-equipment-api-openapi.yml
- filename: encarapi-com-leasing-api-openapi.yml
  format: yaml
  label: encarapi-com Leasing API
  slug: encarapi-com-leasing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-leasing-api-openapi.yml
- filename: encarapi-com-sync-api-openapi.yml
  format: yaml
  label: encarapi-com Sync API
  slug: encarapi-com-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-sync-api-openapi.yml
- filename: encarapi-com-taxonomy-api-openapi.yml
  format: yaml
  label: encarapi-com Taxonomy API
  slug: encarapi-com-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-taxonomy-api-openapi.yml
- filename: encarapi-com-trucks-api-openapi.yml
  format: yaml
  label: encarapi-com Trucks API
  slug: encarapi-com-trucks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-trucks-api-openapi.yml
- filename: encarapi-com-vehicle-api-openapi.yml
  format: yaml
  label: encarapi-com Vehicle API
  slug: encarapi-com-vehicle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/encarapi-com/openapi/encarapi-com-vehicle-api-openapi.yml
consequence_counts:
  read: 25
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Encarapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'encarapi-com exposes 29 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: encarapi-com
provider_slug: encarapi-com
slug: encarapi-com-agentic-access
source_filename: encarapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/encarapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 25\n    acting: 4\n  by_consequence:\n    read: 25\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/trucks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/trucks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/trucks/enums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/trucks/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/equipment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/equipment/enums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/equipment/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/leasing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/enums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nav\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/model-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/taxonomy/makes.csv\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /api/taxonomy/models.csv\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/changes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/taxonomy/badges.csv\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/taxonomy/option-packages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/bulk\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inspection/bulk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/record/bulk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inspection/{id}/versions\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/record/{id}/versions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/{id}/refresh\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/vehicle/by-vin/{vin}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/record/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/price-check/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inspection/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/encarapi-com/agentic-access/encarapi-com-agentic-access.yml
summary_line: 29 operations · 4 acting
tags:
- Automotive
- Data
- Korean
- Cars
---
