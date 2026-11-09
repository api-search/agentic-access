---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: filingfirehose-com-billing-api-openapi.yml
  format: yaml
  label: filingfirehose-com Billing API
  slug: filingfirehose-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingfirehose-com/openapi/filingfirehose-com-billing-api-openapi.yml
- filename: filingfirehose-com-filings-api-openapi.yml
  format: yaml
  label: filingfirehose-com Filings API
  slug: filingfirehose-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingfirehose-com/openapi/filingfirehose-com-filings-api-openapi.yml
- filename: filingfirehose-com-meta-api-openapi.yml
  format: yaml
  label: filingfirehose-com Meta API
  slug: filingfirehose-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingfirehose-com/openapi/filingfirehose-com-meta-api-openapi.yml
- filename: filingfirehose-com-public-api-openapi.yml
  format: yaml
  label: filingfirehose-com Public API
  slug: filingfirehose-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingfirehose-com/openapi/filingfirehose-com-public-api-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filingfirehose Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'filingfirehose-com exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: filingfirehose-com
provider_slug: filingfirehose-com
slug: filingfirehose-com-agentic-access
source_filename: filingfirehose-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/filingfirehose-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 1\n    connected: 7\n  by_consequence:\n    write: 1\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/billing/stripe-webhook\n  method: post\n  operationId: stripe_webhook_v1_billing_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/8k\n  method: get\n  operationId: public_8k_v1_public_8k_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/13d\n  method: get\n  operationId: public_13d_v1_public_13d_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/atm\n  method: get\n  operationId: public_atm_v1_public_atm_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/8-k\n  method: get\n  operationId: get_8k_filings_v1_filings_8_k_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/s3\n  method: get\n  operationId: get_s3_filings_v1_filings_s3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/13d\n  method: get\n  operationId: get_13_filings_v1_filings_13d_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filingfirehose-com/agentic-access/filingfirehose-com-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- SEC
- EDGAR
- Finance
- Data API
- JSON
---
