---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 9
api_specs:
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Sink Consumers API
  slug: sequin-io-sink-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Postgres Databases API
  slug: sequin-io-postgres-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin HTTP Endpoints API
  slug: sequin-io-http-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Backfills API
  slug: sequin-io-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Stream Pull API
  slug: sequin-io-stream-pull-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
consequence_counts:
  read: 9
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sequin Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Sequin exposes 25 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sequin
provider_slug: sequin-io
slug: sequin-io-agentic-access
source_filename: sequin-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sequin-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 9\n    acting: 16\n  by_consequence:\n    read: 9\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /postgres_databases\n  method: get\n  operationId: listPostgresDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postgres_databases\n  method: post\n  operationId: createPostgresDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postgres_databases/{id_or_name}\n  method: get\n  operationId: getPostgresDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postgres_databases/{id_or_name}\n  method: patch\n  operationId: updatePostgresDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postgres_databases/{id_or_name}\n  method: delete\n  operationId: deletePostgresDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postgres_databases/{id_or_name}/test-connection\n  method: post\n  operationId: testPostgresDatabaseConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postgres_databases/{id_or_name}/refresh-tables\n  method: post\n  operationId: refreshPostgresDatabaseTables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sinks\n  method: get\n  operationId: listSinkConsumers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sinks\n  method: post\n  operationId: createSinkConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sinks/{id_or_name}\n  method: get\n  operationId: getSinkConsumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sinks/{id_or_name}\n  method: patch\n  operationId: updateSinkConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sinks/{id_or_name}\n  method: delete\n  operationId: deleteSinkConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/http_endpoints\n  method: get\n  operationId: listHttpEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/http_endpoints\n  method: post\n  operationId: createHttpEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/http_endpoints/{id_or_name}\n\
  \  method: get\n  operationId: getHttpEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/http_endpoints/{id_or_name}\n  method: patch\n  operationId: updateHttpEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/http_endpoints/{id_or_name}\n  method: delete\n  operationId: deleteHttpEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sinks/{sink_id_or_name}/backfills\n\
  \  method: get\n  operationId: listBackfills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sinks/{sink_id_or_name}/backfills\n  method: post\n  operationId: createBackfill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sinks/{sink_id_or_name}/backfills/{backfill_id}\n  method: get\n  operationId: getBackfill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sinks/{sink_id_or_name}/backfills/{backfill_id}\n  method: patch\n  operationId: updateBackfill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sinks/{sink_id_or_name}/backfills/{backfill_id}\n  method: delete\n  operationId: deleteBackfill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /http_pull_consumers/{consumer_name}/receive\n  method: get\n  operationId: receiveMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http_pull_consumers/{consumer_name}/ack\n  method: post\n  operationId: ackMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /http_pull_consumers/{consumer_name}/nack\n  method: post\n  operationId: nackMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/agentic-access/sequin-io-agentic-access.yml
summary_line: 25 operations · 16 acting
tags:
- Change Data Capture
- CDC
- Postgres
- Streaming
- Open Source
- Data Pipeline
---
