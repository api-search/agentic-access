---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Accounts API
  slug: badger-maps-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Locations API
  slug: badger-maps-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Check-Ins API
  slug: badger-maps-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Routes API
  slug: badger-maps-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Users API
  slug: badger-maps-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Badger Maps Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Badger Maps exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Badger Maps
provider_slug: badger-maps
slug: badger-maps-agentic-access
source_filename: badger-maps-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/badger-maps-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /login/\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/users/\n  method: get\n  operationId: searchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{account_id}/\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{account_id}/\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{account_id}/\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{location_id}/\n  method: patch\n  operationId: updateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/\n  method: get\n  operationId: listCheckIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/\n  method: post\n  operationId: createCheckIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routes/\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{route_id}/\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/agentic-access/badger-maps-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Field Sales
- Route Planning
- Mapping
- CRM
- Sales Enablement
- Territory Management
---
