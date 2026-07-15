---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner People API
  slug: zenplanner-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Memberships API
  slug: zenplanner-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Classes API
  slug: zenplanner-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Locations API
  slug: zenplanner-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Programs API
  slug: zenplanner-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Prospects API
  slug: zenplanner-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Groups API
  slug: zenplanner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zenplanner Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Zen Planner exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zen Planner
provider_slug: zenplanner
slug: zenplanner-agentic-access
source_filename: zenplanner-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zenplanner-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}/memberships\n  method: get\n\
  \  operationId: listPersonMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes\n  method: get\n  operationId: listClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/people/{personId}/reservations\n  method: get\n  operationId: listPersonReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/people/{personId}/attendances\n  method: get\n  operationId: listPersonAttendances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs\n  method: get\n  operationId: listPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prospects\n  method: post\n  operationId: createProspect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/agentic-access/zenplanner-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Fitness
- Gym Management
- Studio Management
- Martial Arts
- Membership
- Scheduling
- Class Booking
- Daxko
---
