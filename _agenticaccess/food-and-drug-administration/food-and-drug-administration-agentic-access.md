---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: food-and-drug-administration-animal-veterinary-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Animal & Veterinary API
  slug: food-and-drug-administration-animal-veterinary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-animal-veterinary-api-openapi.yml
- filename: food-and-drug-administration-device-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Device API
  slug: food-and-drug-administration-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-device-api-openapi.yml
- filename: food-and-drug-administration-drug-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Drug API
  slug: food-and-drug-administration-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-drug-api-openapi.yml
- filename: food-and-drug-administration-food-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Food API
  slug: food-and-drug-administration-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-food-api-openapi.yml
- filename: food-and-drug-administration-other-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Other API
  slug: food-and-drug-administration-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-other-api-openapi.yml
- filename: food-and-drug-administration-tobacco-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Tobacco API
  slug: food-and-drug-administration-tobacco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-tobacco-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Food And Drug Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Food and Drug Administration exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Food and Drug Administration
provider_slug: food-and-drug-administration
slug: food-and-drug-administration-agentic-access
source_filename: food-and-drug-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openfda-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /drug/event.json\n  method: get\n  operationId: searchDrugEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug/label.json\n  method: get\n  operationId: searchDrugLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug/enforcement.json\n  method: get\n  operationId:\
  \ searchDrugEnforcement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug/ndc.json\n  method: get\n  operationId: searchDrugNDC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug/drugsfda.json\n  method: get\n  operationId: searchDrugsFDA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug/shortages.json\n  method: get\n  operationId: searchDrugShortages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/event.json\n  method: get\n  operationId: searchDeviceEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/enforcement.json\n  method: get\n  operationId: searchDeviceEnforcement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/recall.json\n  method: get\n  operationId: searchDeviceRecalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/classification.json\n  method: get\n  operationId: searchDeviceClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/510k.json\n  method: get\n  operationId: searchDevice510k\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/pma.json\n\
  \  method: get\n  operationId: searchDevicePMA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/registrationlisting.json\n  method: get\n  operationId: searchDeviceRegistrationListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/udi.json\n  method: get\n  operationId: searchDeviceUDI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/covid19serology.json\n  method: get\n  operationId: searchCovid19Serology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/enforcement.json\n  method: get\n  operationId: searchFoodEnforcement\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/event.json\n  method: get\n  operationId: searchFoodEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /animalandveterinary/event.json\n  method: get\n  operationId: searchAnimalVetEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tobacco/problem.json\n  method: get\n  operationId: searchTobaccoProblems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /other/nsde.json\n  method: get\n  operationId: searchNSDE\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /other/substance.json\n  method: get\n  operationId: searchSubstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /other/historicaldocument.json\n  method: get\n  operationId: searchHistoricalDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/agentic-access/food-and-drug-administration-agentic-access.yml
summary_line: 22 operations
tags:
- Drugs
- Devices
- Federal-Government
- Food Safety
- Public Data
- Recalls
- Adverse Events
---
