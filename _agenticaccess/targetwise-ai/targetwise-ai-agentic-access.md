---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: targetwise-ai-account-api-openapi.yml
  format: yaml
  label: targetwise-ai Account API
  slug: targetwise-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-account-api-openapi.yml
- filename: targetwise-ai-autocomplete-api-openapi.yml
  format: yaml
  label: targetwise-ai Autocomplete API
  slug: targetwise-ai-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-autocomplete-api-openapi.yml
- filename: targetwise-ai-companies-api-openapi.yml
  format: yaml
  label: targetwise-ai Companies API
  slug: targetwise-ai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-companies-api-openapi.yml
- filename: targetwise-ai-employees-api-openapi.yml
  format: yaml
  label: targetwise-ai Employees API
  slug: targetwise-ai-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-employees-api-openapi.yml
- filename: targetwise-ai-enrichment-api-openapi.yml
  format: yaml
  label: targetwise-ai Enrichment API
  slug: targetwise-ai-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-enrichment-api-openapi.yml
- filename: targetwise-ai-prospecting-api-openapi.yml
  format: yaml
  label: targetwise-ai Prospecting API
  slug: targetwise-ai-prospecting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-prospecting-api-openapi.yml
- filename: targetwise-ai-resolution-api-openapi.yml
  format: yaml
  label: targetwise-ai Resolution API
  slug: targetwise-ai-resolution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/targetwise-ai/openapi/targetwise-ai-resolution-api-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Targetwise Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'targetwise-ai exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: targetwise-ai
provider_slug: targetwise-ai
slug: targetwise-ai-agentic-access
source_filename: targetwise-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/targetwise-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/prospecting/companies/search\n  method: post\n  operationId: targetwise_search_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prospecting/contacts/search\n  method: post\n  operationId: targetwise_search_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/enrich\n  method: post\n  operationId: targetwise_enrich_company\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contacts/enrich\n  method: post\n  operationId: targetwise_enrich_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contacts/find-work-email\n  method: post\n  operationId: targetwise_find_work_email\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/contacts/find-phone\n  method: post\n  operationId: targetwise_find_phone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reverse-email\n  method: post\n  operationId: targetwise_reverse_email_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/companies/search\n  method: post\n  operationId: targetwise_find_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/employees/search\n  method: post\n  operationId: targetwise_search_employees\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/employees/details\n  method: post\n  operationId: targetwise_get_employee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/autocomplete/company\n  method: post\n  operationId: targetwise_autocomplete_company\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/status\n  method: get\n  operationId: targetwise_account_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/targetwise-ai/agentic-access/targetwise-ai-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- B2B
- Data Enrichment
- MCP
- Software-as-a-Service
---
