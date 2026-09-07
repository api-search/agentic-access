---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 18
api_specs:
- filename: carsxe-specifications-api-openapi.yml
  format: yaml
  label: CarsXE Specifications API
  slug: carsxe-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-specifications-api-openapi.yml
- filename: carsxe-market-value-api-openapi.yml
  format: yaml
  label: CarsXE Market Value API
  slug: carsxe-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-market-value-api-openapi.yml
- filename: carsxe-plate-api-openapi.yml
  format: yaml
  label: CarsXE Plate Decoder API
  slug: carsxe-plate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-plate-api-openapi.yml
- filename: carsxe-recalls-api-openapi.yml
  format: yaml
  label: CarsXE Recalls API
  slug: carsxe-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recalls-api-openapi.yml
- filename: carsxe-history-api-openapi.yml
  format: yaml
  label: CarsXE History API
  slug: carsxe-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-history-api-openapi.yml
- filename: carsxe-images-api-openapi.yml
  format: yaml
  label: CarsXE Images API
  slug: carsxe-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-images-api-openapi.yml
- filename: carsxe-recognition-api-openapi.yml
  format: yaml
  label: CarsXE Recognition API
  slug: carsxe-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recognition-api-openapi.yml
- filename: carsxe-year-make-model-api-openapi.yml
  format: yaml
  label: CarsXE Year Make Model API
  slug: carsxe-year-make-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-year-make-model-api-openapi.yml
- filename: carsxe-lien-theft-api-openapi.yml
  format: yaml
  label: CarsXE Lien & Theft API
  slug: carsxe-lien-theft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-lien-theft-api-openapi.yml
- filename: carsxe-auth-api-openapi.yml
  format: yaml
  label: CarsXE Auth API
  slug: carsxe-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-auth-api-openapi.yml
consequence_counts:
  read: 18
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carsxe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'CarsXE exposes 22 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CarsXE
provider_slug: carsxe
slug: carsxe-agentic-access
source_filename: carsxe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/carsxe-auth-api-openapi.yml, openapi/carsxe-history-api-openapi.yml, openapi/carsxe-images-api-openapi.yml,\n  openapi/carsxe-lien-theft-api-openapi.yml, openapi/carsxe-market-value-api-openapi.yml, openapi/carsxe-plate-api-openapi.yml,\n  openapi/carsxe-recalls-api-openapi.yml, openapi/carsxe-recognition-api-openapi.yml, openapi/carsxe-specifications-api-openapi.yml,\n  openapi/carsxe-year-make-model-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 4\n    connected: 18\n  by_consequence:\n    write: 4\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth/validate\n  method: post\n  operationId: validateKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history\n  method: get\n  operationId: getVehicleHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: get\n  operationId: getVehicleImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lien-theft\n  method: get\n  operationId: getLienTheft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketvalue\n  method: get\n  operationId: getMarketValue\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/marketvalue\n  method: get\n  operationId: getMarketValueV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platedecoder\n  method: get\n  operationId: decodePlate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/us-platedecoder\n  method: get\n  operationId: decodeUsPlate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/platedecoder\n  method: get\n  operationId: decodePlateV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/recalls\n  method: get\n  operationId: getVehicleRecalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls-ymm\n  method: get\n  operationId: getRecallsByYmm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls-batch/submit\n  method: post\n  operationId: submitRecallsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recalls-batch/status\n  method: get\n  operationId: getRecallsBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/recalls-batch/results\n  method: get\n  operationId: getRecallsBatchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls-batch/download\n  method: get\n  operationId: downloadRecallsBatchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platerecognition\n  method: post\n  operationId: recognizePlate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vinocr\n  method: post\n  operationId: vinOcr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /specs\n  method: get\n  operationId: getVehicleSpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/international-vin-decoder\n  method: get\n  operationId: getInternationalVinDecoder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ymm\n  method: get\n  operationId: getYearMakeModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ymm-options\n  method: get\n  operationId: getYearMakeModelOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obdcodesdecoder\n  method: get\n  operationId: decodeObdCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/agentic-access/carsxe-agentic-access.yml
summary_line: 22 operations · 4 acting
tags:
- Automotive
- Vehicles
- VIN
- Vehicle Data
- License Plate
- OCR
- Automobiles
- Recalls
- Market Value
- Vehicle History
- Model Context Protocol
- Agents
---
