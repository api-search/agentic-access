---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 5
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Google Cloud Logging API
  slug: google-cloud-logging-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/googleapis.com/logging/v2/openapi.yaml
consequence_counts:
  read: 5
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Logging Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Google Cloud Logging exposes 15 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
slug: google-cloud-logging-agentic-access
source_filename: google-cloud-logging-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-cloud-logging-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 10\n    connected: 5\n  by_consequence:\n    write: 10\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/entries:write\n  method: post\n  operationId: writeLogEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/entries:list\n\
  \  method: post\n  operationId: listLogEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/entries:tail\n  method: post\n  operationId: tailLogEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/entries:copy\n  method: post\n  operationId: copyLogEntries\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/buckets\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/buckets\n  method: post\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n\
  \    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{name}/bucket\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{name}/bucket\n  method: patch\n  operationId: updateBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{name}/bucket\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/sinks\n  method: get\n  operationId: listSinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/sinks\n  method: post\n  operationId: createSink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n\
  \    - logging.write\n- path: /v2/{sinkName}\n  method: get\n  operationId: getSink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{sinkName}\n  method: delete\n  operationId: deleteSink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/exclusions\n  method: get\n  operationId: listExclusions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n- path: /v2/{parent}/exclusions\n  method: post\n  operationId: createExclusion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - logging.admin\n    - logging.read\n    - logging.write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/agentic-access/google-cloud-logging-agentic-access.yml
summary_line: 15 operations · 10 acting
tags:
- Cloud
- Logging
- Monitoring
- Observability
---
