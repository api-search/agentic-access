---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: fabricatedemail-com-health-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Health API
  slug: fabricatedemail-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-health-api-openapi.yml
- filename: fabricatedemail-com-mcp-api-openapi.yml
  format: yaml
  label: fabricatedemail-com MCP API
  slug: fabricatedemail-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-mcp-api-openapi.yml
- filename: fabricatedemail-com-messages-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Messages API
  slug: fabricatedemail-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-messages-api-openapi.yml
- filename: fabricatedemail-com-subscriptions-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Subscriptions API
  slug: fabricatedemail-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-subscriptions-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fabricatedemail Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'fabricatedemail-com exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fabricatedemail-com
provider_slug: fabricatedemail-com
slug: fabricatedemail-com-agentic-access
source_filename: fabricatedemail-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/fabricatedemail-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{sid}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{sid}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{sid}/messages/{id}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{sid}/messages/{id}/extract\n  method: get\n  operationId: extractFromMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fabricatedemail-com/agentic-access/fabricatedemail-com-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Email
- Disposable
- Testing
- Automation
- Services
---
