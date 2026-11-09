---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: chartervsown-com-calculator-api-openapi.yml
  format: yaml
  label: Charter vs Own Calculator API
  slug: chartervsown-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-calculator-api-openapi.yml
- filename: chartervsown-com-enquiry-api-openapi.yml
  format: yaml
  label: Charter vs Own Enquiry API
  slug: chartervsown-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-enquiry-api-openapi.yml
- filename: chartervsown-com-mcp-api-openapi.yml
  format: yaml
  label: Charter vs Own MCP API
  slug: chartervsown-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-mcp-api-openapi.yml
consequence_counts:
  physical: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chartervsown Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/calculate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/calculator_describe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/enquiry_describe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/submit_enquiry
operation_count: 5
overview: 'Charter vs Own exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Charter vs Own
provider_slug: chartervsown-com
slug: chartervsown-com-agentic-access
source_filename: chartervsown-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chartervsown-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    physical: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/calculator_describe\n  method: post\n  operationId: calculator_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/calculate\n  method: post\n  operationId:\
  \ calculate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/submit_enquiry\n  method: post\n  operationId: submit_enquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/chartervsown-com/agentic-access/chartervsown-com-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- Aviation
- Finance
- Calculator
- Private-Jet
- CostEstimator
---
