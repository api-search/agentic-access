---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: logrocket-rest-api-openapi.yml
  format: yaml
  label: LogRocket REST API
  slug: logrocket-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-rest-api-openapi.yml
- filename: logrocket-graphql-api-openapi.yml
  format: yaml
  label: LogRocket GraphQL API
  slug: logrocket-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-graphql-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Logrocket Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'LogRocket exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LogRocket
provider_slug: logrocket
slug: logrocket-agentic-access
source_filename: logrocket-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/logrocket-graphql-api-openapi.yml, openapi/logrocket-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /graphql\n  method: post\n  operationId: executeGraphQLQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/apps/{appId}/users/{userId}\n  method: put\n  operationId:\
  \ updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/apps/{appId}/data-export/\n  method: get\n  operationId: listDataExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/apps/{appId}/highlights/\n  method: post\n  operationId: createHighlights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/apps/{appId}/highlights/\n  method: get\n  operationId: getHighlights\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/agentic-access/logrocket-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Session Replay
- Product Analytics
- Frontend Monitoring
- Logging
- Errors
---
