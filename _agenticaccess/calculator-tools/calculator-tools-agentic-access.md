---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: calculator-tools-openai-api-openapi.yml
  format: yaml
  label: Calculator Tools Openai API
  slug: calculator-tools-openai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculator-tools/openapi/calculator-tools-openai-api-openapi.yml
consequence_counts:
  physical: 1
  read: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Calculator Tools Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openai/webapp/edit/
operation_count: 5
overview: 'Calculator Tools exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Calculator Tools
provider_slug: calculator-tools
slug: calculator-tools-agentic-access
source_filename: calculator-tools-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/calculator-tools-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 3\n    read: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /openai/webapp/create/\n  method: post\n  operationId: webappCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/webapp/list/\n  method: post\n  operationId: webappList\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/webapp/html/\n  method: post\n  operationId: webappHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/webapp/edit/\n  method: post\n  operationId: webappEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/webapp/logo/\n  method: post\n  operationId: webappLogo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/calculator-tools/agentic-access/calculator-tools-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Artificial Intelligence
- No-Code
- Platform
- Calculator
- Tools
- Automation
---
