---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: vincario-vin-decoder-api-openapi.yml
  format: yaml
  label: Vincario VIN Decoder API
  slug: vincario-vin-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-vin-decoder-api-openapi.yml
- filename: vincario-oem-vin-lookup-api-openapi.yml
  format: yaml
  label: Vincario OEM VIN Lookup API
  slug: vincario-oem-vin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-oem-vin-lookup-api-openapi.yml
- filename: vincario-oem-service-history-api-openapi.yml
  format: yaml
  label: Vincario OEM Service History API
  slug: vincario-oem-service-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-oem-service-history-api-openapi.yml
- filename: vincario-vehicle-market-value-api-openapi.yml
  format: yaml
  label: Vincario Vehicle Market Value API
  slug: vincario-vehicle-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-vehicle-market-value-api-openapi.yml
- filename: vincario-stolen-check-api-openapi.yml
  format: yaml
  label: Vincario Stolen Check API
  slug: vincario-stolen-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-stolen-check-api-openapi.yml
- filename: vincario-get-balance-api-openapi.yml
  format: yaml
  label: Vincario Credit Balance API
  slug: vincario-get-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-get-balance-api-openapi.yml
- filename: vincario-enums-api-openapi.yml
  format: yaml
  label: Vincario Enums API
  slug: vincario-enums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-enums-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vincario Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Vincario exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vincario
provider_slug: vincario
slug: vincario-agentic-access
source_filename: vincario-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: generated\nsource: openapi/vincario-enums-api-openapi.yml, openapi/vincario-get-balance-api-openapi.yml,\n  openapi/vincario-oem-service-history-api-openapi.yml, openapi/vincario-oem-vin-lookup-api-openapi.yml,\n  openapi/vincario-stolen-check-api-openapi.yml, openapi/vincario-vehicle-market-value-api-openapi.yml,\n  openapi/vincario-vin-decoder-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_make.{format}\n  method: get\n  operationId: Enum_Make\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_model.{format}\n  method: get\n  operationId: Enum_Model\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_make_model.{format}\n  method: get\n  operationId: Enum_Vehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_body.{format}\n  method: get\n  operationId: Enum_Body\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_color.{format}\n  method: get\n  operationId:\
  \ Enum_Color\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_drive.{format}\n  method: get\n  operationId: Enum_Drive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_fuel.{format}\n  method: get\n  operationId: Enum_Fuel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_product_type.{format}\n  method: get\n  operationId: Enum_Product_Type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/value-list/enum/enum_transmission.{format}\n\
  \  method: get\n  operationId: Enum_Transmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/balance.{format}\n  method: get\n  operationId: Get_Balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/oem/history/{VIN}.{format}\n  method: get\n  operationId: OEM_Service_History\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/oem/{VIN}.{format}\n  method: get\n  operationId: OEM_VIN_Lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/stolen-check/{VIN}.{format}\n\
  \  method: get\n  operationId: Stolen_Check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/vehicle-market-value/{VIN}.{format}\n  method: get\n  operationId: Vehicle_Market_Value\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/info/{VIN}.{format}\n  method: get\n  operationId: VIN_Decode_Info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3.2/{API_KEY}/{CONTROL_SUM}/decode/{VIN}.{format}\n  method: get\n  operationId: VIN_Decode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/agentic-access/vincario-agentic-access.yml
summary_line: 16 operations
tags:
- VIN
- Vehicle Data
- Automotive
- VIN Decoder
- Market Value
---
