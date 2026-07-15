---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: openapi.yml
  format: yaml
  label: SolarEdge Monitoring API
  slug: solar-edge-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi.yml
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Solar Edge Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'SolarEdge exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SolarEdge
provider_slug: solar-edge
slug: solar-edge-agentic-access
source_filename: solar-edge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/solar-edge-monitoring-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /sites/list\n  method: get\n  operationId: getSiteList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/details\n  method: get\n  operationId: getSiteDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/dataPeriod\n  method: get\n\
  \  operationId: getSiteDataPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/overview\n  method: get\n  operationId: getSiteOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/energy\n  method: get\n  operationId: getSiteEnergy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/timeFrameEnergy\n  method: get\n  operationId: getSiteTimeFrameEnergy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/energyDetails\n  method: get\n  operationId: getSiteEnergyDetails\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/power\n  method: get\n  operationId: getSitePower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/powerDetails\n  method: get\n  operationId: getSitePowerDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/currentPowerFlow\n  method: get\n  operationId: getSiteCurrentPowerFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/storageData\n  method: get\n  operationId: getSiteStorageData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /site/{siteId}/inventory\n  method: get\n  operationId: getSiteInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{siteId}/list\n  method: get\n  operationId: getComponentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/inverter/{serialNumber}/data\n  method: get\n  operationId: getInverterTechnicalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/{serialNumber}/changeLog\n  method: get\n  operationId: getEquipmentChangeLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/meters\n\
  \  method: get\n  operationId: getSiteMeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{siteId}/sensors\n  method: get\n  operationId: getSensorList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/envBenefits\n  method: get\n  operationId: getSiteEnvironmentalBenefits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/image\n  method: get\n  operationId: getSiteImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{siteId}/installerImage\n  method: get\n  operationId: getSiteInstallerImage\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/list\n  method: get\n  operationId: getAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version/current\n  method: get\n  operationId: getCurrentApiVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version/supported\n  method: get\n  operationId: getSupportedApiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/agentic-access/solar-edge-agentic-access.yml
summary_line: 23 operations
tags:
- Solar
- Energy
- Monitoring
- PV
- Inverter
- Renewable Energy
- IoT
---
