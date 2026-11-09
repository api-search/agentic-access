---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 3
api_specs:
- filename: damagerestorehq-com-dataset-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Dataset API
  slug: damagerestorehq-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-dataset-api-openapi.yml
- filename: damagerestorehq-com-enquiry-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Enquiry API
  slug: damagerestorehq-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-enquiry-api-openapi.yml
- filename: damagerestorehq-com-entities-api-openapi.yml
  format: yaml
  label: damagerestorehq-com Entities API
  slug: damagerestorehq-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-entities-api-openapi.yml
- filename: damagerestorehq-com-mcp-api-openapi.yml
  format: yaml
  label: damagerestorehq-com MCP API
  slug: damagerestorehq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damagerestorehq-com/openapi/damagerestorehq-com-mcp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 3
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Damagerestorehq Com Agentic Access
name_suffix: Agentic Access
notable_actions:
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
operation_count: 17
overview: 'damagerestorehq-com exposes 17 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: damagerestorehq-com
provider_slug: damagerestorehq-com
slug: damagerestorehq-com-agentic-access
source_filename: damagerestorehq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/damagerestorehq-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 14\n    connected: 3\n  by_consequence:\n    write: 12\n    read: 3\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/dataset_columns\n  method: post\n  operationId: dataset_columns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_search\n  method: post\n  operationId: dataset_search\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/tools/dataset_row\n  method: post\n  operationId: dataset_row\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_compare\n  method: post\n  operationId: dataset_compare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_stats\n  method: post\n  operationId: dataset_stats\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_top\n  method: post\n  operationId: dataset_top\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_provenance\n  method: post\n  operationId: dataset_provenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/entities_schema\n  method: post\n  operationId:\
  \ entities_schema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/entity_lookup\n  method: post\n  operationId: entity_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/entities_search\n  method: post\n  operationId: entities_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/tools/entities_in\n  method: post\n  operationId: entities_in\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/entities_export\n  method: post\n  operationId: entities_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/submit_enquiry\n  method: post\n  operationId: submit_enquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/damagerestorehq-com/agentic-access/damagerestorehq-com-agentic-access.yml
summary_line: 17 operations · 14 acting
tags:
- WaterDamage
- Insurance
- Restoration
- US
- Data
---
