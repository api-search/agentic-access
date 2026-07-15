---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: brella-openapi.yml
  format: yaml
  label: Brella Events API
  slug: brella-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Attendees API
  slug: brella-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Speakers API
  slug: brella-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Sponsors API
  slug: brella-sponsors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Schedule API
  slug: brella-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
- filename: brella-openapi.yml
  format: yaml
  label: Brella Invites API
  slug: brella-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/openapi/brella-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brella Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Brella exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brella
provider_slug: brella
slug: brella-agentic-access
source_filename: brella-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/brella-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /organizations/{organizationId}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/events/{eventId}/attendees\n  method: get\n  operationId: listAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/events/{eventId}/speakers\n\
  \  method: get\n  operationId: listSpeakers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/events/{eventId}/sponsors\n  method: get\n  operationId: listSponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/events/{eventId}/timeslots\n  method: get\n  operationId: listTimeslots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/events/{eventId}/invites\n  method: get\n  operationId: listInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brella/refs/heads/main/agentic-access/brella-agentic-access.yml
summary_line: 6 operations
tags:
- Events
- Event Networking
- Matchmaking
- Event Platform
- Attendees
- Engagement
- Conferences
- SaaS
---
