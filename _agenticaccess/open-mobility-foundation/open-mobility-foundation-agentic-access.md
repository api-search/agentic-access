---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 29
api_specs:
- filename: open-mobility-foundation-events-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Events API
  slug: open-mobility-foundation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-events-api-openapi.yml
- filename: open-mobility-foundation-geographies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies API
  slug: open-mobility-foundation-geographies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-api-openapi.yml
- filename: open-mobility-foundation-geographies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies.json API
  slug: open-mobility-foundation-geographies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-json-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions API
  slug: open-mobility-foundation-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions.json API
  slug: open-mobility-foundation-jurisdictions-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-json-api-openapi.yml
- filename: open-mobility-foundation-metrics-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Metrics API
  slug: open-mobility-foundation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-metrics-api-openapi.yml
- filename: open-mobility-foundation-policies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies API
  slug: open-mobility-foundation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-api-openapi.yml
- filename: open-mobility-foundation-policies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies.json API
  slug: open-mobility-foundation-policies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-json-api-openapi.yml
- filename: open-mobility-foundation-reports-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Reports API
  slug: open-mobility-foundation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-reports-api-openapi.yml
- filename: open-mobility-foundation-requirements-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Requirements API
  slug: open-mobility-foundation-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-requirements-api-openapi.yml
- filename: open-mobility-foundation-stops-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Stops API
  slug: open-mobility-foundation-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-stops-api-openapi.yml
- filename: open-mobility-foundation-telemetry-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Telemetry API
  slug: open-mobility-foundation-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-telemetry-api-openapi.yml
- filename: open-mobility-foundation-trips-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Trips API
  slug: open-mobility-foundation-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-trips-api-openapi.yml
- filename: open-mobility-foundation-value-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Value API
  slug: open-mobility-foundation-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-value-api-openapi.yml
- filename: open-mobility-foundation-vehicles-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Vehicles API
  slug: open-mobility-foundation-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-vehicles-api-openapi.yml
consequence_counts:
  read: 29
  safety-critical: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Open Mobility Foundation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stops
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /stops
operation_count: 38
overview: 'Open Mobility Foundation exposes 38 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 7 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open Mobility Foundation
provider_slug: open-mobility-foundation
slug: open-mobility-foundation-agentic-access
source_filename: open-mobility-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/open-mobility-foundation-mds-agency-openapi.yml, openapi/open-mobility-foundation-mds-geography-openapi.yml,\n  openapi/open-mobility-foundation-mds-jurisdiction-openapi.yml, openapi/open-mobility-foundation-mds-metrics-openapi.yml,\n  openapi/open-mobility-foundation-mds-policy-openapi.yml, openapi/open-mobility-foundation-mds-provider-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    acting: 9\n    connected: 29\n  by_consequence:\n    write: 7\n    read: 29\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /vehicles\n  method: post\n  operationId: post-vehicles\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles\n  method: put\n  operationId: put-vehicles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles\n  method: get\n  operationId: get-vehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{device_id}\n  method: get\n  operationId: get-vehicles-device_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /vehicles/status\n  method: get\n  operationId: get-vehicles-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/status/{device_id}\n  method: get\n  operationId: get-vehicles-status-device_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: post\n  operationId: post-trips\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /telemetry\n  method: post\n  operationId: post-telemetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: post-events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stops\n  method: post\n  operationId: post-stops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stops\n  method: put\n  operationId: put-stops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stops\n  method: get\n  operationId: get-stops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops/{stop_id}\n  method: get\n  operationId: get-stops-stop_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: post\n  operationId: post-reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geographies\n\
  \  method: get\n  operationId: get-geographies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographies/{geography_id}\n  method: get\n  operationId: get-geographies-geography_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographies.json\n  method: get\n  operationId: get-geographies.json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jurisdictions\n  method: get\n  operationId: get-jurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jurisdictions/{jurisdiction_id}\n  method: get\n  operationId: get-jurisdictions-jurisdiction_id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jurisdictions.json\n  method: get\n  operationId: get-jurisdictions.json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: get-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: post\n  operationId: post-metrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies\n  method: get\n  operationId: get-policies\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policy_id}\n  method: get\n  operationId: get-policies-policy_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies.json\n  method: get\n  operationId: get-policies.json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /value\n  method: get\n  operationId: get-value\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requirements\n  method: get\n  operationId: get-requirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n \
  \ method: get\n  operationId: get-vehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{device_id}\n  method: get\n  operationId: get-vehicles-device_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/status\n  method: get\n  operationId: get-vehicles-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/status/{device_id}\n  method: get\n  operationId: get-vehicles-status-device_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: get\n  operationId: get-trips-end_time\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /telemetry\n  method: get\n  operationId: get-telemetry-telemetry_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/historical\n  method: get\n  operationId: get-events-historical-event_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/recent\n  method: get\n  operationId: get-events-recent-start_time-end_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops\n  method: get\n  operationId: get-stops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /stops/{stop_id}\n  method: get\n  operationId: get-stops-stop_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{filename}\n  method: get\n  operationId: get-reports-filename\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/agentic-access/open-mobility-foundation-agentic-access.yml
summary_line: 38 operations · 9 acting · 2 human-in-the-loop
tags:
- Company
- Mobility
- Open Source
- Open Standards
- Transportation
- Cities
- Micromobility
- Data Specifications
---
