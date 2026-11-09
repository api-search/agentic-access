---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: dentalsoftwarecompare-com-enquiry-api-openapi.yml
  format: yaml
  label: Dental Software Compare Enquiry API
  slug: dentalsoftwarecompare-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-enquiry-api-openapi.yml
- filename: dentalsoftwarecompare-com-guide-api-openapi.yml
  format: yaml
  label: Dental Software Compare Guide API
  slug: dentalsoftwarecompare-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-guide-api-openapi.yml
- filename: dentalsoftwarecompare-com-mcp-api-openapi.yml
  format: yaml
  label: Dental Software Compare MCP API
  slug: dentalsoftwarecompare-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-mcp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dentalsoftwarecompare Com Agentic Access
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
operation_count: 8
overview: 'Dental Software Compare exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dental Software Compare
provider_slug: dentalsoftwarecompare-com
slug: dentalsoftwarecompare-com-agentic-access
source_filename: dentalsoftwarecompare-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dentalsoftwarecompare-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 5\n    physical: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/compare_criteria\n  method: post\n  operationId: compare_criteria\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/compare_options\n  method: post\n  operationId: compare_options\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/compare_table\n  method: post\n  operationId: compare_table\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/submit_enquiry\n  method: post\n  operationId: submit_enquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dentalsoftwarecompare-com/agentic-access/dentalsoftwarecompare-com-agentic-access.yml
summary_line: 8 operations · 7 acting
tags:
- Company
- Dental Software
- Practice Management
- Healthcare
- NHS
- Software Comparison
- United Kingdom
- Datasets
---
