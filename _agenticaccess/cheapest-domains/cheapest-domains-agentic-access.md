---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: cheapest-domains-availability-api-openapi.yml
  format: yaml
  label: Cheapest Domains Availability API
  slug: cheapest-domains-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-availability-api-openapi.yml
- filename: cheapest-domains-availability-batch-api-openapi.yml
  format: yaml
  label: Cheapest Domains Availability Batch API
  slug: cheapest-domains-availability-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-availability-batch-api-openapi.yml
- filename: cheapest-domains-cheapest-domains-public-api-api-openapi.yml
  format: yaml
  label: Cheapest Domains Cheapest Domains Public API
  slug: cheapest-domains-cheapest-domains-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-cheapest-domains-public-api-api-openapi.yml
- filename: cheapest-domains-estimate-api-openapi.yml
  format: yaml
  label: Cheapest Domains Estimate API
  slug: cheapest-domains-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-estimate-api-openapi.yml
- filename: cheapest-domains-health-api-openapi.yml
  format: yaml
  label: Cheapest Domains Health API
  slug: cheapest-domains-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-health-api-openapi.yml
- filename: cheapest-domains-name-comparison-api-openapi.yml
  format: yaml
  label: Cheapest Domains Name Comparison API
  slug: cheapest-domains-name-comparison-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-name-comparison-api-openapi.yml
- filename: cheapest-domains-name-finder-api-openapi.yml
  format: yaml
  label: Cheapest Domains Name Finder API
  slug: cheapest-domains-name-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-name-finder-api-openapi.yml
- filename: cheapest-domains-naming-guide-api-openapi.yml
  format: yaml
  label: Cheapest Domains Naming Guide API
  slug: cheapest-domains-naming-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-naming-guide-api-openapi.yml
- filename: cheapest-domains-popularity-api-openapi.yml
  format: yaml
  label: Cheapest Domains Popularity API
  slug: cheapest-domains-popularity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-popularity-api-openapi.yml
- filename: cheapest-domains-prices-api-openapi.yml
  format: yaml
  label: Cheapest Domains Prices API
  slug: cheapest-domains-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-prices-api-openapi.yml
- filename: cheapest-domains-registrar-link-api-openapi.yml
  format: yaml
  label: Cheapest Domains Registrar Link API
  slug: cheapest-domains-registrar-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-registrar-link-api-openapi.yml
- filename: cheapest-domains-registrars-api-openapi.yml
  format: yaml
  label: Cheapest Domains Registrars API
  slug: cheapest-domains-registrars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-registrars-api-openapi.yml
- filename: cheapest-domains-tlds-api-openapi.yml
  format: yaml
  label: Cheapest Domains Tlds API
  slug: cheapest-domains-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapest-domains/openapi/cheapest-domains-tlds-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cheapest Domains Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Cheapest Domains exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cheapest Domains
provider_slug: cheapest-domains
slug: cheapest-domains-agentic-access
source_filename: cheapest-domains-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cheapest-domains-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: get_capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: get_service_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices\n  method: get\n  operationId: search_prices\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tlds/{tld}\n  method: get\n  operationId: get_tld_prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/registrars\n  method: get\n  operationId: get_registrars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/estimate\n  method: get\n  operationId: estimate_cost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/registrar-link\n  method: get\n  operationId: get_registrar_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/naming-guide\n  method: get\n  operationId: get_naming_guidance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/availability\n  method: get\n  operationId: check_availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/popularity\n  method: get\n  operationId: get_domain_popularity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/availability-batch\n  method: get\n  operationId: check_availability_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/name-finder\n  method: get\n  operationId:\
  \ open_name_finder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tlds/{tld}/history\n  method: get\n  operationId: get_price_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/name-comparison\n  method: get\n  operationId: compare_domain_names\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cheapest-domains/agentic-access/cheapest-domains-agentic-access.yml
summary_line: 14 operations
tags:
- Domain Registration
- Price Comparison
- Domain Search
- API Tools
---
