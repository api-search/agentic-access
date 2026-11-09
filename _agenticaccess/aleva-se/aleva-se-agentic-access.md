---
acting_count: 0
action_class_counts:
  connected: 50
api_specs:
- filename: aleva-se-aviation-api-openapi.yml
  format: yaml
  label: Aleva Aviation API
  slug: aleva-se-aviation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-aviation-api-openapi.yml
- filename: aleva-se-courts-api-openapi.yml
  format: yaml
  label: Aleva Courts API
  slug: aleva-se-courts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-courts-api-openapi.yml
- filename: aleva-se-domains-api-openapi.yml
  format: yaml
  label: Aleva Domains API
  slug: aleva-se-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-domains-api-openapi.yml
- filename: aleva-se-economy-api-openapi.yml
  format: yaml
  label: Aleva Economy API
  slug: aleva-se-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-economy-api-openapi.yml
- filename: aleva-se-energy-api-openapi.yml
  format: yaml
  label: Aleva Energy API
  slug: aleva-se-energy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-energy-api-openapi.yml
- filename: aleva-se-foods-api-openapi.yml
  format: yaml
  label: Aleva Foods API
  slug: aleva-se-foods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-foods-api-openapi.yml
- filename: aleva-se-jobs-api-openapi.yml
  format: yaml
  label: Aleva Jobs API
  slug: aleva-se-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-jobs-api-openapi.yml
- filename: aleva-se-medicines-api-openapi.yml
  format: yaml
  label: Aleva Medicines API
  slug: aleva-se-medicines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-medicines-api-openapi.yml
- filename: aleva-se-municipalities-api-openapi.yml
  format: yaml
  label: Aleva Municipalities API
  slug: aleva-se-municipalities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-municipalities-api-openapi.yml
- filename: aleva-se-rates-api-openapi.yml
  format: yaml
  label: Aleva Rates API
  slug: aleva-se-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-rates-api-openapi.yml
- filename: aleva-se-riksdag-api-openapi.yml
  format: yaml
  label: Aleva Riksdag API
  slug: aleva-se-riksdag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-riksdag-api-openapi.yml
- filename: aleva-se-stats-api-openapi.yml
  format: yaml
  label: Aleva Stats API
  slug: aleva-se-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-stats-api-openapi.yml
- filename: aleva-se-sweden-api-openapi.yml
  format: yaml
  label: Aleva Sweden API
  slug: aleva-se-sweden-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-sweden-api-openapi.yml
- filename: aleva-se-tourism-api-openapi.yml
  format: yaml
  label: Aleva Tourism API
  slug: aleva-se-tourism-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-tourism-api-openapi.yml
- filename: aleva-se-trains-api-openapi.yml
  format: yaml
  label: Aleva Trains API
  slug: aleva-se-trains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-trains-api-openapi.yml
- filename: aleva-se-weather-api-openapi.yml
  format: yaml
  label: Aleva Weather API
  slug: aleva-se-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-weather-api-openapi.yml
- filename: aleva-se-web-api-openapi.yml
  format: yaml
  label: Aleva Web API
  slug: aleva-se-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-web-api-openapi.yml
consequence_counts:
  read: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aleva Se Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 50
overview: 'Aleva exposes 50 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aleva
provider_slug: aleva-se
slug: aleva-se-agentic-access
source_filename: aleva-se-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aleva-se-dev-openapi.json, openapi/aleva-se-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 50\n  by_consequence:\n    read: 50\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/domains/dropped\n  method: get\n  operationId: domains-dropped\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/new\n  method: get\n  operationId: domains-new\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{name}\n\
  \  method: get\n  operationId: domain-lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats/dnssec\n  method: get\n  operationId: stats-dnssec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats/nameservers\n  method: get\n  operationId: stats-nameservers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aviation/airports\n  method: get\n  operationId: airport-passengers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aviation/passengers/monthly\n  method: get\n  operationId: air-passengers-monthly\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courts/rulings\n  method: get\n  operationId: court-rulings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courts/rulings/by-court\n  method: get\n  operationId: court-rulings-by-court\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/dropped\n  method: get\n  operationId: domains-dropped\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/expiring\n  method: get\n  operationId: domains-expiring\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/domains/expiring/valuable\n  method: get\n  operationId: domains-valuable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/new\n  method: get\n  operationId: domains-new\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{name}\n  method: get\n  operationId: domain-lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/economy/debt-restructuring\n  method: get\n  operationId: debt-restructuring\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/economy/debt-restructuring/by-age\n  method: get\n  operationId: debt-restructuring-by-age\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/energy/electricity/balance\n  method: get\n  operationId: electricity-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/energy/electricity/by-source\n  method: get\n  operationId: electricity-forecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/foods\n  method: get\n  operationId: foods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/ads\n  method: get\n  operationId: job-ads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/jobs/ads/national\n  method: get\n  operationId: job-ads-national\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/medicines/shortages\n  method: get\n  operationId: medicine-shortages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/medicines/shortages/by-group\n  method: get\n  operationId: medicine-shortages-by-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/medicines/shortages/monthly\n  method: get\n  operationId: medicine-shortages-monthly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/municipalities/figures\n\
  \  method: get\n  operationId: municipal-figures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/municipalities/figures/latest\n  method: get\n  operationId: municipal-figures-latest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rates/riksbank\n  method: get\n  operationId: riksbank-rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rates/swestr\n  method: get\n  operationId: swestr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/riksdag/party-agreement\n  method: get\n  operationId: party-agreement\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/riksdag/party-attendance\n  method: get\n  operationId: party-attendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats/dnssec\n  method: get\n  operationId: stats-dnssec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats/nameservers\n  method: get\n  operationId: stats-nameservers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sweden/cpi\n  method: get\n  operationId: consumer-prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sweden/house-prices\n\
  \  method: get\n  operationId: house-prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sweden/population\n  method: get\n  operationId: population\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sweden/population/latest\n  method: get\n  operationId: population-latest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tourism/guest-nights\n  method: get\n  operationId: guest-nights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tourism/guest-nights/by-country\n  method: get\n  operationId: guest-nights-by-country\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tourism/guest-nights/by-county\n  method: get\n  operationId: guest-nights-by-county\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trains/punctuality\n  method: get\n  operationId: train-punctuality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trains/punctuality/daily\n  method: get\n  operationId: train-punctuality-daily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/history\n  method: get\n  operationId: weather-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/weather/now\n  method: get\n  operationId: weather-now\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/agents\n  method: get\n  operationId: web-agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/ai-stance\n  method: get\n  operationId: web-ai-stance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/apis\n  method: get\n  operationId: web-apis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/commerce-agents\n  method: get\n  operationId: web-commerce-agents\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/llms\n  method: get\n  operationId: web-llms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/mcp-registry\n  method: get\n  operationId: web-mcp-registry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/mcp-servers\n  method: get\n  operationId: web-mcp-servers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aleva-se/agentic-access/aleva-se-agentic-access.yml
summary_line: 50 operations
tags:
- Swedish
- Data Infrastructure
- Artificial Intelligence
- Open Data
- Government Data
---
