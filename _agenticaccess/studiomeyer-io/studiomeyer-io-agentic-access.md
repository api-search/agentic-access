---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: studiomeyer-io-account-api-openapi.yml
  format: yaml
  label: studiomeyer-io Account API
  slug: studiomeyer-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-account-api-openapi.yml
- filename: studiomeyer-io-backfill-api-openapi.yml
  format: yaml
  label: studiomeyer-io Backfill API
  slug: studiomeyer-io-backfill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-backfill-api-openapi.yml
- filename: studiomeyer-io-case-study-api-openapi.yml
  format: yaml
  label: studiomeyer-io Case Study API
  slug: studiomeyer-io-case-study-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-case-study-api-openapi.yml
- filename: studiomeyer-io-consultation-api-openapi.yml
  format: yaml
  label: studiomeyer-io Consultation API
  slug: studiomeyer-io-consultation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-consultation-api-openapi.yml
- filename: studiomeyer-io-decide-api-openapi.yml
  format: yaml
  label: studiomeyer-io Decide API
  slug: studiomeyer-io-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-decide-api-openapi.yml
- filename: studiomeyer-io-docs-api-openapi.yml
  format: yaml
  label: studiomeyer-io Docs API
  slug: studiomeyer-io-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-docs-api-openapi.yml
- filename: studiomeyer-io-entity-api-openapi.yml
  format: yaml
  label: studiomeyer-io Entity API
  slug: studiomeyer-io-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-entity-api-openapi.yml
- filename: studiomeyer-io-export-api-openapi.yml
  format: yaml
  label: studiomeyer-io Export API
  slug: studiomeyer-io-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-export-api-openapi.yml
- filename: studiomeyer-io-generate-agents-json-api-openapi.yml
  format: yaml
  label: studiomeyer-io Generate Agents Json API
  slug: studiomeyer-io-generate-agents-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-generate-agents-json-api-openapi.yml
- filename: studiomeyer-io-learn-api-openapi.yml
  format: yaml
  label: studiomeyer-io Learn API
  slug: studiomeyer-io-learn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-learn-api-openapi.yml
- filename: studiomeyer-io-memory-api-openapi.yml
  format: yaml
  label: studiomeyer-io Memory API
  slug: studiomeyer-io-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-memory-api-openapi.yml
- filename: studiomeyer-io-portfolio-api-openapi.yml
  format: yaml
  label: studiomeyer-io Portfolio API
  slug: studiomeyer-io-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-portfolio-api-openapi.yml
- filename: studiomeyer-io-quote-api-openapi.yml
  format: yaml
  label: studiomeyer-io Quote API
  slug: studiomeyer-io-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-quote-api-openapi.yml
- filename: studiomeyer-io-search-api-openapi.yml
  format: yaml
  label: studiomeyer-io Search API
  slug: studiomeyer-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-search-api-openapi.yml
- filename: studiomeyer-io-services-api-openapi.yml
  format: yaml
  label: studiomeyer-io Services API
  slug: studiomeyer-io-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-services-api-openapi.yml
- filename: studiomeyer-io-studiomeyer-memory-rest-api-api-openapi.yml
  format: yaml
  label: studiomeyer-io StudioMeyer Memory REST API
  slug: studiomeyer-io-studiomeyer-memory-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-studiomeyer-memory-rest-api-api-openapi.yml
- filename: studiomeyer-io-validate-webmcp-api-openapi.yml
  format: yaml
  label: studiomeyer-io Validate Webmcp API
  slug: studiomeyer-io-validate-webmcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-validate-webmcp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Studiomeyer Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/generate-agents-json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/quote
operation_count: 18
overview: 'studiomeyer-io exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: studiomeyer-io
provider_slug: studiomeyer-io
slug: studiomeyer-io-agentic-access
source_filename: studiomeyer-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/memory-openapi.json, openapi/studiomeyer-io-openapi.json, openapi/studiomeyer-io-stripe-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  operationId: getMemoryApiInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - memory\n- path: /api/search\n  method: post\n  operationId: searchMemory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - memory\n- path: /api/learn\n  method: post\n  operationId: learnMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - memory\n- path: /api/decide\n  method: post\n  operationId: decideMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - memory\n- path: /api/entity\n  method: post\n  operationId: createMemoryEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - memory\n- path: /api/account\n  method: get\n  operationId: getMemoryAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - memory\n- path: /api/export\n  method: get\n  operationId: exportMemory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - memory\n- path: /api/backfill\n  method: post\n  operationId: backfillMemoryEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - memory\n- path: /api/v1/memory/purchase\n  method: get\n  operationId: get_purchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/portfolio\n  method: get\n  operationId: get_portfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/services\n  method: get\n  operationId: get_services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: post\n  operationId: post_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/case-study\n  method: get\n  operationId: get_case_study\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/consultation\n  method: post\n  operationId: post_consultation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate-webmcp\n  method: get\n  operationId: get_validate_webmcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/generate-agents-json\n  method: post\n  operationId: post_generate_agents_json\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/docs\n  method: get\n  operationId: get_docs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stripe/checkout-status\n  method: get\n  operationId: getCheckoutStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/studiomeyer-io/agentic-access/studiomeyer-io-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Company
- Artificial Intelligence
- Web Design
- MCP
- Mallorca
---
