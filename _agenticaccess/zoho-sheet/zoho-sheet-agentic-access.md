---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: openapi.yml
  format: yaml
  label: Zoho Sheet Data API
  slug: zoho-sheet-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sheet/refs/heads/main/openapi/openapi.yml
consequence_counts:
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Zoho Sheet Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{resource_id}
operation_count: 1
overview: 'Zoho Sheet exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoho Sheet
provider_slug: zoho-sheet
slug: zoho-sheet-agentic-access
source_filename: zoho-sheet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /{resource_id}\n  method: post\n  operationId: dispatchSheetOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - ZohoSheet.dataAPI.READ\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-sheet/refs/heads/main/agentic-access/zoho-sheet-agentic-access.yml
summary_line: 1 operation · 1 acting · 1 human-in-the-loop
tags:
- Spreadsheets
- Productivity
- Collaboration
- Data
- Office
- Zoho
---
