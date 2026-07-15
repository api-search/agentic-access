---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: lunar-dev-gateway-admin-openapi.yml
  format: yaml
  label: Lunar.dev Gateway Admin API
  slug: gateway-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/openapi/lunar-dev-gateway-admin-openapi.yml
- filename: lunar-dev-gateway-proxy-openapi.yml
  format: yaml
  label: Lunar.dev Gateway Proxy API
  slug: gateway-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/openapi/lunar-dev-gateway-proxy-openapi.yml
consequence_counts:
  read: 3
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lunar Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Lunar.dev exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lunar.dev
provider_slug: lunar-dev
slug: lunar-dev-agentic-access
source_filename: lunar-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lunar-dev-gateway-admin-openapi.yml, openapi/lunar-dev-gateway-proxy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 3\n    acting: 8\n  by_consequence:\n    read: 3\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /healthcheck\n  method: get\n  operationId: getHealthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover\n  method: get\n  operationId: getDiscover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /apply_policies\n  method: post\n  operationId: applyPolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate_policies\n  method: post\n  operationId: validatePolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate_flows\n  method: post\n  operationId: validateFlows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /apply_flows\n  method: post\n  operationId: applyFlows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: get\n  operationId: proxyGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: proxyPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: proxyPut\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: proxyDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: patch\n  operationId: proxyPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/agentic-access/lunar-dev-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- AI Gateway
- Automation
- Consumption Gateway
- Control
- Deployment
- Integrations
- MCP Gateway
- Performance
- Platform
- Version Control
- Visibility
- Workflows
---
