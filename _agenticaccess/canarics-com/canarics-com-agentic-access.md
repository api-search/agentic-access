---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: canarics-com-agents-api-openapi.yml
  format: yaml
  label: canarics-com Agents API
  slug: canarics-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-agents-api-openapi.yml
- filename: canarics-com-callbacks-api-openapi.yml
  format: yaml
  label: canarics-com Callbacks API
  slug: canarics-com-callbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-callbacks-api-openapi.yml
- filename: canarics-com-calls-api-openapi.yml
  format: yaml
  label: canarics-com Calls API
  slug: canarics-com-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-calls-api-openapi.yml
- filename: canarics-com-campaigns-api-openapi.yml
  format: yaml
  label: canarics-com Campaigns API
  slug: canarics-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-campaigns-api-openapi.yml
- filename: canarics-com-canarics-api-for-ai-agents-api-openapi.yml
  format: yaml
  label: canarics-com Canarics API For AI Agents API
  slug: canarics-com-canarics-api-for-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-canarics-api-for-ai-agents-api-openapi.yml
- filename: canarics-com-contacts-api-openapi.yml
  format: yaml
  label: canarics-com Contacts API
  slug: canarics-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-contacts-api-openapi.yml
- filename: canarics-com-conversations-api-openapi.yml
  format: yaml
  label: canarics-com Conversations API
  slug: canarics-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-conversations-api-openapi.yml
- filename: canarics-com-demo-call-api-openapi.yml
  format: yaml
  label: canarics-com Demo Call API
  slug: canarics-com-demo-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-demo-call-api-openapi.yml
- filename: canarics-com-mcp-api-openapi.yml
  format: yaml
  label: canarics-com MCP API
  slug: canarics-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-mcp-api-openapi.yml
- filename: canarics-com-me-api-openapi.yml
  format: yaml
  label: canarics-com Me API
  slug: canarics-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-me-api-openapi.yml
- filename: canarics-com-signup-api-openapi.yml
  format: yaml
  label: canarics-com Signup API
  slug: canarics-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-signup-api-openapi.yml
- filename: canarics-com-tools-api-openapi.yml
  format: yaml
  label: canarics-com Tools API
  slug: canarics-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-tools-api-openapi.yml
- filename: canarics-com-upgrade-api-openapi.yml
  format: yaml
  label: canarics-com Upgrade API
  slug: canarics-com-upgrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-upgrade-api-openapi.yml
- filename: canarics-com-usage-api-openapi.yml
  format: yaml
  label: canarics-com Usage API
  slug: canarics-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canarics-com/openapi/canarics-com-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canarics Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/upgrade/checkout
operation_count: 21
overview: 'canarics-com exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: canarics-com
provider_slug: canarics-com
slug: canarics-com-agentic-access
source_filename: canarics-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/canarics-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 9\n    connected: 12\n  by_consequence:\n    write: 8\n    read: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/v1/signup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signup/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upgrade\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upgrade/checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/conversations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/contacts/{number}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/callbacks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calls/daily-stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/test\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/{name}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/demo-call\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/canarics-com/agentic-access/canarics-com-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Company
- Artificial Intelligence
- Voice
- Sales Intelligence
- Enterprise
---
