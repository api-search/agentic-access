---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 6
api_specs:
- filename: swagger.json
  format: json
  label: NPR Listening
  slug: listening
  spec_type: OpenAPI
  url: https://listening.api.npr.org/v2/swagger.json
- filename: npr-station-finder-openapi-original.yml
  format: yaml
  label: NPR Station Finder
  slug: station-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-station-finder-openapi-original.yml
- filename: npr-identity-openapi-original.yml
  format: yaml
  label: NPR Identity
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-identity-openapi-original.yml
- filename: npr-authorization-openapi-original.yml
  format: yaml
  label: NPR Authorization
  slug: authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-authorization-openapi-original.yml
consequence_counts:
  read: 6
  safety-critical: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Npr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/token/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/token/revoke
operation_count: 18
overview: 'NPR exposes 18 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 10 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NPR
provider_slug: npr
slug: npr-agentic-access
source_filename: npr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/npr-authorization-openapi-original.yml, openapi/npr-identity-openapi-original.yml,\n  openapi/npr-station-finder-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 12\n    connected: 6\n  by_consequence:\n    write: 10\n    read: 6\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/authorize\n  method: get\n  operationId: getAuthorizationPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/device\n  method: post\n  operationId: generateDeviceCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/token/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/user\n  method: get\n  operationId:\
  \ getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/stations\n  method: put\n  operationId: updateStations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/following\n  method: post\n  operationId:\
  \ postFollowing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/authorize\n  method: get\n  operationId: getAuthorizationPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/device\n  method: post\n  operationId: generateDeviceCode\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/token/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/stations\n  method: put\n  operationId: updateStations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/following\n  method: post\n  operationId: postFollowing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/stations\n\
  \  method: get\n  operationId: searchStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/stations/{stationId}\n  method: get\n  operationId: getStationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npr/refs/heads/main/agentic-access/npr-agentic-access.yml
summary_line: 18 operations · 12 acting · 2 human-in-the-loop
tags:
- Media
- News
- Radio
---
