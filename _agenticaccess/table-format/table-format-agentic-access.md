---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 7
api_specs:
- filename: rest-catalog-open-api.yaml
  format: yaml
  label: Apache Iceberg REST Catalog API
  slug: apache-iceberg-rest-catalog
  spec_type: OpenAPI
  url: https://github.com/apache/iceberg/blob/main/open-api/rest-catalog-open-api.yaml
- filename: all.yaml
  format: yaml
  label: Unity Catalog
  slug: unity-catalog
  spec_type: OpenAPI
  url: https://github.com/unitycatalog/unitycatalog/blob/main/api/all.yaml
consequence_counts:
  read: 7
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Table Format Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Table Format exposes 18 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Table Format
provider_slug: table-format
slug: table-format-agentic-access
source_filename: table-format-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apache-iceberg-rest-catalog-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 7\n    acting: 11\n  by_consequence:\n    read: 7\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/oauth/tokens\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/namespaces\n  method: post\n  operationId: createNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}\n  method: get\n  operationId: loadNamespaceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n   \
  \ scope:\n    - catalog\n- path: /v1/namespaces/{namespace}\n  method: delete\n  operationId: dropNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/properties\n  method: post\n  operationId: updateNamespaceProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables/{table}\n  method: get\n  operationId: loadTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables/{table}\n  method: post\n  operationId: commitTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables/{table}\n  method: delete\n  operationId: dropTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/tables/{table}/metrics\n  method: post\n  operationId: reportMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/views\n  method: get\n  operationId: listViews\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/views\n  method: post\n  operationId: createView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/views/{view}\n  method: get\n  operationId: loadView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - catalog\n- path: /v1/namespaces/{namespace}/views/{view}\n  method: delete\n  operationId: dropView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n- path: /v1/transactions/commit\n  method: post\n  operationId: commitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - catalog\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/agentic-access/table-format-agentic-access.yml
summary_line: 18 operations · 11 acting
tags:
- Data Lakehouse
- Open Table Format
- Apache Iceberg
- Delta Lake
- Apache Hudi
- Data Lake
- ACID Transactions
- Schema Evolution
- Time Travel
---
