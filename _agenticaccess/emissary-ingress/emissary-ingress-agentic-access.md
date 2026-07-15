---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 9
api_specs:
- filename: emissary-ingress-openapi.yml
  format: yaml
  label: Emissary-Ingress Configuration API
  slug: emissary-ingress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emissary-ingress/refs/heads/main/openapi/emissary-ingress-openapi.yml
consequence_counts:
  read: 9
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Emissary Ingress Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Emissary-Ingress exposes 20 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Emissary-Ingress
provider_slug: emissary-ingress
slug: emissary-ingress-agentic-access
source_filename: emissary-ingress-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/emissary-ingress-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 9\n    acting: 11\n  by_consequence:\n    read: 9\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings\n  method: get\n  operationId: listNamespacedMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings\n  method: post\n  operationId: createNamespacedMapping\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: get\n  operationId: readNamespacedMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: put\n  operationId: replaceNamespacedMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: patch\n\
  \  operationId: patchNamespacedMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: delete\n  operationId: deleteNamespacedMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/mappings\n  method: get\n  operationId: listMappingAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts\n\
  \  method: get\n  operationId: listNamespacedHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts\n  method: post\n  operationId: createNamespacedHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: get\n  operationId: readNamespacedHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: put\n  operationId: replaceNamespacedHost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: delete\n  operationId: deleteNamespacedHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts\n  method: get\n  operationId: listNamespacedTLSContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts\n\
  \  method: post\n  operationId: createNamespacedTLSContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts/{name}\n  method: get\n  operationId: readNamespacedTLSContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts/{name}\n  method: delete\n  operationId: deleteNamespacedTLSContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimitservices\n  method: get\n  operationId: listNamespacedRateLimitService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimitservices\n  method: post\n  operationId: createNamespacedRateLimitService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/authservices\n  method: get\n  operationId: listNamespacedAuthService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/authservices\n  method: post\n  operationId: createNamespacedAuthService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emissary-ingress/refs/heads/main/agentic-access/emissary-ingress-agentic-access.yml
summary_line: 20 operations · 11 acting
tags:
- API Gateway
- Cloud Native
- Envoy
- Incubating
- Ingress
- Kubernetes
---
