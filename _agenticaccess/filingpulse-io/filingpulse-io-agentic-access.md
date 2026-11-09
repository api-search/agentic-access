---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: filingpulse-io-account-api-openapi.yml
  format: yaml
  label: FilingPulse Account API
  slug: filingpulse-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-account-api-openapi.yml
- filename: filingpulse-io-events-api-openapi.yml
  format: yaml
  label: FilingPulse Events API
  slug: filingpulse-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-events-api-openapi.yml
- filename: filingpulse-io-filings-api-openapi.yml
  format: yaml
  label: FilingPulse Filings API
  slug: filingpulse-io-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-filings-api-openapi.yml
- filename: filingpulse-io-meta-api-openapi.yml
  format: yaml
  label: FilingPulse Meta API
  slug: filingpulse-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-meta-api-openapi.yml
- filename: filingpulse-io-registrations-api-openapi.yml
  format: yaml
  label: FilingPulse Registrations API
  slug: filingpulse-io-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-registrations-api-openapi.yml
- filename: filingpulse-io-signup-api-openapi.yml
  format: yaml
  label: FilingPulse Signup API
  slug: filingpulse-io-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-signup-api-openapi.yml
- filename: filingpulse-io-webhooks-api-openapi.yml
  format: yaml
  label: FilingPulse Webhooks API
  slug: filingpulse-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filingpulse Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/signup
operation_count: 14
overview: 'FilingPulse exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FilingPulse
provider_slug: filingpulse-io
slug: filingpulse-io-agentic-access
source_filename: filingpulse-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/filingpulse-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schema\n  method: get\n  operationId: schema_v1_schema_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n\
  \  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insider-trades\n  method: get\n  operationId: insider_trades_v1_insider_trades_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insider-trades/{accession}\n  method: get\n  operationId: insider_trade_v1_insider_trades__accession__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signup\n  method: post\n  operationId: signup_endpoint_v1_signup_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/registrations\n  method: get\n  operationId: registrations_v1_registrations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registrations/{accession}\n  method: get\n  operationId: registration_v1_registrations__accession__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: list_webhooks_v1_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: create_webhook_v1_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{sub_id}\n  method: delete\n  operationId: delete_webhook_v1_webhooks__sub_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{sub_id}/deliveries\n  method: get\n  operationId: webhook_deliveries_v1_webhooks__sub_id__deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: events_v1_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filingpulse-io/agentic-access/filingpulse-io-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- SEC EDGAR
- Regulatory Filings
- Insider Trading
- Form 4
- 8-K
- S-1 / IPO Registrations
- Financial Data
- Webhooks
- REST API
- MCP Server
---
