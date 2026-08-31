---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: resultid-endpoints-api-openapi.yml
  format: yaml
  label: Resultid Endpoints API
  slug: resultid-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/openapi/resultid-endpoints-api-openapi.yml
- filename: resultid-insight-endpoints-api-openapi.yml
  format: yaml
  label: Resultid Insight endpoints API
  slug: resultid-insight-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/openapi/resultid-insight-endpoints-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Resultid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Resultid exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Resultid
provider_slug: resultid
slug: resultid-agentic-access
source_filename: resultid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/resultid-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /get_insight_last_result\n  method: get\n  operationId: do_get_insight_last_result_get_insight_last_result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_all_highlights_for_tracker_value\n  method: get\n  operationId: do_get_all_highlights_for_tracker_value_get_all_highlights_for_tracker_value_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_campaign_data\n  method: get\n  operationId: do_get_campaign_data_get_campaign_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_campaign_theme_data\n  method: get\n  operationId: do_get_campaign_theme_data_get_campaign_theme_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read_insight_grid_data\n  method: get\n  operationId: do_read_insight_grid_data_read_insight_grid_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read_insight_grid_data_by_filtered_data_efs_key\n  method: get\n  operationId: do_read_insight_grid_data_by_filtered_data_efs_key_read_insight_grid_data_by_filtered_data_efs_key_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read_campaign_trend_data\n  method: get\n  operationId: do_read_campaign_trend_data_read_campaign_trend_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_unique_values_for_tracker\n  method: get\n  operationId: do_get_unique_values_for_tracker_get_unique_values_for_tracker_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_campaign_uuids\n  method: get\n  operationId: do_get_campaign_uuids_get_campaign_uuids_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/agentic-access/resultid-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- Operational Intelligence
- Analytics
- Enterprise Software
- Artificial Intelligence
- Customer Experience
- Data Integration
- Revenue Intelligence
---
