---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: carbonara-co2-org-calculate-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Calculate API
  slug: carbonara-co2-org-calculate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-calculate-api-openapi.yml
- filename: carbonara-co2-org-factors-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Factors API
  slug: carbonara-co2-org-factors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-factors-api-openapi.yml
- filename: carbonara-co2-org-healthz-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Healthz API
  slug: carbonara-co2-org-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-healthz-api-openapi.yml
- filename: carbonara-co2-org-places-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Places API
  slug: carbonara-co2-org-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-places-api-openapi.yml
- filename: carbonara-co2-org-recommend-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Recommend API
  slug: carbonara-co2-org-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-recommend-api-openapi.yml
- filename: carbonara-co2-org-report-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Report API
  slug: carbonara-co2-org-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-report-api-openapi.yml
- filename: carbonara-co2-org-scenario-api-openapi.yml
  format: yaml
  label: Carbonara CO2 Scenario API
  slug: carbonara-co2-org-scenario-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonara-co2-org/openapi/carbonara-co2-org-scenario-api-openapi.yml
consequence_counts:
  physical: 5
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carbonara Co2 Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/calculate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/calculate/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/recommend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/report
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/scenario
operation_count: 8
overview: 'Carbonara CO2 exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carbonara CO2
provider_slug: carbonara-co2-org
slug: carbonara-co2-org-agentic-access
source_filename: carbonara-co2-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carbonara-co2-org-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 3\n    acting: 5\n  by_consequence:\n    read: 3\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/factors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calculate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calculate/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/report\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scenario\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recommend\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/carbonara-co2-org/agentic-access/carbonara-co2-org-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- Company
- Sustainability
- Open Source
- Climate Tech
- Software
---
