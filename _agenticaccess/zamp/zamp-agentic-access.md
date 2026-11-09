---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: zamp-openapi-generated.yml
  format: yaml
  label: Zamp API
  slug: zamp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/_ae-authored/zamp-openapi-generated.yml
- filename: zamp-addresses-api-openapi.yml
  format: yaml
  label: Zamp Addresses API
  slug: zamp-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-addresses-api-openapi.yml
- filename: zamp-calculations-api-openapi.yml
  format: yaml
  label: Zamp Calculations API
  slug: zamp-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-calculations-api-openapi.yml
- filename: zamp-companies-api-openapi.yml
  format: yaml
  label: Zamp Companies API
  slug: zamp-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-companies-api-openapi.yml
- filename: zamp-filings-api-openapi.yml
  format: yaml
  label: Zamp Filings API
  slug: zamp-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-filings-api-openapi.yml
- filename: zamp-registrations-api-openapi.yml
  format: yaml
  label: Zamp Registrations API
  slug: zamp-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-registrations-api-openapi.yml
- filename: zamp-tax-codes-api-openapi.yml
  format: yaml
  label: Zamp Tax Codes API
  slug: zamp-tax-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-tax-codes-api-openapi.yml
- filename: zamp-transactions-api-openapi.yml
  format: yaml
  label: Zamp Transactions API
  slug: zamp-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-transactions-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zamp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Zamp exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zamp
provider_slug: zamp
slug: zamp-agentic-access
source_filename: zamp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/zamp-addresses-api-openapi.yml, openapi/zamp-calculations-api-openapi.yml, openapi/zamp-companies-api-openapi.yml,\n  openapi/zamp-filings-api-openapi.yml, openapi/zamp-registrations-api-openapi.yml, openapi/zamp-tax-codes-api-openapi.yml,\n  openapi/zamp-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 4\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /addresses\n  method: post\n  operationId: post_addresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calculations\n  method: post\n  operationId: post_calculations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies\n  method: get\n  operationId: get_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filings\n  method: get\n  operationId: get_filings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registrations\n  method: get\n  operationId: get_registrations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-codes\n  method: get\n  operationId: get_tax_codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: delete\n  operationId: delete_transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: get_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId: post_transactions\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/zamp/agentic-access/zamp-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- Sales Tax
- Automation
- Compliance
---
