---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: agenthelpnetwork-com-feedback-api-openapi.yml
  format: yaml
  label: agenthelpnetwork-com Feedback API
  slug: agenthelpnetwork-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthelpnetwork-com/openapi/agenthelpnetwork-com-feedback-api-openapi.yml
- filename: agenthelpnetwork-com-health-api-openapi.yml
  format: yaml
  label: agenthelpnetwork-com Health API
  slug: agenthelpnetwork-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthelpnetwork-com/openapi/agenthelpnetwork-com-health-api-openapi.yml
- filename: agenthelpnetwork-com-incidents-api-openapi.yml
  format: yaml
  label: agenthelpnetwork-com Incidents API
  slug: agenthelpnetwork-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthelpnetwork-com/openapi/agenthelpnetwork-com-incidents-api-openapi.yml
- filename: agenthelpnetwork-com-observations-api-openapi.yml
  format: yaml
  label: agenthelpnetwork-com Observations API
  slug: agenthelpnetwork-com-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthelpnetwork-com/openapi/agenthelpnetwork-com-observations-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agenthelpnetwork Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'agenthelpnetwork-com exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agenthelpnetwork-com
provider_slug: agenthelpnetwork-com
slug: agenthelpnetwork-com-agentic-access
source_filename: agenthelpnetwork-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agenthelpnetwork-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/incidents/check\n  method: get\n  operationId: check_incident_v1_incidents_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/feedback\n  method: post\n  operationId: lookup_feedback_v1_feedback_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/incidents\n  method: get\n  operationId: list_incidents_v1_incidents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/incidents/{incident_id}\n  method: get\n  operationId: incident_detail_v1_incidents__incident_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations\n  method: post\n  operationId: report_observation_v1_observations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/observations/{observation_id}\n  method: delete\n  operationId: delete_observation_v1_observations__observation_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agenthelpnetwork-com/agentic-access/agenthelpnetwork-com-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Company
---
