---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: audd-recognition-api-openapi.yml
  format: yaml
  label: AudD Recognition API
  slug: audd-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-recognition-api-openapi.yml
- filename: audd-custom-catalog-api-openapi.yml
  format: yaml
  label: AudD Custom Catalog API
  slug: audd-custom-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-custom-catalog-api-openapi.yml
- filename: audd-streams-api-openapi.yml
  format: yaml
  label: AudD Streams API
  slug: audd-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-streams-api-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Audd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'AudD exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AudD
provider_slug: audd
slug: audd-agentic-access
source_filename: audd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: searched\nsource: openapi/audd-custom-catalog-api-openapi.yml, openapi/audd-recognition-api-openapi.yml, openapi/audd-streams-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting\n  point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\nnote: 'Curated 2026-10-08 on AudD''s correction (api@audd.io, 2026-10-07): \"Recognition requests don''t modify anything on\n  our side, so they shouldn''t be labelled as write actions.\" recognize (POST /) and recognizeEnterprise (POST enterprise.audd.io/)\n  are classified read, like recognizeGet; the stream and custom-catalog operations, which change account state, stay write.'\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n\
  - path: /upload/\n  method: post\n  operationId: customCatalogAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: recognize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: recognizeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprise/\n  method: post\n  operationId: recognizeEnterprise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setCallbackUrl/\n  method:\
  \ post\n  operationId: setCallbackUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getCallbackUrl/\n  method: post\n  operationId: getCallbackUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addStream/\n  method: post\n  operationId: addStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getStreams/\n  method: post\n  operationId: getStreams\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setStreamUrl/\n  method: post\n  operationId: setStreamUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteStream/\n  method: post\n  operationId: deleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /longpoll/\n  method: get\n  operationId: longpoll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/agentic-access/audd-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Music
- Music Recognition
- Audio
- Fingerprinting
---
