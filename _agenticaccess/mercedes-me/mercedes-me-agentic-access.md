---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 34
api_specs:
- filename: mercedes-me-configurator-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Car Configurator API
  slug: mercedes-me-car-configurator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-configurator-api-openapi.yml
- filename: mercedes-me-dealer-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Dealer API
  slug: mercedes-me-dealer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-dealer-api-openapi.yml
- filename: mercedes-me-vehicle-images-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Vehicle Images API
  slug: mercedes-me-vehicle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-vehicle-images-api-openapi.yml
- filename: mercedes-me-remote-diagnostic-support-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Remote Diagnostic Support API
  slug: mercedes-me-remote-diagnostic-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-remote-diagnostic-support-api-openapi.yml
consequence_counts:
  read: 34
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Mercedes Me Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vehicles/{vehicleId}/ecuReadouts
operation_count: 39
overview: 'Mercedes-Benz Mercedes me exposes 39 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mercedes-Benz Mercedes me
provider_slug: mercedes-me
slug: mercedes-me-agentic-access
source_filename: mercedes-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mercedes-me-configurator-api-openapi.yml, openapi/mercedes-me-dealer-api-openapi.yml,\n  openapi/mercedes-me-remote-diagnostic-support-api-openapi.yml, openapi/mercedes-me-vehicle-images-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 34\n    acting: 5\n  by_consequence:\n    read: 34\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /markets\n  method: get\n  operationId: marketsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}\n  method: get\n  operationId:\
  \ marketGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/bodies\n  method: get\n  operationId: bodiesGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/bodies/{bodyId}\n  method: get\n  operationId: bodyGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/classes\n  method: get\n  operationId: classesGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/classes/{classId}\n  method: get\n  operationId: classGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models\n  method: get\n  operationId: modelsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}\n  method: get\n  operationId: modelGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/initial\n  method: get\n  operationId: modelConfigurationsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}\n  method: get\n  operationId: modelConfigurationGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/alternatives/{componentList}\n  method: get\n  operationId: modelConfigurationAlternativesGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components\n  method: get\n  operationId: imageComponentsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/engine\n  method: get\n  operationId: imageComponentsEngineGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/equipments\n  method: get\n  operationId: imageComponentsEquipmentsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/equipments/{componentCode}\n  method: get\n  operationId: imageComponentsEquipmentsByCodeGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/paint\n  method: get\n  operationId: imageComponentsPaintGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/rim\n\
  \  method: get\n  operationId: imageComponentsRimGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/trim\n  method: get\n  operationId: imageComponentsTrimGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/components/upholstery\n  method: get\n  operationId: imageComponentsUpholsteryGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/images/vehicle\n  method: get\n  operationId: imageVehicleGET\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/models/{modelId}/configurations/{configurationId}/selectables\n  method: get\n  operationId: modelConfigurationSelectablesGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{marketId}/onlinecode\n  method: post\n  operationId: onlineCodePOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /markets/{marketId}/onlinecode/{onlineCode}\n  method: get\n  operationId: onlineCodeGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /markets/{marketId}/productgroups\n  method: get\n  operationId: productGroupsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries\n  method: get\n  operationId: countriesGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealers\n  method: get\n  operationId: dealersGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealers/{dealerId}\n  method: get\n  operationId: dealerGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{vehicleId}/dtcReadouts\n  method: post\n  operationId: getDtcDataListByEcuUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{vehicleId}/ecuId/{ecuId}/dtcId/{dtcId}/dtcSnapshotReadouts\n  method: post\n  operationId: getDtcSnapshotReadoutsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{vehicleId}/ecuReadouts\n  method: post\n  operationId: getEcuDataListByVehicleIdUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n    \
  \  proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vehicles/{vehicleId}/resourceReadouts\n  method: post\n  operationId: getResourceReadoutsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{finorvin}/components\n  method: get\n  operationId: imageComponentsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/engine\n  method: get\n  operationId: imageComponentsEngineGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/equipments\n\
  \  method: get\n  operationId: imageComponentsEquipmentsGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/paint\n  method: get\n  operationId: imageComponentsPaintGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/rim\n  method: get\n  operationId: imageComponentsRimGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/trim\n  method: get\n  operationId: imageComponentsTrimGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/components/upholstery\n  method: get\n  operationId: imageComponentsUpholsteryGET\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{finorvin}/vehicle\n  method: get\n  operationId: imageVehicleGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/agentic-access/mercedes-me-agentic-access.yml
summary_line: 39 operations · 5 acting · 1 human-in-the-loop
tags:
- Automotive
- Connected Car
- Connected Vehicle
- Daimler
- Fleet Management
- Mercedes me
- Mercedes-Benz
- OEM
- Telematics
- Vehicle Data
---
