---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: maddegen-art-pump-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Pump Cortex API
  slug: maddegen-art-pump-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-pump-cortex-api-openapi.yml
- filename: maddegen-art-chain-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Chain Cortex API
  slug: maddegen-art-chain-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-chain-cortex-api-openapi.yml
- filename: maddegen-art-forensics-lobe-api-openapi.yml
  format: yaml
  label: maddegen-art Forensics Lobe API
  slug: maddegen-art-forensics-lobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-forensics-lobe-api-openapi.yml
- filename: maddegen-art-hub-api-openapi.yml
  format: yaml
  label: maddegen-art Hub API
  slug: maddegen-art-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-hub-api-openapi.yml
- filename: maddegen-art-knowledge-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Knowledge Cortex API
  slug: maddegen-art-knowledge-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-knowledge-cortex-api-openapi.yml
- filename: maddegen-art-liquidity-lobe-api-openapi.yml
  format: yaml
  label: maddegen-art Liquidity Lobe API
  slug: maddegen-art-liquidity-lobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-liquidity-lobe-api-openapi.yml
- filename: maddegen-art-market-stem-api-openapi.yml
  format: yaml
  label: maddegen-art Market Stem API
  slug: maddegen-art-market-stem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-market-stem-api-openapi.yml
- filename: maddegen-art-risk-amygdala-api-openapi.yml
  format: yaml
  label: maddegen-art Risk Amygdala API
  slug: maddegen-art-risk-amygdala-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-risk-amygdala-api-openapi.yml
- filename: maddegen-art-utility-cerebellum-api-openapi.yml
  format: yaml
  label: maddegen-art Utility Cerebellum API
  slug: maddegen-art-utility-cerebellum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-utility-cerebellum-api-openapi.yml
- filename: maddegen-art-web-senses-api-openapi.yml
  format: yaml
  label: maddegen-art Web Senses API
  slug: maddegen-art-web-senses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-web-senses-api-openapi.yml
- filename: maddegen-art-world-map-api-openapi.yml
  format: yaml
  label: maddegen-art World Map API
  slug: maddegen-art-world-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-world-map-api-openapi.yml
consequence_counts:
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Maddegen Art Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'maddegen-art exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: maddegen-art
provider_slug: maddegen-art
slug: maddegen-art-agentic-access
source_filename: maddegen-art-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/maddegen-art-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /hub/api/v1/tools/pump_pulse\n  method: post\n  operationId: pump_pulse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/tools/pump_history\n  method: post\n  operationId: pump_history\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/tools/pump_launches\n  method: post\n  operationId: pump_launches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/tools/pump_token\n  method: post\n  operationId: pump_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/maddegen-art/agentic-access/maddegen-art-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Company
---
