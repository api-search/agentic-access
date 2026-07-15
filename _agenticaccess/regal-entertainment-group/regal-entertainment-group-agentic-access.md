---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: regal-cinema-openapi.yml
  format: yaml
  label: Regal Cinema API
  slug: regal-cinema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/openapi/regal-cinema-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Regal Entertainment Group Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tickets
operation_count: 9
overview: 'regal-entertainment-group exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: regal-entertainment-group
provider_slug: regal-entertainment-group
slug: regal-entertainment-group-agentic-access
source_filename: regal-entertainment-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/regal-cinema-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /movies\n  method: get\n  operationId: listMovies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{movieId}\n  method: get\n  operationId: getMovie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /theatres\n  method: get\n\
  \  operationId: listTheatres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /theatres/{theatreId}\n  method: get\n  operationId: getTheatre\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /showtimes\n  method: get\n  operationId: listShowtimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets\n  method: post\n  operationId: purchaseTickets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /tickets/{orderId}\n  method: get\n  operationId: getTicketOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/members/{memberId}\n  method: get\n  operationId: getLoyaltyMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/members/{memberId}/credits\n  method: post\n  operationId: addLoyaltyCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/agentic-access/regal-entertainment-group-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Cinema
- Entertainment
- Movies
- Ticketing
- Loyalty
- Theatre
- Fortune 500
---
