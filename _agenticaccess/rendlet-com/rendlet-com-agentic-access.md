---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: rendlet-com-checkout-api-openapi.yml
  format: yaml
  label: rendlet-com Checkout API
  slug: rendlet-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-checkout-api-openapi.yml
- filename: rendlet-com-pdf-api-openapi.yml
  format: yaml
  label: rendlet-com PDF API
  slug: rendlet-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-pdf-api-openapi.yml
- filename: rendlet-com-signup-api-openapi.yml
  format: yaml
  label: rendlet-com Signup API
  slug: rendlet-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-signup-api-openapi.yml
- filename: rendlet-com-templates-api-openapi.yml
  format: yaml
  label: rendlet-com Templates API
  slug: rendlet-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-templates-api-openapi.yml
- filename: rendlet-com-usage-api-openapi.yml
  format: yaml
  label: rendlet-com Usage API
  slug: rendlet-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendlet-com/openapi/rendlet-com-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rendlet Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 5
overview: 'rendlet-com exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rendlet-com
provider_slug: rendlet-com
slug: rendlet-com-agentic-access
source_filename: rendlet-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rendlet-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/pdf\n  method: post\n  operationId: renderPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signup\n  method: post\n  operationId: requestKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://artifacts.apis.io/rendlet-com/agentic-access/rendlet-com-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Company
- PDF
- Document Generation
- Software-as-a-Service
- Artificial Intelligence
---
