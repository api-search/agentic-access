---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Negotiated Rates
  slug: negotiated-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Rate Search
  slug: rate-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Benchmarks
  slug: benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Payerset Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Payerset exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Payerset
provider_slug: payerset
slug: payerset-agentic-access
source_filename: payerset-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/payerset-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/rates/rate_query\n  method: get\n  operationId: queryRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/payers/payer_detail\n  method: get\n  operationId: getPayerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/payers/payer_list\n  method:\
  \ get\n  operationId: getPayerList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/providers/npi_detail\n  method: get\n  operationId: getNpiDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/providers/npi_to_tin\n  method: get\n  operationId: getNpiToTin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/providers/tin_to_npi\n  method: get\n  operationId: getTinToNpi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/providers/npi_to_parent\n  method: get\n  operationId: getNpiToParent\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/providers/npi_parent\n  method: get\n  operationId: getNpiParent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/billing_codes/code_detail\n  method: get\n  operationId: getBillingCodeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/billing_codes/code_types\n  method: get\n  operationId: getBillingCodeTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hospital_mrf/hospital_list\n  method: get\n  operationId: getHospitalList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hospital_mrf/system_list\n  method: get\n  operationId: getSystemList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hospital_mrf/payer_list\n  method: get\n  operationId: getHospitalPayerList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/agentic-access/payerset-agentic-access.yml
summary_line: 13 operations
tags:
- Healthcare
- Price Transparency
- Negotiated Rates
- Machine-Readable Files
- Payer Data
---
