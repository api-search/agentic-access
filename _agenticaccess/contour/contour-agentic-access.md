---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: contour-httpproxy-openapi.yml
  format: yaml
  label: Contour HTTPProxy API
  slug: contour-httpproxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/openapi/contour-httpproxy-openapi.yml
- filename: contour-gateway-openapi.yml
  format: yaml
  label: Contour Gateway API
  slug: contour-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/openapi/contour-gateway-openapi.yml
consequence_counts:
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contour Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Contour exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Contour
provider_slug: contour
slug: contour-agentic-access
source_filename: contour-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/contour-gateway-openapi.yml, openapi/contour-httpproxy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/gateway.networking.k8s.io/v1/gatewayclasses\n  method: get\n  operationId: listGatewayClass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/gatewayclasses/{name}\n  method: get\n  operationId: readGatewayClass\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/gateways\n  method: get\n  operationId: listNamespacedGateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/gateways\n  method: post\n  operationId: createNamespacedGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/gateways/{name}\n  method: get\n  operationId: readNamespacedGateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/gateways/{name}\n  method: put\n  operationId: replaceNamespacedGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/gateways/{name}\n  method: delete\n  operationId: deleteNamespacedGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/httproutes\n  method: get\n  operationId: listNamespacedHTTPRoute\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/httproutes\n  method: post\n  operationId: createNamespacedHTTPRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/httproutes/{name}\n  method: get\n  operationId: readNamespacedHTTPRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/httproutes/{name}\n  method: put\n  operationId: replaceNamespacedHTTPRoute\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1/namespaces/{namespace}/httproutes/{name}\n  method: delete\n  operationId: deleteNamespacedHTTPRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/gateway.networking.k8s.io/v1alpha2/namespaces/{namespace}/tlsroutes\n  method: get\n  operationId: listNamespacedTLSRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/gateway.networking.k8s.io/v1alpha2/namespaces/{namespace}/tlsroutes\n\
  \  method: post\n  operationId: createNamespacedTLSRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies\n  method: get\n  operationId: listNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies\n  method: post\n  operationId: createNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies/{name}\n  method: get\n  operationId: readNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies/{name}\n  method: put\n  operationId: replaceNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies/{name}\n  method: patch\n  operationId: patchNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/httpproxies/{name}\n  method: delete\n  operationId: deleteNamespacedHTTPProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/projectcontour.io/v1/httpproxies\n  method: get\n  operationId: listHTTPProxyAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/tlscertificatedelegations\n  method: get\n  operationId: listNamespacedTLSCertificateDelegation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/projectcontour.io/v1/namespaces/{namespace}/tlscertificatedelegations\n  method: post\n  operationId: createNamespacedTLSCertificateDelegation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/agentic-access/contour-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Envoy
- Ingress Controller
- Kubernetes
- Networking
- Proxy
---
