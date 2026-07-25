---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: linkerd-discovery-api-openapi.yml
  format: yaml
  label: Linkerd Discovery API
  slug: linkerd-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-discovery-api-openapi.yml
- filename: linkerd-edges-api-openapi.yml
  format: yaml
  label: Linkerd Edges API
  slug: linkerd-edges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-edges-api-openapi.yml
- filename: linkerd-gateways-api-openapi.yml
  format: yaml
  label: Linkerd Gateways API
  slug: linkerd-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-gateways-api-openapi.yml
- filename: linkerd-health-api-openapi.yml
  format: yaml
  label: Linkerd Health API
  slug: linkerd-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-health-api-openapi.yml
- filename: linkerd-lifecycle-api-openapi.yml
  format: yaml
  label: Linkerd Lifecycle API
  slug: linkerd-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-lifecycle-api-openapi.yml
- filename: linkerd-metrics-api-openapi.yml
  format: yaml
  label: Linkerd Metrics API
  slug: linkerd-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-metrics-api-openapi.yml
- filename: linkerd-routes-api-openapi.yml
  format: yaml
  label: Linkerd Routes API
  slug: linkerd-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-routes-api-openapi.yml
- filename: linkerd-statistics-api-openapi.yml
  format: yaml
  label: Linkerd Statistics API
  slug: linkerd-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-statistics-api-openapi.yml
- filename: linkerd-tap-api-openapi.yml
  format: yaml
  label: Linkerd Tap API
  slug: linkerd-tap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-tap-api-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Linkerd Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shutdown
operation_count: 12
overview: 'Linkerd exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Linkerd
provider_slug: linkerd
slug: linkerd-agentic-access
source_filename: linkerd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/linkerd-proxy-admin-openapi.yml, openapi/linkerd-tap-openapi.yml, openapi/linkerd-viz-metrics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    safety-critical: 1\n    write: 6\n  human_in_the_loop_required: 1\noperations:\n- path: /metrics\n  method: get\n  operationId: getProxyMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ready\n  method: get\n  operationId: getProxyReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: getProxyLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shutdown\n  method: post\n  operationId: shutdownProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apis/tap.linkerd.io/v1alpha1\n  method: get\n  operationId: getTapApiResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watch/namespaces/{namespace}/tap\n  method: post\n  operationId: tapNamespace\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/namespaces/{namespace}/{resource_type}/{resource_name}/tap\n  method: post\n  operationId: tapResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stat\n  method: post\n  operationId: getStatSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/top-routes\n\
  \  method: post\n  operationId: getTopRoutes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/edges\n  method: post\n  operationId: getEdges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gateways\n  method: post\n  operationId: getGateways\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /ready\n  method: get\n  operationId: getMetricsApiReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/agentic-access/linkerd-agentic-access.yml
summary_line: 12 operations · 7 acting · 1 human-in-the-loop
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
---
