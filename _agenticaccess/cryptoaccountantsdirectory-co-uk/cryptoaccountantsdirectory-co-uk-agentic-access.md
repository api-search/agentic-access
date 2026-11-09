---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: cryptoaccountantsdirectory-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory Enquiry API
  slug: cryptoaccountantsdirectory-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-enquiry-api-openapi.yml
- filename: cryptoaccountantsdirectory-co-uk-guide-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory Guide API
  slug: cryptoaccountantsdirectory-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-guide-api-openapi.yml
- filename: cryptoaccountantsdirectory-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory MCP API
  slug: cryptoaccountantsdirectory-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-mcp-api-openapi.yml
consequence_counts:
  physical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cryptoaccountantsdirectory Co Uk Agentic Access
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
operation_count: 6
overview: 'Crypto Accountants Directory exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crypto Accountants Directory
provider_slug: cryptoaccountantsdirectory-co-uk
slug: cryptoaccountantsdirectory-co-uk-agentic-access
source_filename: cryptoaccountantsdirectory-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cryptoaccountantsdirectory-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    write: 4\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/compare_criteria\n  method: post\n  operationId: compare_criteria\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/compare_options\n  method: post\n  operationId: compare_options\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/compare_table\n  method: post\n  operationId: compare_table\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/enquiry_describe\n  method: post\n  operationId: enquiry_describe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /mcp/tools/enquiry_fields\n  method: post\n  operationId: enquiry_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/submit_enquiry\n  method: post\n  operationId: submit_enquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/agentic-access/cryptoaccountantsdirectory-co-uk-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- Company
- Cryptocurrency
- Accounting
- United Kingdom
- Tax
---
