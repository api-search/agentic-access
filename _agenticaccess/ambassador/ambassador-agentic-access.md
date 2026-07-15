---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 13
api_specs:
- filename: ambassador-openapi.yml
  format: yaml
  label: Ambassador
  slug: ambassador
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-openapi.yml
- filename: ambassador-openapi.yml
  format: yaml
  label: Ambassador Edge Stack API Gateway
  slug: edge-stack-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-openapi.yml
consequence_counts:
  read: 13
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ambassador Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Ambassador exposes 26 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ambassador
provider_slug: ambassador
slug: ambassador-agentic-access
source_filename: ambassador-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ambassador-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 13\n    acting: 13\n  by_consequence:\n    read: 13\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /ambassador/v0/diag\n  method: get\n  operationId: getDiagnostics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambassador/v0/check_ready\n  method: get\n  operationId: checkReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambassador/v0/check_alive\n\
  \  method: get\n  operationId: checkAlive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings\n  method: get\n  operationId: listMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings\n  method: post\n  operationId: createMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: get\n  operationId: getMapping\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: put\n  operationId: updateMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/mappings/{name}\n  method: delete\n  operationId: deleteMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts\n  method: get\n\
  \  operationId: listHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts\n  method: post\n  operationId: createHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: get\n  operationId: getHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: put\n  operationId: updateHost\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/hosts/{name}\n  method: delete\n  operationId: deleteHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts\n  method: get\n  operationId: listTLSContexts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts\n  method: post\n  operationId: createTLSContext\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts/{name}\n  method: get\n  operationId: getTLSContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts/{name}\n  method: put\n  operationId: updateTLSContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/tlscontexts/{name}\n\
  \  method: delete\n  operationId: deleteTLSContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimits\n  method: get\n  operationId: listRateLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimits\n  method: post\n  operationId: createRateLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimits/{name}\n  method: get\n  operationId: getRateLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimits/{name}\n  method: put\n  operationId: updateRateLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/ratelimits/{name}\n  method: delete\n  operationId: deleteRateLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/modules\n  method: get\n  operationId: listModules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/modules/{name}\n  method: get\n  operationId: getModule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/getambassador.io/v3alpha1/namespaces/{namespace}/modules/{name}\n  method: put\n  operationId: updateModule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/agentic-access/ambassador-agentic-access.yml
summary_line: 26 operations · 13 acting
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
---
