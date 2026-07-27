---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 18
api_specs:
- filename: itu-datahub-openapi.yml
  format: yaml
  label: ITU DataHub API
  slug: itu-datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-datahub-openapi.yml
- filename: itu-proximity-openapi.yml
  format: yaml
  label: ITU Proximity to Fibre Node API
  slug: itu-proximity-to-fibre-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/openapi/itu-proximity-openapi.yml
consequence_counts:
  read: 18
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Itu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'ITU exposes 20 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ITU
provider_slug: itu
slug: itu-agentic-access
source_filename: itu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/itu-datahub-openapi.yml, openapi/itu-proximity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 18\n    acting: 2\n  by_consequence:\n    read: 18\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /country/all\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /region/all\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dictionaries/getcategories\n\
  \  method: get\n  operationId: getIndicatorCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dictionaries/getbyid/{codeID}\n  method: get\n  operationId: getIndicatorById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/bycode/{codeID}\n  method: get\n  operationId: getDataByCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/bycode/{codeID}/byiso/{iso}\n  method: get\n  operationId: getDataByCodeAndIso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregation/bycodeid/{codeID}/byregionid/{regionID}\n  method: get\n  operationId: getRegionalAggregate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/all\n  method: get\n  operationId: listDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idi/dashboard/all\n  method: get\n  operationId: getIdiStructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idi/dashboard/version\n  method: get\n  operationId: listIdiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idi/data/bycountryid/{countryID}\n  method: get\n  operationId: getIdiByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /idi/region/byregionid/{regionID}\n  method: get\n  operationId: getIdiByRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umc/dashboard/all\n  method: get\n  operationId: getUmcDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umc/topic/all\n  method: get\n  operationId: listUmcTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umc/macro/all\n  method: get\n  operationId: listUmcMacros\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umc/target/all\n  method: get\n  operationId: listUmcTargets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umc/bycountryid/{countryID}\n  method: get\n  operationId: getUmcByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /methodology/dataset\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route-calcdistancetonode\n  method: post\n  operationId: calcDistanceToNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /route-calc10kmintersection\n  method: post\n  operationId:\
  \ calc10kmIntersection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itu/refs/heads/main/agentic-access/itu-agentic-access.yml
summary_line: 20 operations · 2 acting
tags:
- Telecommunications
- Global
- Regulator
- Standards
- Spectrum
- Satellite
- Broadband
- ICT Statistics
- Open Data
- United Nations
---
