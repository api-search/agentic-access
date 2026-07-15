---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: traefik-proxy-openapi.yml
  format: yaml
  label: Traefik Proxy
  slug: traefik-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/openapi/traefik-proxy-openapi.yml
- filename: traefik-proxy-openapi.yml
  format: yaml
  label: Traefik Proxy REST API
  slug: traefik-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/openapi/traefik-proxy-openapi.yml
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Traefik Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Traefik Labs exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Traefik Labs
provider_slug: traefik
slug: traefik-agentic-access
source_filename: traefik-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/traefik-proxy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /overview\n  method: get\n  operationId: getOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rawdata\n  method: get\n  operationId: getRawData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entrypoints\n  method: get\n  operationId: listEntryPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entrypoints/{name}\n  method: get\n  operationId: getEntryPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/routers\n  method: get\n  operationId: listHTTPRouters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/routers/{name}\n  method: get\n  operationId: getHTTPRouter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /http/services\n  method: get\n  operationId: listHTTPServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/services/{name}\n  method: get\n  operationId: getHTTPService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/middlewares\n  method: get\n  operationId: listHTTPMiddlewares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/middlewares/{name}\n  method: get\n  operationId: getHTTPMiddleware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/routers\n  method: get\n  operationId: listTCPRouters\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/routers/{name}\n  method: get\n  operationId: getTCPRouter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/services\n  method: get\n  operationId: listTCPServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/services/{name}\n  method: get\n  operationId: getTCPService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/middlewares\n  method: get\n  operationId: listTCPMiddlewares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcp/middlewares/{name}\n\
  \  method: get\n  operationId: getTCPMiddleware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /udp/routers\n  method: get\n  operationId: listUDPRouters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /udp/routers/{name}\n  method: get\n  operationId: getUDPRouter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /udp/services\n  method: get\n  operationId: listUDPServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /udp/services/{name}\n  method: get\n  operationId: getUDPService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /support-dump\n  method: get\n  operationId: getSupportDump\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/agentic-access/traefik-agentic-access.yml
summary_line: 23 operations
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- GitOps
- Kubernetes
- Load Balancer
- MCP Gateway
- Open Source
- Reverse Proxy
- WAF
---
