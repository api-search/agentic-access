---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 28
api_specs:
- filename: thanos-query-api.yml
  format: yaml
  label: Thanos Query API
  slug: thanos-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-query-api.yml
- filename: thanos-store-gateway-openapi.yml
  format: yaml
  label: Thanos Store Gateway API
  slug: thanos-store-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-store-gateway-openapi.yml
- filename: thanos-sidecar-openapi.yml
  format: yaml
  label: Thanos Sidecar API
  slug: thanos-sidecar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-sidecar-openapi.yml
- filename: thanos-ruler-openapi.yml
  format: yaml
  label: Thanos Ruler API
  slug: thanos-ruler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-ruler-openapi.yml
- filename: thanos-receive-openapi.yml
  format: yaml
  label: Thanos Receive API
  slug: thanos-receive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-receive-openapi.yml
- filename: thanos-compact-openapi.yml
  format: yaml
  label: Thanos Compact API
  slug: thanos-compact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/openapi/thanos-compact-openapi.yml
consequence_counts:
  read: 28
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thanos Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Thanos exposes 31 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Thanos
provider_slug: thanos
slug: thanos-agentic-access
source_filename: thanos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thanos-compact-openapi.yml, openapi/thanos-query-api.yml, openapi/thanos-receive-openapi.yml,\n  openapi/thanos-ruler-openapi.yml, openapi/thanos-sidecar-openapi.yml, openapi/thanos-store-gateway-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 28\n    acting: 3\n  by_consequence:\n    read: 28\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /-/healthy\n  method: get\n  operationId: getCompactHealthy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/ready\n  method: get\n  operationId: getCompactReady\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getCompactMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/blocks\n  method: get\n  operationId: listCompactBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query\n  method: get\n  operationId: instantQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query\n  method: post\n  operationId: instantQueryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/query_range\n  method: get\n  operationId: rangeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query_range\n  method: post\n  operationId: rangeQueryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/series\n  method: get\n  operationId: getSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/labels\n  method: get\n  operationId: getLabels\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/label/{label_name}/values\n  method: get\n  operationId: getLabelValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/targets\n  method: get\n  operationId: getTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rules\n  method: get\n  operationId: getRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/alerts\n  method: get\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores\n\
  \  method: get\n  operationId: getStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/healthy\n  method: get\n  operationId: getReceiveHealthy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/ready\n  method: get\n  operationId: getReceiveReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getReceiveMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receive\n  method: post\n  operationId: remoteWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /-/healthy\n  method: get\n  operationId: getRulerHealthy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/ready\n  method: get\n  operationId: getRulerReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getRulerMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rules\n  method: get\n  operationId: getRulerRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/alerts\n  method: get\n  operationId: getRulerAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/healthy\n  method: get\n  operationId: getSidecarHealthy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/ready\n  method: get\n  operationId: getSidecarReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getSidecarMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/healthy\n  method: get\n  operationId: getStoreHealthy\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/ready\n  method: get\n  operationId: getStoreReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getStoreMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/blocks\n  method: get\n  operationId: listStoreBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/agentic-access/thanos-agentic-access.yml
summary_line: 31 operations · 3 acting
tags:
- Metrics
- Monitoring
- Observability
- Prometheus
- Time Series Database
---
