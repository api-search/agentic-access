---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 18
api_specs:
- filename: aquabyte-behaviour-api-openapi.yml
  format: yaml
  label: Aquabyte Behaviour API
  slug: aquabyte-behaviour-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-behaviour-api-openapi.yml
- filename: aquabyte-biomass-api-openapi.yml
  format: yaml
  label: Aquabyte Biomass API
  slug: aquabyte-biomass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-biomass-api-openapi.yml
- filename: aquabyte-environmental-api-openapi.yml
  format: yaml
  label: Aquabyte Environmental API
  slug: aquabyte-environmental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-environmental-api-openapi.yml
- filename: aquabyte-lice-api-openapi.yml
  format: yaml
  label: Aquabyte Lice API
  slug: aquabyte-lice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-lice-api-openapi.yml
- filename: aquabyte-sites-api-openapi.yml
  format: yaml
  label: Aquabyte Sites API
  slug: aquabyte-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-sites-api-openapi.yml
- filename: aquabyte-v3-0-api-openapi.yml
  format: yaml
  label: Aquabyte V3.0 API
  slug: aquabyte-v3-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-v3-0-api-openapi.yml
- filename: aquabyte-welfare-api-openapi.yml
  format: yaml
  label: Aquabyte Welfare API
  slug: aquabyte-welfare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-welfare-api-openapi.yml
consequence_counts:
  read: 18
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aquabyte Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Aquabyte exposes 19 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aquabyte
provider_slug: aquabyte
slug: aquabyte-agentic-access
source_filename: aquabyte-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/aquabyte-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 18\n    acting: 1\n  by_consequence:\n    read: 18\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /sites\n  method: get\n  operationId: get_sites_sites_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{siteId}\n  method: get\n  operationId: get_sites_siteId_sites__siteId__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environmental\n\
  \  method: get\n  operationId: get_environmental_environmental_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/environmental\n  method: get\n  operationId: get_environmental_deprecated_pens__penId__environmental_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/environmental/latest\n  method: get\n  operationId: get_environmental_latest_pens__penId__environmental_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environmental/latest\n  method: get\n  operationId: get_environmental_latest_all_pens_environmental_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /biomass\n  method: get\n  operationId: get_biomass_daily_biomass_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/biomass\n  method: get\n  operationId: get_biomass_daily_deprecated_pens__penId__biomass_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biomass/harvestReport\n  method: get\n  operationId: get_biomass_harvest_report_biomass_harvestReport_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/biomass/harvestReport\n  method: get\n  operationId: get_biomass_harvest_report_deprecated_pens__penId__biomass_harvestReport_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/liceCount\n  method: get\n  operationId: get_pen_lice_count_deprecated_pens__penId__liceCount_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liceCount\n  method: get\n  operationId: get_pen_lice_count_liceCount_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/behavior/swimSpeed\n  method: get\n  operationId: get_behavior_swim_speed_deprecated_pens__penId__behavior_swimSpeed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /behaviour/swimSpeed\n  method: get\n  operationId: get_behavior_swim_speed_behaviour_swimSpeed_get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/behavior/breathingIndex\n  method: get\n  operationId: get_behavior_breathing_index_deprecated_pens__penId__behavior_breathingIndex_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /behaviour/breathingIndex\n  method: get\n  operationId: get_behavior_breathing_index_behaviour_breathingIndex_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /welfareScores\n  method: get\n  operationId: get_pen_welfare_data_welfareScores_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pens/{penId}/welfareScores\n  method: get\n  operationId:\
  \ get_pen_welfare_data_deprecated_pens__penId__welfareScores_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /superiorRate\n  method: post\n  operationId: get_pen_superior_rate_superiorRate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/agentic-access/aquabyte-agentic-access.yml
summary_line: 19 operations · 1 acting
tags:
- Aquaculture
- Fish Farming
- Computer Vision
- Machine Learning
- Biomass Estimation
- Sea Lice
- Fish Welfare
- Environmental Monitoring
- Agriculture Technology
- Norway
- Salmon
- Data
---
