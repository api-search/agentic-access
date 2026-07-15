---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments General Payments API
  slug: open-payments-general-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Research Payments API
  slug: open-payments-research-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Ownership and Investment API
  slug: open-payments-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Datastore Query API
  slug: open-payments-datastore-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Metastore and Search API
  slug: open-payments-metastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Open Payments Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'CMS Open Payments exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CMS Open Payments
provider_slug: open-payments
slug: open-payments-agentic-access
source_filename: open-payments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/open-payments-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /metastore/schemas/dataset/items\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metastore/schemas/dataset/items/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /search\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastore/query/{datasetId}/{index}\n  method: get\n  operationId: queryDatastoreByDatasetGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastore/query/{datasetId}/{index}\n  method: post\n  operationId: queryDatastoreByDatasetPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datastore/query/{distributionId}\n  method: post\n  operationId: queryDatastoreByDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datastore/query/{datasetId}/{index}/download\n  method: get\n  operationId: downloadDatastore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastore/sql\n  method: get\n  operationId: queryDatastoreSql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/agentic-access/open-payments-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Government Data
- Healthcare
- Open Data
- Transparency
- Payments
- Clinical Data
- Physicians
- Open Government
- Public Sector
---
