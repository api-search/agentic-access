---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: compliapi-com-screen-api-openapi.yml
  format: yaml
  label: compliapi-com Screen API
  slug: compliapi-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compliapi-com/openapi/compliapi-com-screen-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Compliapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'compliapi-com exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: compliapi-com
provider_slug: compliapi-com
slug: compliapi-com-agentic-access
source_filename: compliapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/compliapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /screen/lists\n  method: get\n  operationId: screening_lists_screen_lists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screen/lists/{slug}/entities\n  method: get\n  operationId: screening_list_entities_screen_lists__slug__entities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /screen/crypto/{address}\n  method: get\n  operationId: screen_crypto_screen_crypto__address__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screen/email/{email}\n  method: get\n  operationId: screen_email_screen_email__email__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screen/website\n  method: get\n  operationId: screen_website_screen_website_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screen/id/{government_id}\n  method: get\n  operationId: screen_government_id_screen_id__government_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /screen/pep\n  method: get\n  operationId: screen_pep_screen_pep_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screen/country/{country}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/compliapi-com/agentic-access/compliapi-com-agentic-access.yml
summary_line: 8 operations
tags:
- Compliance
- Sanctions
- Screening
- Fintech
- Cryptocurrency
---
