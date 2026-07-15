---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 9
api_specs:
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Connections API
  slug: decodable-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Streams API
  slug: decodable-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Pipelines API
  slug: decodable-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Secrets API
  slug: decodable-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
- filename: decodable-openapi.yml
  format: yaml
  label: Decodable Resources API
  slug: decodable-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/openapi/decodable-openapi.yml
consequence_counts:
  read: 9
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Decodable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Decodable exposes 26 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Decodable
provider_slug: decodable
slug: decodable-agentic-access
source_filename: decodable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/decodable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 9\n    acting: 17\n  by_consequence:\n    read: 9\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /v1alpha2/connections/\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/connections/\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/connections/{connection_id}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/connections/{connection_id}\n  method: put\n  operationId: updateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/connections/{connection_id}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/connections/{connection_id}/activate\n  method: post\n  operationId: activateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/connections/{connection_id}/deactivate\n  method: post\n  operationId: deactivateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/streams/\n  method: get\n  operationId: listStreams\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/streams/\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/streams/{stream_id}\n  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/streams/{stream_id}\n  method: put\n  operationId: updateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v1alpha2/streams/{stream_id}\n  method: delete\n  operationId: deleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/streams/{stream_id}/preview/token\n  method: post\n  operationId: createStreamPreviewToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/pipelines/\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/pipelines/\n\
  \  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/pipelines/{pipeline_id}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/pipelines/{pipeline_id}\n  method: put\n  operationId: updatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/pipelines/{pipeline_id}\n  method: delete\n  operationId: deletePipeline\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/pipelines/{pipeline_id}/activate\n  method: post\n  operationId: activatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/pipelines/{pipeline_id}/deactivate\n  method: post\n  operationId: deactivatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v1alpha2/secrets/\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/secrets/\n  method: post\n  operationId: createSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/secrets/{secret_id}\n  method: get\n  operationId: getSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha2/secrets/{secret_id}\n  method: put\n  operationId: updateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/secrets/{secret_id}\n  method: delete\n  operationId: deleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha2/accounts/{account_name}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decodable/refs/heads/main/agentic-access/decodable-agentic-access.yml
summary_line: 26 operations · 17 acting
tags:
- Stream Processing
- Apache Flink
- Debezium
- Real Time Data
- Data Pipelines
- CDC
---
