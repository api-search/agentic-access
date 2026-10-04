---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: quasar-cluster-api-openapi.yml
  format: yaml
  label: Quasar Cluster API
  slug: quasar-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-cluster-api-openapi.yml
- filename: quasar-login-api-openapi.yml
  format: yaml
  label: Quasar Login API
  slug: quasar-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-login-api-openapi.yml
- filename: quasar-max-in-buffer-size-api-openapi.yml
  format: yaml
  label: Quasar Max In Buffer Size API
  slug: quasar-max-in-buffer-size-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-max-in-buffer-size-api-openapi.yml
- filename: quasar-option-api-openapi.yml
  format: yaml
  label: Quasar Option API
  slug: quasar-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-option-api-openapi.yml
- filename: quasar-parallelism-api-openapi.yml
  format: yaml
  label: Quasar Parallelism API
  slug: quasar-parallelism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-parallelism-api-openapi.yml
- filename: quasar-prometheus-api-openapi.yml
  format: yaml
  label: Quasar Prometheus API
  slug: quasar-prometheus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-prometheus-api-openapi.yml
- filename: quasar-query-api-openapi.yml
  format: yaml
  label: Quasar Query API
  slug: quasar-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-query-api-openapi.yml
- filename: quasar-status-api-openapi.yml
  format: yaml
  label: Quasar Status API
  slug: quasar-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-status-api-openapi.yml
- filename: quasar-tables-api-openapi.yml
  format: yaml
  label: Quasar Tables API
  slug: quasar-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tables-api-openapi.yml
- filename: quasar-tags-api-openapi.yml
  format: yaml
  label: Quasar Tags API
  slug: quasar-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tags-api-openapi.yml
consequence_counts:
  read: 11
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quasar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Quasar exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quasar
provider_slug: quasar
slug: quasar-agentic-access
source_filename: quasar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/quasar-cluster-api-openapi.yml, openapi/quasar-login-api-openapi.yml, openapi/quasar-max-in-buffer-size-api-openapi.yml,\n  openapi/quasar-option-api-openapi.yml, openapi/quasar-parallelism-api-openapi.yml, openapi/quasar-prometheus-api-openapi.yml,\n  openapi/quasar-query-api-openapi.yml, openapi/quasar-status-api-openapi.yml, openapi/quasar-tables-api-openapi.yml,\n  openapi/quasar-tags-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /cluster\n  method: get\n  operationId: get-cluster\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cluster/nodes/{id}\n  method: get\n  operationId: get-node\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /option/max-in-buffer-size\n  method: get\n  operationId: get-max-in-buffer-size\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /option/parallelism\n  method: get\n  operationId: get-parallelism\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /option/max-in-buffer-size\n  method: get\n  operationId: get-max-in-buffer-size\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /option/parallelism\n  method: get\n  operationId: get-parallelism\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prometheus/read\n  method: post\n  operationId: prometheusRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prometheus/write\n  method: post\n  operationId: prometheusWrite\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: post\n  operationId: post-query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/liveness\n  method: get\n  operationId: status-liveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/readiness\n  method: get\n  operationId: status-readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{name}.csv\n  method: get\n  operationId: get-table-csv\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId: get-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/agentic-access/quasar-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- Company
- Time Series Database
- Database
- Analytics
- Infrastructure
- Real-Time Data
- Aerospace
- Finance
---
