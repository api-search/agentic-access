---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: icao-geo-api-openapi.yml
  format: yaml
  label: ICAO GEO API
  slug: icao-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-geo-api-openapi.yml
- filename: icao-icao-api-openapi.yml
  format: yaml
  label: ICAO ICAO API
  slug: icao-icao-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-icao-api-openapi.yml
- filename: icao-infomation-api-openapi.yml
  format: yaml
  label: ICAO Infomation API
  slug: icao-infomation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-infomation-api-openapi.yml
- filename: icao-publication-api-openapi.yml
  format: yaml
  label: ICAO Publication API
  slug: icao-publication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-publication-api-openapi.yml
- filename: icao-safety-api-openapi.yml
  format: yaml
  label: ICAO Safety API
  slug: icao-safety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-safety-api-openapi.yml
- filename: icao-usoap-api-openapi.yml
  format: yaml
  label: ICAO USOAP API
  slug: icao-usoap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-usoap-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Icao Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'ICAO exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ICAO
provider_slug: icao
slug: icao-agentic-access
source_filename: icao-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/icao-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /doc7910\n  method: get\n  operationId: getDoc7910\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doc8585\n  method: get\n  operationId: getDoc8585\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doc8643\n  method: get\n  operationId: getDoc8643\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accidents\n  method: get\n  operationId: getAccidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eisummary-stats\n  method: get\n  operationId: getEisummaryStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /annex\n  method: get\n  operationId: getAnnex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /icao-member-states\n  method: get\n  operationId: getIcaoMemberStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: get\n\
  \  operationId: getIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iosa-registry-list\n  method: get\n  operationId: getIosaRegistryList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fir-by-location\n  method: get\n  operationId: getFirByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturer-list\n  method: get\n  operationId: getManufacturerList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Manufacturer-list-uas\n  method: get\n  operationId: getManufacturerListUas\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-stats\n  method: get\n  operationId: getProfileStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /safety-partner-stats\n  method: get\n  operationId: getSafetyPartnerStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration-states\n  method: get\n  operationId: getRegistrationStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /safety-margin-stats\n  method: get\n  operationId: getSafetyMarginStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usoap-activity-list\n\
  \  method: get\n  operationId: getUsoapActivityList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ei-stats\n  method: get\n  operationId: getEiStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregated-ei-trend-stats\n  method: get\n  operationId: getAggregatedEiTrendStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /progress-stats\n  method: get\n  operationId: getProgressStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /progress-cert-stats\n  method: get\n  operationId: getProgressCertStats\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/agentic-access/icao-agentic-access.yml
summary_line: 21 operations
tags:
- Airlines
- Airports
- Airspace
- Aviation
- Reference Data
- Standards
- United Nations
---
