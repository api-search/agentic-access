---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 19
api_specs:
- filename: department-of-transportation-airport-status-api-openapi.yml
  format: yaml
  label: Department of Transportation Airport Status API
  slug: department-of-transportation-airport-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-airport-status-api-openapi.yml
- filename: department-of-transportation-authority-api-openapi.yml
  format: yaml
  label: Department of Transportation Authority API
  slug: department-of-transportation-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-authority-api-openapi.yml
- filename: department-of-transportation-carriers-api-openapi.yml
  format: yaml
  label: Department of Transportation Carriers API
  slug: department-of-transportation-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-carriers-api-openapi.yml
- filename: department-of-transportation-complaints-api-openapi.yml
  format: yaml
  label: Department of Transportation Complaints API
  slug: department-of-transportation-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-complaints-api-openapi.yml
- filename: department-of-transportation-crashes-api-openapi.yml
  format: yaml
  label: Department of Transportation Crashes API
  slug: department-of-transportation-crashes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-crashes-api-openapi.yml
- filename: department-of-transportation-inspections-api-openapi.yml
  format: yaml
  label: Department of Transportation Inspections API
  slug: department-of-transportation-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-inspections-api-openapi.yml
- filename: department-of-transportation-makes-api-openapi.yml
  format: yaml
  label: Department of Transportation Makes API
  slug: department-of-transportation-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-makes-api-openapi.yml
- filename: department-of-transportation-manufacturers-api-openapi.yml
  format: yaml
  label: Department of Transportation Manufacturers API
  slug: department-of-transportation-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-manufacturers-api-openapi.yml
- filename: department-of-transportation-models-api-openapi.yml
  format: yaml
  label: Department of Transportation Models API
  slug: department-of-transportation-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-models-api-openapi.yml
- filename: department-of-transportation-ratings-api-openapi.yml
  format: yaml
  label: Department of Transportation Ratings API
  slug: department-of-transportation-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-ratings-api-openapi.yml
- filename: department-of-transportation-recalls-api-openapi.yml
  format: yaml
  label: Department of Transportation Recalls API
  slug: department-of-transportation-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-recalls-api-openapi.yml
- filename: department-of-transportation-vehicle-variables-api-openapi.yml
  format: yaml
  label: Department of Transportation Vehicle Variables API
  slug: department-of-transportation-vehicle-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vehicle-variables-api-openapi.yml
- filename: department-of-transportation-vin-decode-api-openapi.yml
  format: yaml
  label: Department of Transportation VIN Decode API
  slug: department-of-transportation-vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vin-decode-api-openapi.yml
- filename: department-of-transportation-wmi-api-openapi.yml
  format: yaml
  label: Department of Transportation WMI API
  slug: department-of-transportation-wmi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-wmi-api-openapi.yml
consequence_counts:
  read: 19
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Department Of Transportation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Department of Transportation exposes 20 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Department of Transportation
provider_slug: department-of-transportation
slug: department-of-transportation-agentic-access
source_filename: department-of-transportation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/faa-system-status-api-openapi.yml, openapi/fmcsa-qcmobile-api-openapi.yml, openapi/nhtsa-recalls-api-openapi.yml,\n  openapi/nhtsa-vpic-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 19\n    acting: 1\n  by_consequence:\n    read: 19\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{airportCode}\n  method: get\n  operationId: getAirportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}\n  method: get\n  operationId: getCarrierByDotNumber\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/name/{name}\n  method: get\n  operationId: getCarriersByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/docket-number/{docketNumber}\n  method: get\n  operationId: getCarrierByDocket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/authority\n  method: get\n  operationId: getAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/inspections\n  method: get\n  operationId: getInspections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/crashes\n  method: get\n  operationId: getCrashes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recalls/recallsByVehicle\n  method: get\n  operationId: getRecallsByVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recalls/campaignNumber\n  method: get\n  operationId: getRecallByCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/complaintsByVehicle\n  method: get\n  operationId: getComplaintsByVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SafetyRatings/modelyear/{modelYear}/make/{make}/model/{model}\n\
  \  method: get\n  operationId: getSafetyRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/DecodeVin/{vin}\n  method: get\n  operationId: decodeVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/DecodeVinValues/{vin}\n  method: get\n  operationId: decodeVinValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/DecodeVINValuesBatch/\n  method: post\n  operationId: decodeVinBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /vehicles/GetAllMakes\n  method: get\n  operationId: getAllMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/GetModelsForMake/{makeName}\n  method: get\n  operationId: getModelsForMake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/GetModelsForMakeYear/make/{make}/modelyear/{year}\n  method: get\n  operationId: getModelsForMakeYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/GetAllManufacturers\n  method: get\n  operationId: getAllManufacturers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/DecodeWMI/{wmi}\n\
  \  method: get\n  operationId: decodeWmi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/GetVehicleVariableList\n  method: get\n  operationId: getVehicleVariableList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/agentic-access/department-of-transportation-agentic-access.yml
summary_line: 20 operations · 1 acting
tags:
- Federal-Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
---
