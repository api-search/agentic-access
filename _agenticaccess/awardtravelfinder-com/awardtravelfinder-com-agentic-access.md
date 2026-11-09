---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: awardtravelfinder-com-agent-api-openapi.yml
  format: yaml
  label: Award Travel Finder Agent API
  slug: awardtravelfinder-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardtravelfinder-com/openapi/awardtravelfinder-com-agent-api-openapi.yml
- filename: awardtravelfinder-com-airlines-api-openapi.yml
  format: yaml
  label: Award Travel Finder Airlines API
  slug: awardtravelfinder-com-airlines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardtravelfinder-com/openapi/awardtravelfinder-com-airlines-api-openapi.yml
- filename: awardtravelfinder-com-british-airways-admin-only-api-openapi.yml
  format: yaml
  label: Award Travel Finder British Airways (Admin Only) API
  slug: awardtravelfinder-com-british-airways-admin-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardtravelfinder-com/openapi/awardtravelfinder-com-british-airways-admin-only-api-openapi.yml
- filename: awardtravelfinder-com-cathay-pacific-api-openapi.yml
  format: yaml
  label: Award Travel Finder Cathay Pacific API
  slug: awardtravelfinder-com-cathay-pacific-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardtravelfinder-com/openapi/awardtravelfinder-com-cathay-pacific-api-openapi.yml
- filename: awardtravelfinder-com-hotels-api-openapi.yml
  format: yaml
  label: Award Travel Finder Hotels API
  slug: awardtravelfinder-com-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardtravelfinder-com/openapi/awardtravelfinder-com-hotels-api-openapi.yml
consequence_counts:
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Awardtravelfinder Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Award Travel Finder exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Award Travel Finder
provider_slug: awardtravelfinder-com
slug: awardtravelfinder-com-agentic-access
source_filename: awardtravelfinder-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/awardtravelfinder-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/airlines/airports\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/british_airways/availability\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/british_airways/monthly_availability\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/british_airways/pricing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cathay_pacific/availability\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cathay_pacific/monthly_availability\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cathay_pacific/pricing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hotels\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hotels/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hotels/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hotels/availability\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hotels/brands\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/awardtravelfinder-com/agentic-access/awardtravelfinder-com-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- Travel
- Awards
- Artificial Intelligence
- Flights
- Loyalty
---
