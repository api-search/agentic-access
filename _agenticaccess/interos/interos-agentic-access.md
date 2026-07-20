---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: interos-openapi.json
  format: json
  label: Interos API
  slug: interos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-openapi.json
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Interos Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Interos exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Interos
provider_slug: interos
slug: interos-agentic-access
source_filename: interos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/interos-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/search_lite\n  method: get\n  operationId: get_organizations_search_lite_v1_external_organizations_search_lite_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/organizations/{organization_id}\n  method: get\n  operationId: get_organization_profile_v1_external_organizations__organization_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization_groups\n  method: get\n  operationId: get_all_for_customer_v1_external_organization_groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization_groups/{group_id}/organizations\n  method: get\n  operationId: get_organizations_for_group_v1_external_organization_groups__group_id__organizations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{destination_organization_id}/connections\n  method: get\n  operationId: get_suppliers_for_organization_v1_external_organizations__destination_organization_id__connections_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{organization_id}/suppliers\n  method: get\n  operationId: get_suppliers_for_organization_v1_external_organizations__organization_id__suppliers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom_fields\n  method: get\n  operationId: get_custom_fields_custom_fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/static_custom_fields/values\n  method: post\n  operationId: post_organizations_static_custom_fields_values_organizations_static_custom_fields_values_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scenarios/watchlists/{watchlist_id}/organizations\n  method: get\n  operationId: get_watchlist_organizations_scenarios_watchlists__watchlist_id__organizations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/agentic-access/interos-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Company
- Enterprise
- Supply Chain
- Risk Management
- Supplier Risk
- Third-Party Risk
- Artificial Intelligence
- API
---
