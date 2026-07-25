---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: openstates-bills-api-openapi.yml
  format: yaml
  label: Open States bills API
  slug: openstates-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-bills-api-openapi.yml
- filename: openstates-committees-api-openapi.yml
  format: yaml
  label: Open States committees API
  slug: openstates-committees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-committees-api-openapi.yml
- filename: openstates-events-api-openapi.yml
  format: yaml
  label: Open States events API
  slug: openstates-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-events-api-openapi.yml
- filename: openstates-jurisdictions-api-openapi.yml
  format: yaml
  label: Open States jurisdictions API
  slug: openstates-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-jurisdictions-api-openapi.yml
- filename: openstates-metrics-api-openapi.yml
  format: yaml
  label: Open States Metrics API
  slug: openstates-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-metrics-api-openapi.yml
- filename: openstates-people-api-openapi.yml
  format: yaml
  label: Open States people API
  slug: openstates-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/openapi/openstates-people-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openstates Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Open States exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open States
provider_slug: openstates
slug: openstates-agentic-access
source_filename: openstates-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openstates-api-v3-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /jurisdictions\n  method: get\n  operationId: jurisdiction_list_jurisdictions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jurisdictions/{jurisdiction_id}\n  method: get\n  operationId: jurisdiction_detail_jurisdictions__jurisdiction_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /people\n  method: get\n  operationId: people_search_people_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people.geo\n  method: get\n  operationId: people_geo_people_geo_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills\n  method: get\n  operationId: bills_search_bills_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/ocd-bill/{openstates_bill_id}\n  method: get\n  operationId: bill_detail_by_id_bills_ocd_bill__openstates_bill_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{jurisdiction}/{session}/{bill_id}\n\
  \  method: get\n  operationId: bill_detail_bills__jurisdiction___session___bill_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /committees\n  method: get\n  operationId: committee_list_committees_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /committees/{committee_id}\n  method: get\n  operationId: committee_detail_committees__committee_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: event_list_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  operationId: event_detail_events__event_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: metrics_metrics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/agentic-access/openstates-agentic-access.yml
summary_line: 12 operations
tags:
- Government
- Legislative Data
- Civic Technology
- State Legislature
- Bills
- Legislators
- Committees
- Open Data
- REST
- GraphQL
---
