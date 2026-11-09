---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 16
api_specs:
- filename: ecoaloha-com-a2a-api-openapi.yml
  format: yaml
  label: EcoAloha A2a API
  slug: ecoaloha-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-a2a-api-openapi.yml
- filename: ecoaloha-com-ask-api-openapi.yml
  format: yaml
  label: EcoAloha Ask API
  slug: ecoaloha-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-ask-api-openapi.yml
- filename: ecoaloha-com-discovery-api-openapi.yml
  format: yaml
  label: EcoAloha Discovery API
  slug: ecoaloha-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-discovery-api-openapi.yml
- filename: ecoaloha-com-experiences-api-openapi.yml
  format: yaml
  label: EcoAloha Experiences API
  slug: ecoaloha-com-experiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-experiences-api-openapi.yml
- filename: ecoaloha-com-sandbox-api-openapi.yml
  format: yaml
  label: EcoAloha Sandbox API
  slug: ecoaloha-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-sandbox-api-openapi.yml
- filename: ecoaloha-com-share-api-openapi.yml
  format: yaml
  label: EcoAloha Share API
  slug: ecoaloha-com-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecoaloha-com/openapi/ecoaloha-com-share-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ecoaloha Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a
operation_count: 22
overview: 'EcoAloha exposes 22 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EcoAloha
provider_slug: ecoaloha-com
slug: ecoaloha-com-agentic-access
source_filename: ecoaloha-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/ecoaloha-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 16\n    acting: 6\n  by_consequence:\n    read: 16\n    physical: 1\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/sandbox/v1\n  method: get\n  operationId: discover_fixture_sandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a\n  method: post\n  operationId: a2a_catalog_message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: get\n  operationId: search_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: ask_catalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/v1/destinations\n  method: get\n  operationId: sandbox_destinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/v1/experiences\n  method: get\n \
  \ operationId: sandbox_experiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox\n  method: get\n  operationId: discover_api_sandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations\n  method: get\n  operationId: list_destinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/nearest\n  method: get\n  operationId: nearest_destination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page-references\n  method: get\n  operationId: get_page_references\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: list_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{slug}\n  method: get\n  operationId: get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{slug}/experiences\n  method: get\n  operationId: get_collection_experiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiences\n  method: get\n  operationId: search_experiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiences/{id}\n\
  \  method: get\n  operationId: get_experience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiences/{id}/reviews\n  method: get\n  operationId: get_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare\n  method: post\n  operationId: compare_experiences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /experiences/batch\n  method: post\n  operationId: batch_experiences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking-link\n  method: post\n  operationId: get_booking_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share\n  method: post\n  operationId: create_share_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /share/{id}\n  method: get\n  operationId: get_share_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share/{id}\n  method: delete\n  operationId: delete_share_list\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ecoaloha-com/agentic-access/ecoaloha-com-agentic-access.yml
summary_line: 22 operations · 6 acting
tags:
- Travel
- Eco-tourism
- Outdoor
- Sustainable
- Adventure
---
