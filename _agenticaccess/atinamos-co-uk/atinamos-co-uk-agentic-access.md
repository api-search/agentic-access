---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: atinamos-co-uk-agent-api-openapi.yml
  format: yaml
  label: atinamos-co-uk Agent API
  slug: atinamos-co-uk-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atinamos-co-uk/openapi/atinamos-co-uk-agent-api-openapi.yml
- filename: atinamos-co-uk-catalog-api-openapi.yml
  format: yaml
  label: atinamos-co-uk Catalog API
  slug: atinamos-co-uk-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atinamos-co-uk/openapi/atinamos-co-uk-catalog-api-openapi.yml
- filename: atinamos-co-uk-health-api-openapi.yml
  format: yaml
  label: atinamos-co-uk Health API
  slug: atinamos-co-uk-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atinamos-co-uk/openapi/atinamos-co-uk-health-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atinamos Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'atinamos-co-uk exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: atinamos-co-uk
provider_slug: atinamos-co-uk
slug: atinamos-co-uk-agentic-access
source_filename: atinamos-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/atinamos-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/render-check\n  method: post\n  operationId: create_render_check_agent_render_check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog\n  method: get\n  operationId: catalog_v1_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/market/search\n  method: get\n  operationId: market_search_agent_market_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/market/service/{service_id}\n  method: get\n  operationId: market_service_agent_market_service__service_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/buyer-check\n  method: post\n  operationId: create_buyer_check_agent_buyer_check_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/technical-seo-crawl\n  method: post\n  operationId: create_technical_seo_crawl_agent_technical_seo_crawl_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/json-repair\n  method: post\n  operationId: create_json_repair_agent_json_repair_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /agent/jobs/{job_id}\n  method: get\n  operationId: get_shop_job_agent_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/atinamos-co-uk/agentic-access/atinamos-co-uk-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Web Development
- Software
- Automation
- Artificial Intelligence
- E-Commerce
- United Kingdom
---
