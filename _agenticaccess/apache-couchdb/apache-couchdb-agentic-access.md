---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 10
api_specs:
- filename: apache-couchdb-authentication-api-openapi.yml
  format: yaml
  label: Apache CouchDB Authentication API
  slug: apache-couchdb-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-authentication-api-openapi.yml
- filename: apache-couchdb-changes-api-openapi.yml
  format: yaml
  label: Apache CouchDB Changes API
  slug: apache-couchdb-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-changes-api-openapi.yml
- filename: apache-couchdb-cluster-api-openapi.yml
  format: yaml
  label: Apache CouchDB Cluster API
  slug: apache-couchdb-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-cluster-api-openapi.yml
- filename: apache-couchdb-database-api-openapi.yml
  format: yaml
  label: Apache CouchDB Database API
  slug: apache-couchdb-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-database-api-openapi.yml
- filename: apache-couchdb-design-documents-api-openapi.yml
  format: yaml
  label: Apache CouchDB Design Documents API
  slug: apache-couchdb-design-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-design-documents-api-openapi.yml
- filename: apache-couchdb-documents-api-openapi.yml
  format: yaml
  label: Apache CouchDB Documents API
  slug: apache-couchdb-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-documents-api-openapi.yml
- filename: apache-couchdb-mango-api-openapi.yml
  format: yaml
  label: Apache CouchDB Mango API
  slug: apache-couchdb-mango-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-mango-api-openapi.yml
- filename: apache-couchdb-replication-api-openapi.yml
  format: yaml
  label: Apache CouchDB Replication API
  slug: apache-couchdb-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-replication-api-openapi.yml
- filename: apache-couchdb-server-api-openapi.yml
  format: yaml
  label: Apache CouchDB Server API
  slug: apache-couchdb-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-server-api-openapi.yml
consequence_counts:
  read: 10
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apache Couchdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Apache CouchDB exposes 21 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apache CouchDB
provider_slug: apache-couchdb
slug: apache-couchdb-agentic-access
source_filename: apache-couchdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apache-couchdb-http-api-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 10\n    acting: 11\n  by_consequence:\n    read: 10\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getServerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_all_dbs\n  method: get\n  operationId: getAllDbs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_session\n  method: get\n  operationId:\
  \ getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_session\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}\n  method: get\n  operationId: getDatabaseInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{db}\n  method: put\n  operationId: createDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}\n  method: delete\n  operationId: deleteDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_all_docs\n  method: get\n  operationId: getAllDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{db}/_all_docs\n  method: post\n  operationId: bulkGetDocs\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/{docid}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{db}/{docid}\n  method: put\n  operationId: createOrUpdateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/{docid}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_bulk_docs\n  method: post\n  operationId: bulkDocs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_find\n  method: post\n  operationId: findDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_index\n  method: get\n  operationId: getIndexes\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{db}/_index\n  method: post\n  operationId: createIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_changes\n  method: get\n  operationId: getChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_replicate\n  method: post\n  operationId: replicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{db}/_design/{ddoc}/_view/{view}\n\
  \  method: get\n  operationId: getView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_cluster_setup\n  method: get\n  operationId: getClusterSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/agentic-access/apache-couchdb-agentic-access.yml
summary_line: 21 operations · 11 acting
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open-Source
- Replication
- REST
---
