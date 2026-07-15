---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 1
consequence_counts:
  read: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Datastore Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Google Cloud Datastore exposes 9 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Datastore
provider_slug: google-cloud-datastore
slug: google-cloud-datastore-agentic-access
source_filename: google-cloud-datastore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-cloud-datastore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 8\n    connected: 1\n  by_consequence:\n    write: 8\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects/{projectId}:allocateIds\n  method: post\n  operationId: allocateIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:beginTransaction\n\
  \  method: post\n  operationId: beginTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:commit\n  method: post\n  operationId: commit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:lookup\n  method: post\n  operationId: lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:reserveIds\n  method: post\n  operationId: reserveIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:rollback\n  method: post\n  operationId: rollback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n\
  \    - datastore\n- path: /v1/projects/{projectId}:runQuery\n  method: post\n  operationId: runQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}:runAggregationQuery\n  method: post\n  operationId: runAggregationQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - datastore\n- path: /v1/projects/{projectId}/operations\n  method: get\n  operationId: listOperations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - datastore\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-datastore/refs/heads/main/agentic-access/google-cloud-datastore-agentic-access.yml
summary_line: 9 operations · 8 acting
tags:
- NoSQL
- Database
- Document Database
- Google Cloud
- Firestore
- Managed Service
- Key-Value Store
---
