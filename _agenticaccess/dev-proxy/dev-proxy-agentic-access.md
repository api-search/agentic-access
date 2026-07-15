---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: dev-proxy-openapi.yml
  format: yaml
  label: Dev Proxy
  slug: dev-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-proxy/refs/heads/main/openapi/dev-proxy-openapi.yml
consequence_counts:
  read: 2
  safety-critical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Dev Proxy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /proxy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /proxy/stopproxy
operation_count: 6
overview: 'Dev Proxy exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dev Proxy
provider_slug: dev-proxy
slug: dev-proxy-agentic-access
source_filename: dev-proxy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dev-proxy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 2\n    acting: 4\n  by_consequence:\n    read: 2\n    safety-critical: 2\n    write: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /proxy\n  method: get\n  operationId: getProxyInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proxy\n  method: post\n  operationId: setProxyState\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n  \
  \    purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /proxy/jwtToken\n  method: post\n  operationId: generateJwt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /proxy/mockrequest\n  method: post\n  operationId: raiseMockRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /proxy/rootCertificate\n  method: get\n  operationId: getRootCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proxy/stopproxy\n  method: post\n  operationId: stopProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dev-proxy/refs/heads/main/agentic-access/dev-proxy-agentic-access.yml
summary_line: 6 operations · 4 acting · 2 human-in-the-loop
tags:
- Debugging Proxy
- Proxy
---
