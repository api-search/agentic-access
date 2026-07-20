---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: leeo-insurance-services-fleet-openapi.yml
  format: yaml
  label: LEEO Fleet Telematics API
  slug: leeo-insurance-services-fleet-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/openapi/leeo-insurance-services-fleet-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Leeo Insurance Services Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'LEEO Insurance Services exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LEEO Insurance Services
provider_slug: leeo-insurance-services
slug: leeo-insurance-services-agentic-access
source_filename: leeo-insurance-services-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/leeo-insurance-services-fleet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /drivers\n  method: get\n  operationId: listDrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/{driver_id}/trips\n  method: get\n  operationId: listDriverTrips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trip/trip_id/{trip_id}\n  method: get\n\
  \  operationId: getTripByTripId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trip/tracking_id/{tracking_id}\n  method: get\n  operationId: getTripByTrackingId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver-aggregate/daily\n  method: get\n  operationId: getDailyDriverAggregate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver-aggregate/weekly\n  method: get\n  operationId: getWeeklyDriverAggregate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getReportLink\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/agentic-access/leeo-insurance-services-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Insurance
- Insurtech
- Commercial Auto Insurance
- Telematics
- Fleet Management
- Driving Behavior
- Risk Management
- Managing General Agent
- Mobile SDK
---
