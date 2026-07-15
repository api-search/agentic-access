---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: google-cloud-service-mesh-openapi.yml
  format: yaml
  label: Google Cloud Network Services API
  slug: network-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-openapi.yml
consequence_counts:
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Service Mesh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Google Cloud Service Mesh exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Service Mesh
provider_slug: google-cloud-service-mesh
slug: google-cloud-service-mesh-agentic-access
source_filename: google-cloud-service-mesh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-cloud-service-mesh-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 11\n    acting: 11\n  by_consequence:\n    read: 11\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/{name}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{name}\n  method: delete\n  operationId: deleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{name}\n  method: patch\n  operationId: updateResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/endpointPolicies\n  method: get\n  operationId:\
  \ listEndpointPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/endpointPolicies\n  method: post\n  operationId: createEndpointPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/gateways\n  method: get\n  operationId: listGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/gateways\n  method: post\n\
  \  operationId: createGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/meshes\n  method: get\n  operationId: listMeshes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/meshes\n  method: post\n  operationId: createMesh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/httpRoutes\n  method: get\n  operationId: listHttpRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/httpRoutes\n  method: post\n  operationId: createHttpRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/grpcRoutes\n  method: get\n  operationId: listGrpcRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/grpcRoutes\n  method: post\n  operationId: createGrpcRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/tcpRoutes\n  method: get\n  operationId: listTcpRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/tcpRoutes\n  method: post\n  operationId: createTcpRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/tlsRoutes\n  method: get\n  operationId: listTlsRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/tlsRoutes\n  method: post\n  operationId: createTlsRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/serviceLbPolicies\n  method: get\n  operationId: listServiceLbPolicies\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/serviceLbPolicies\n  method: post\n  operationId: createServiceLbPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{parent}/operations\n  method: get\n  operationId: listOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1/{name}:cancel\n  method: post\n  operationId: cancelOperation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/agentic-access/google-cloud-service-mesh-agentic-access.yml
summary_line: 22 operations · 11 acting
tags:
- Google Cloud
- Istio
- Kubernetes
- Microservices
- Service Mesh
---
