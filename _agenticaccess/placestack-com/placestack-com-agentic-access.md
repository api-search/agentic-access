---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 29
api_specs:
- filename: placestack-com-account-api-openapi.yml
  format: yaml
  label: placestack-com Account API
  slug: placestack-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-account-api-openapi.yml
- filename: placestack-com-case-api-openapi.yml
  format: yaml
  label: placestack-com Case API
  slug: placestack-com-case-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-case-api-openapi.yml
- filename: placestack-com-event-api-openapi.yml
  format: yaml
  label: placestack-com Event API
  slug: placestack-com-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-event-api-openapi.yml
- filename: placestack-com-jurisdiction-api-openapi.yml
  format: yaml
  label: placestack-com Jurisdiction API
  slug: placestack-com-jurisdiction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-jurisdiction-api-openapi.yml
- filename: placestack-com-list-api-openapi.yml
  format: yaml
  label: placestack-com List API
  slug: placestack-com-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-list-api-openapi.yml
- filename: placestack-com-monitor-api-openapi.yml
  format: yaml
  label: placestack-com Monitor API
  slug: placestack-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-monitor-api-openapi.yml
- filename: placestack-com-parcel-api-openapi.yml
  format: yaml
  label: placestack-com Parcel API
  slug: placestack-com-parcel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-parcel-api-openapi.yml
- filename: placestack-com-permit-api-openapi.yml
  format: yaml
  label: placestack-com Permit API
  slug: placestack-com-permit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-permit-api-openapi.yml
- filename: placestack-com-suggestion-api-openapi.yml
  format: yaml
  label: placestack-com Suggestion API
  slug: placestack-com-suggestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-suggestion-api-openapi.yml
- filename: placestack-com-usage-api-openapi.yml
  format: yaml
  label: placestack-com Usage API
  slug: placestack-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-usage-api-openapi.yml
- filename: placestack-com-webhook-api-openapi.yml
  format: yaml
  label: placestack-com Webhook API
  slug: placestack-com-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-webhook-api-openapi.yml
- filename: placestack-com-zoning-api-openapi.yml
  format: yaml
  label: placestack-com Zoning API
  slug: placestack-com-zoning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placestack-com/openapi/placestack-com-zoning-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Placestack Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhook/{webhook}/delivery
operation_count: 43
overview: 'placestack-com exposes 43 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 13 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: placestack-com
provider_slug: placestack-com
slug: placestack-com-agentic-access
source_filename: placestack-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/placestack-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 29\n    acting: 14\n  by_consequence:\n    read: 29\n    write: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/parcel\n  method: get\n  operationId: list_parcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcel/batch\n  method: post\n  operationId: create_parcel_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcel/{parcel_id}\n  method: get\n  operationId: get_parcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list\n  method: get\n  operationId: list_saved_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list\n  method: post\n  operationId: post_saved_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/list/{list_id}\n  method: get\n  operationId: get_saved_list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list/{list_id}\n  method: patch\n  operationId: patch_saved_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/list/{list_id}\n  method: delete\n  operationId: delete_saved_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/list/{list_id}/item\n  method: get\n  operationId: list_saved_list_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list/{list_id}/item\n  method: post\n  operationId: post_saved_list_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/list/{list_id}/item/{item_id}\n  method: get\n  operationId: get_saved_list_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list/{list_id}/item/{item_id}\n  method: patch\n  operationId: patch_saved_list_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/list/{list_id}/item/{item_id}\n  method: delete\n  operationId: delete_saved_list_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tag\n  method: get\n  operationId: list_tag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitor\n  method: get\n  operationId: list_monitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitor\n  method: post\n  operationId: post_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/{monitor_id}\n  method: get\n  operationId: get_monitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitor/{monitor_id}\n  method: patch\n  operationId: patch_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/{monitor_id}\n  method: delete\n  operationId: delete_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event\n  method: get\n  operationId: list_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event/{event_id}\n  method: get\n  operationId: get_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suggestion\n  method: get\n  operationId: list_suggestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jurisdiction\n  method: get\n  operationId: list_jurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jurisdiction/{jurisdiction_id}\n  method:\
  \ get\n  operationId: get_jurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/zoning\n  method: get\n  operationId: search_zoning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/zoning/{zoning_id}\n  method: get\n  operationId: get_zoning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/permit\n  method: get\n  operationId: search_permit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/permit/{permit_id}\n  method: get\n  operationId: get_permit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/case\n  method: get\n  operationId: search_case\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/case/{case_id}\n  method: get\n  operationId: get_case\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: read_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit\n  method: get\n  operationId: read_credit\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/request\n  method: get\n  operationId: list_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_type\n  method: get\n  operationId: list_event_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: get\n  operationId: list_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: post_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /webhook/{webhook}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/{webhook}\n  method: patch\n  operationId: patch_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/{webhook}\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/{webhook}/delivery\n\
  \  method: get\n  operationId: list_delivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/{webhook}/delivery\n  method: post\n  operationId: post_delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/{webhook}/delivery/{delivery}\n  method: get\n  operationId: get_delivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/placestack-com/agentic-access/placestack-com-agentic-access.yml
summary_line: 43 operations · 14 acting
tags:
- Company
- Real Estate
- Data
- Geospatial
- Property
---
