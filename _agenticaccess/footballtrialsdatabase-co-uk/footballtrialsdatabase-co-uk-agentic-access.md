---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: footballtrialsdatabase-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Football Trials Database Enquiry API
  slug: footballtrialsdatabase-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-enquiry-api-openapi.yml
- filename: footballtrialsdatabase-co-uk-guide-api-openapi.yml
  format: yaml
  label: Football Trials Database Guide API
  slug: footballtrialsdatabase-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-guide-api-openapi.yml
- filename: footballtrialsdatabase-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Football Trials Database MCP API
  slug: footballtrialsdatabase-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/openapi/footballtrialsdatabase-co-uk-mcp-api-openapi.yml
consequence_counts:
  physical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Footballtrialsdatabase Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp/tools/enquiry_describe
operation_count: 5
overview: 'Football Trials Database exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Football Trials Database
provider_slug: footballtrialsdatabase-co-uk
slug: footballtrialsdatabase-co-uk-agentic-access
source_filename: footballtrialsdatabase-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/footballtrialsdatabase-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/checker_start\n  method: post\n  operationId: checker_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/checker_answer\n  method: post\n  operationId: checker_answer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/checker_tree\n  method: post\n  operationId: checker_tree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/footballtrialsdatabase-co-uk/agentic-access/footballtrialsdatabase-co-uk-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- football trials
- academy recruitment
- non‑league clubs
- county FA
- paid trial events
---
