---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Sessions API
  slug: veriff-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Decisions API
  slug: veriff-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Person API
  slug: veriff-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Media API
  slug: veriff-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Watchlist Screening API
  slug: veriff-watchlist-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Attempts API
  slug: veriff-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Webhooks API
  slug: veriff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Veriff Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Veriff exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Veriff
provider_slug: veriff-com
slug: veriff-com-agentic-access
source_filename: veriff-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/veriff-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 5\n    connected: 7\n  by_consequence:\n    write: 5\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: patch\n  operationId: updateSession\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/media\n  method: get\n  operationId:\
  \ getSessionMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/collected-data\n  method: post\n  operationId: uploadCollectedData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/decision\n  method: get\n  operationId: getSessionDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/person\n  method: get\n  operationId: getSessionPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sessions/{sessionId}/watchlist-screening\n  method: get\n  operationId: getWatchlistScreening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/attempts\n  method: get\n  operationId: getSessionAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attempts/{attemptId}/media\n  method: get\n  operationId: getAttemptMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{mediaId}\n  method: get\n  operationId: getMediaFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/agentic-access/veriff-com-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Identity Verification
- KYC
- AML
- Biometrics
- Document Verification
- Fraud Prevention
---
