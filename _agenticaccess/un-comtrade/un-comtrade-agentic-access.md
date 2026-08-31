---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: un-comtrade-bulk-download-api-openapi.yml
  format: yaml
  label: UN Comtrade Bulk Download API
  slug: un-comtrade-bulk-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-bulk-download-api-openapi.yml
- filename: un-comtrade-data-availability-api-openapi.yml
  format: yaml
  label: UN Comtrade Data Availability API
  slug: un-comtrade-data-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-data-availability-api-openapi.yml
- filename: un-comtrade-final-trade-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Final Trade Data API
  slug: un-comtrade-final-trade-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-final-trade-data-api-openapi.yml
- filename: un-comtrade-public-preview-api-openapi.yml
  format: yaml
  label: UN Comtrade Public Preview API
  slug: un-comtrade-public-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-public-preview-api-openapi.yml
- filename: un-comtrade-reference-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Reference Data API
  slug: un-comtrade-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-reference-data-api-openapi.yml
- filename: un-comtrade-tariffline-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Tariffline Data API
  slug: un-comtrade-tariffline-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-tariffline-data-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Un Comtrade Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'UN Comtrade exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UN Comtrade
provider_slug: un-comtrade
slug: un-comtrade-agentic-access
source_filename: un-comtrade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /public/v1/preview/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: previewFinalTradeData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/getMetadata\n  method: get\n  operationId: previewMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/getDA/{typeCode}/{freqCode}/{clCode}\n\
  \  method: get\n  operationId: previewDataAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/get/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: getFinalTradeData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/getTariffline/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: getTarifflineData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/getDa/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: getDataAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/getDaTariffline/{typeCode}/{freqCode}/{clCode}\n\
  \  method: get\n  operationId: getDataAvailabilityTariffline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/getLiveUpdate\n  method: get\n  operationId: getLiveUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/getMetadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/v1/get/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: bulkGetTradeData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/v1/getTariffline/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: bulkGetTarifflineData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/v1/getClassic/{typeCode}/{freqCode}/{clCode}\n  method: get\n  operationId: bulkGetClassicData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/v1/app/reference/country_groups.json\n  method: get\n  operationId: getReferenceCountryGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/agentic-access/un-comtrade-agentic-access.yml
summary_line: 13 operations
tags:
- Trade
- International Trade
- Import
- Export
- Statistics
- United Nations
- Economics
- Commodities
- Bilateral Trade
- HS Codes
- SITC
---
