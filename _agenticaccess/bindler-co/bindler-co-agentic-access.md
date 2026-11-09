---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: bindler-co-ai-act-classify-api-openapi.yml
  format: yaml
  label: Bindler Ai Act Classify API
  slug: bindler-co-ai-act-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-ai-act-classify-api-openapi.yml
- filename: bindler-co-cbam-cost-api-openapi.yml
  format: yaml
  label: Bindler Cbam Cost API
  slug: bindler-co-cbam-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-cbam-cost-api-openapi.yml
- filename: bindler-co-uae-corporate-tax-api-openapi.yml
  format: yaml
  label: Bindler Uae Corporate Tax API
  slug: bindler-co-uae-corporate-tax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-uae-corporate-tax-api-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bindler Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Bindler exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bindler
provider_slug: bindler-co
slug: bindler-co-agentic-access
source_filename: bindler-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bindler-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /ai-act-classify\n  method: get\n  operationId: aiActClassifyGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-act-classify\n  method: post\n  operationId: aiActClassify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-act-classify\n  method: options\n  operationId: aiActClassifyOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbam-cost\n  method: get\n  operationId: cbamCostGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbam-cost\n  method: post\n  operationId: cbamCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cbam-cost\n  method: options\n  operationId: cbamCostOptions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uae-corporate-tax\n  method: get\n  operationId: uaeCorporateTax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uae-corporate-tax\n  method: post\n  operationId: uaeCorporateTaxPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uae-corporate-tax\n  method: options\n  operationId: uaeCorporateTaxOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bindler-co/agentic-access/bindler-co-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Company
- Data
- Finance
- Regulations
- Tools
---
