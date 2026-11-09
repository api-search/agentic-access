---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: catchmentchecker-co-uk-guide-api-openapi.yml
  format: yaml
  label: Catchment Checker Guide API
  slug: catchmentchecker-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchmentchecker-co-uk/openapi/catchmentchecker-co-uk-guide-api-openapi.yml
- filename: catchmentchecker-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Catchment Checker MCP API
  slug: catchmentchecker-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchmentchecker-co-uk/openapi/catchmentchecker-co-uk-mcp-api-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Catchmentchecker Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Catchment Checker exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Catchment Checker
provider_slug: catchmentchecker-co-uk
slug: catchmentchecker-co-uk-agentic-access
source_filename: catchmentchecker-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/checker_start\n  method: post\n  operationId: checker_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/checker_answer\n  method: post\n  operationId: checker_answer\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/checker_tree\n  method: post\n  operationId: checker_tree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCard\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/catchmentchecker-co-uk/agentic-access/catchmentchecker-co-uk-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Education
- United Kingdom
- Schools
- Catchment
- Mapping
---
