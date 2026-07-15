---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 17
api_specs:
- filename: wis2-gdc.weather.gc.ca
  format: yaml
  label: WIS2 Global Discovery Catalogue API
  slug: wis2-global-discovery-catalogue-api
  spec_type: OpenAPI
  url: https://wis2-gdc.weather.gc.ca
consequence_counts:
  read: 17
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wmo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'World Meteorological Organization exposes 21 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: World Meteorological Organization
provider_slug: wmo
slug: wmo-agentic-access
source_filename: wmo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wis2-global-discovery-catalogue-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 17\n    acting: 4\n  by_consequence:\n    read: 17\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata\n\
  \  method: get\n  operationId: describeWis2-discovery-metadataCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/items\n  method: get\n  operationId: getWis2-discovery-metadataFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/items\n  method: options\n  operationId: optionsWis2-discovery-metadataFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/items\n  method: post\n  operationId: getCQL2Wis2-discovery-metadataFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/wis2-discovery-metadata/items/{featureId}\n  method: get\n  operationId: getWis2-discovery-metadataFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/items/{featureId}\n  method: options\n  operationId: optionsWis2-discovery-metadataFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/queryables\n  method: get\n  operationId: getWis2-discovery-metadataQueryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/wis2-discovery-metadata/schema\n\
  \  method: get\n  operationId: getWis2-discovery-metadataSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getConformanceDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n  operationId: getJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{jobId}\n\
  \  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}/results\n  method: get\n  operationId: getJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi\n  method: get\n  operationId: getOpenapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes\n  method: get\n  operationId: getProcesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/pywcmp-wis2-wcmp2-ets\n  method: get\n  operationId: describePywcmp-wis2-wcmp2-etsProcess\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/pywcmp-wis2-wcmp2-ets/execution\n  method: post\n  operationId: executePywcmp-wis2-wcmp2-etsJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processes/pywcmp-wis2-wcmp2-kpi\n  method: get\n  operationId: describePywcmp-wis2-wcmp2-kpiProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/pywcmp-wis2-wcmp2-kpi/execution\n  method: post\n  operationId: executePywcmp-wis2-wcmp2-kpiJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wmo/refs/heads/main/agentic-access/wmo-agentic-access.yml
summary_line: 21 operations · 4 acting
tags:
- Weather
- Climate
- Hydrology
- Meteorology
- International Organization
- United Nations
- Open Data
---
