---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: dsearassessmentcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: DSEAR Assessment Cost Enquiry API
  slug: dsearassessmentcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsearassessmentcost-co-uk/openapi/dsearassessmentcost-co-uk-enquiry-api-openapi.yml
- filename: dsearassessmentcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: DSEAR Assessment Cost MCP API
  slug: dsearassessmentcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsearassessmentcost-co-uk/openapi/dsearassessmentcost-co-uk-mcp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dsearassessmentcost Co Uk Agentic Access
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
operation_count: 5
overview: 'DSEAR Assessment Cost exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DSEAR Assessment Cost
provider_slug: dsearassessmentcost-co-uk
slug: dsearassessmentcost-co-uk-agentic-access
source_filename: dsearassessmentcost-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dsearassessmentcost-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    physical: 2\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_fields\n\
  \  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/submit_enquiry\n  method: post\n  operationId: submit_enquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dsearassessmentcost-co-uk/agentic-access/dsearassessmentcost-co-uk-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Risk Assessment
- hazardous area classification
- workplace health and safety
- DSEAR consultancy
---
