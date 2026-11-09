---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 1
api_specs:
- filename: boatvaluecalculator-com-calculator-api-openapi.yml
  format: yaml
  label: Boat Value Calculator Calculator API
  slug: boatvaluecalculator-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boatvaluecalculator-com/openapi/boatvaluecalculator-com-calculator-api-openapi.yml
- filename: boatvaluecalculator-com-enquiry-api-openapi.yml
  format: yaml
  label: Boat Value Calculator Enquiry API
  slug: boatvaluecalculator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boatvaluecalculator-com/openapi/boatvaluecalculator-com-enquiry-api-openapi.yml
consequence_counts:
  physical: 1
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boatvaluecalculator Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/enquiry_describe
operation_count: 9
overview: 'Boat Value Calculator exposes 9 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Boat Value Calculator
provider_slug: boatvaluecalculator-com
slug: boatvaluecalculator-com-agentic-access
source_filename: boatvaluecalculator-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/boatvaluecalculator-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 8\n    connected: 1\n  by_consequence:\n    write: 7\n    physical: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/calculator_describe\n  method: post\n  operationId: calculator_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/calculate\n  method: post\n  operationId: calculate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_submit\n  method: post\n  operationId: enquiry_submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_status\n  method: post\n  operationId: enquiry_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_cancel\n  method: post\n  operationId: enquiry_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_list\n  method: post\n  operationId: enquiry_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/tools/enquiry_delete\n  method: post\n  operationId: enquiry_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/boatvaluecalculator-com/agentic-access/boatvaluecalculator-com-agentic-access.yml
summary_line: 9 operations · 8 acting
tags:
- Boat
- Valuation
- Finance
- Marine
- Calculator
---
