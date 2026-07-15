---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 7
api_specs:
- filename: google-pub-sub-openapi.yml
  format: yaml
  label: Google Pub/Sub
  slug: google-pub-sub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-openapi.yml
consequence_counts:
  read: 7
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Pub Sub Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Google Pub/Sub exposes 19 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Pub/Sub
provider_slug: google-pub-sub
slug: google-pub-sub-agentic-access
source_filename: google-pub-sub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-pub-sub-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 7\n    acting: 12\n  by_consequence:\n    read: 7\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects/{project}/topics\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/topics/{topic}\n  method: get\n  operationId: getTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/topics/{topic}\n  method: put\n  operationId: createTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/topics/{topic}\n  method: delete\n  operationId: deleteTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/{topic}\n  method: patch\n\
  \  operationId: updateTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/{topic}:publish\n  method: post\n  operationId: publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/subscriptions/{subscription}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/subscriptions/{subscription}\n  method: put\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/subscriptions/{subscription}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/{subscription}:pull\n  method: post\n  operationId: pull\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/{subscription}:acknowledge\n  method: post\n  operationId: acknowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/{subscription}:modifyAckDeadline\n  method: post\n  operationId: modifyAckDeadline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/snapshots\n  method: get\n  operationId: listSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/snapshots/{snapshot}\n  method: get\n  operationId: getSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/snapshots/{snapshot}\n  method: put\n  operationId: createSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/snapshots/{snapshot}\n  method: delete\n  operationId: deleteSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/schemas\n\
  \  method: get\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n- path: /v1/projects/{project}/schemas\n  method: post\n  operationId: createSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/pubsub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/agentic-access/google-pub-sub-agentic-access.yml
summary_line: 19 operations · 12 acting
tags:
- Cloud
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
- Streaming
---
