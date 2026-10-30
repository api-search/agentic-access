---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: georgiaautoquotes-com-agency-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Agency API
  slug: georgiaautoquotes-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-agency-api-openapi.yml
- filename: georgiaautoquotes-com-benchmark-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Benchmark API
  slug: georgiaautoquotes-com-benchmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-benchmark-api-openapi.yml
- filename: georgiaautoquotes-com-consent-record-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Consent Record API
  slug: georgiaautoquotes-com-consent-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-consent-record-api-openapi.yml
- filename: georgiaautoquotes-com-contact-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Contact API
  slug: georgiaautoquotes-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-contact-api-openapi.yml
- filename: georgiaautoquotes-com-dataset-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Dataset API
  slug: georgiaautoquotes-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-dataset-api-openapi.yml
- filename: georgiaautoquotes-com-eligibility-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Eligibility API
  slug: georgiaautoquotes-com-eligibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-eligibility-api-openapi.yml
- filename: georgiaautoquotes-com-forget-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Forget API
  slug: georgiaautoquotes-com-forget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-forget-api-openapi.yml
- filename: georgiaautoquotes-com-join-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Join API
  slug: georgiaautoquotes-com-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-join-api-openapi.yml
- filename: georgiaautoquotes-com-prices-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Prices API
  slug: georgiaautoquotes-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-prices-api-openapi.yml
- filename: georgiaautoquotes-com-pull-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Pull API
  slug: georgiaautoquotes-com-pull-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-pull-api-openapi.yml
- filename: georgiaautoquotes-com-quotes-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Quotes API
  slug: georgiaautoquotes-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-quotes-api-openapi.yml
- filename: georgiaautoquotes-com-terms-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Terms API
  slug: georgiaautoquotes-com-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-terms-api-openapi.yml
- filename: georgiaautoquotes-com-verify-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Verify API
  slug: georgiaautoquotes-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-verify-api-openapi.yml
- filename: georgiaautoquotes-com-top-up-api-openapi.yml
  format: yaml
  label: georgiaautoquotes-com Top Up API
  slug: georgiaautoquotes-com-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiaautoquotes-com/openapi/georgiaautoquotes-com-top-up-api-openapi.yml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Georgiaautoquotes Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/forget
operation_count: 15
overview: 'georgiaautoquotes-com exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: georgiaautoquotes-com
provider_slug: georgiaautoquotes-com
slug: georgiaautoquotes-com-agentic-access
source_filename: georgiaautoquotes-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/georgiaautoquotes-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 6\n    connected: 9\n  by_consequence:\n    write: 5\n    read: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/eligibility\n  method: post\n  operationId: check_eligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes\n  method: post\n  operationId: get_quotes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact\n  method: post\n  operationId: request_agent_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/terms\n  method: get\n  operationId: data_use_terms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify/start\n  method: post\n  operationId: verify_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/verify/check\n  method: post\n  operationId: verify_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consent-record/{lead_id}\n  method: get\n  operationId: consent_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forget\n  method: post\n  operationId: forget\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/benchmark\n\
  \  method: get\n  operationId: benchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices\n  method: get\n  operationId: prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pull\n  method: get\n  operationId: pull_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/join\n  method: post\n  operationId: register_agency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agency\n  method: get\n  operationId: agency_status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dataset\n  method: get\n  operationId: market_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topup\n  method: get\n  operationId: topup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/georgiaautoquotes-com/agentic-access/georgiaautoquotes-com-agentic-access.yml
summary_line: 15 operations · 6 acting · 1 human-in-the-loop
tags:
- Company
- Insurance
- AutoQuotes
- Georgia
- AI-Integration
---
