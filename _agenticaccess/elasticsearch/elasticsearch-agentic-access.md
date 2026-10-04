---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: elasticsearch-cat-api-openapi.yml
  format: yaml
  label: Elasticsearch Cat API
  slug: elasticsearch-cat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/openapi/elasticsearch-cat-api-openapi.yml
- filename: elasticsearch-cluster-api-openapi.yml
  format: yaml
  label: Elasticsearch Cluster API
  slug: elasticsearch-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/openapi/elasticsearch-cluster-api-openapi.yml
- filename: elasticsearch-document-api-openapi.yml
  format: yaml
  label: Elasticsearch Document API
  slug: elasticsearch-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/openapi/elasticsearch-document-api-openapi.yml
- filename: elasticsearch-index-api-openapi.yml
  format: yaml
  label: Elasticsearch Index API
  slug: elasticsearch-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/openapi/elasticsearch-index-api-openapi.yml
- filename: elasticsearch-search-api-openapi.yml
  format: yaml
  label: Elasticsearch Search API
  slug: elasticsearch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/openapi/elasticsearch-search-api-openapi.yml
consequence_counts:
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elasticsearch Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Elasticsearch exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elasticsearch
provider_slug: elasticsearch
slug: elasticsearch-agentic-access
source_filename: elasticsearch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/elasticsearch-cat-api-openapi.yml, openapi/elasticsearch-cluster-api-openapi.yml,\n  openapi/elasticsearch-document-api-openapi.yml, openapi/elasticsearch-index-api-openapi.yml,\n  openapi/elasticsearch-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /_cat/indices\n  method: get\n  operationId: catIndices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cat/nodes\n  method: get\n  operationId: catNodes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cat/health\n  method: get\n  operationId: catHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cluster/health\n  method: get\n  operationId: clusterHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cluster/state\n  method: get\n  operationId: clusterState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cluster/stats\n  method: get\n  operationId: clusterStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{index}/_doc/{id}\n  method: put\n  operationId: indexDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{index}/_doc/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{index}/_doc/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{index}/_update/{id}\n  method: post\n  operationId: updateDocument\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_bulk\n  method: post\n  operationId: bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{index}\n  method: put\n  operationId: createIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{index}\n  method: get\n  operationId: getIndex\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{index}\n  method: delete\n  operationId: deleteIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{index}\n  method: head\n  operationId: indexExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{index}/_search\n  method: get\n  operationId: searchUri\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{index}/_search\n  method: post\n  operationId: searchDsl\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/agentic-access/elasticsearch-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- Analytics
- Database
- Full-Text Search
- NoSQL
- Search
---
