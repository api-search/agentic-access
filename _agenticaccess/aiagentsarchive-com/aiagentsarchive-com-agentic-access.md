---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 15
api_specs:
- filename: aiagentsarchive-com-agents-api-openapi.yml
  format: yaml
  label: AI Agents Archive Agents API
  slug: aiagentsarchive-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-agents-api-openapi.yml
- filename: aiagentsarchive-com-books-api-openapi.yml
  format: yaml
  label: AI Agents Archive Books API
  slug: aiagentsarchive-com-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-books-api-openapi.yml
- filename: aiagentsarchive-com-demand-api-openapi.yml
  format: yaml
  label: AI Agents Archive Demand API
  slug: aiagentsarchive-com-demand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-demand-api-openapi.yml
- filename: aiagentsarchive-com-discover-api-openapi.yml
  format: yaml
  label: AI Agents Archive Discover API
  slug: aiagentsarchive-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-discover-api-openapi.yml
- filename: aiagentsarchive-com-earnings-api-openapi.yml
  format: yaml
  label: AI Agents Archive Earnings API
  slug: aiagentsarchive-com-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-earnings-api-openapi.yml
- filename: aiagentsarchive-com-example-api-openapi.yml
  format: yaml
  label: AI Agents Archive Example API
  slug: aiagentsarchive-com-example-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-example-api-openapi.yml
- filename: aiagentsarchive-com-handoffs-api-openapi.yml
  format: yaml
  label: AI Agents Archive Handoffs API
  slug: aiagentsarchive-com-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-handoffs-api-openapi.yml
- filename: aiagentsarchive-com-health-api-openapi.yml
  format: yaml
  label: AI Agents Archive Health API
  slug: aiagentsarchive-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-health-api-openapi.yml
- filename: aiagentsarchive-com-receipts-api-openapi.yml
  format: yaml
  label: AI Agents Archive Receipts API
  slug: aiagentsarchive-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-receipts-api-openapi.yml
- filename: aiagentsarchive-com-stats-api-openapi.yml
  format: yaml
  label: AI Agents Archive Stats API
  slug: aiagentsarchive-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-stats-api-openapi.yml
- filename: aiagentsarchive-com-status-api-openapi.yml
  format: yaml
  label: AI Agents Archive Status API
  slug: aiagentsarchive-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-status-api-openapi.yml
- filename: aiagentsarchive-com-surface-api-openapi.yml
  format: yaml
  label: AI Agents Archive Surface API
  slug: aiagentsarchive-com-surface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-surface-api-openapi.yml
- filename: aiagentsarchive-com-template-api-openapi.yml
  format: yaml
  label: AI Agents Archive Template API
  slug: aiagentsarchive-com-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagentsarchive-com/openapi/aiagentsarchive-com-template-api-openapi.yml
consequence_counts:
  physical: 2
  read: 15
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aiagentsarchive Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/handoffs/{id}/unlock
operation_count: 19
overview: 'AI Agents Archive exposes 19 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI Agents Archive
provider_slug: aiagentsarchive-com
slug: aiagentsarchive-com-agentic-access
source_filename: aiagentsarchive-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiagentsarchive-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 15\n    acting: 4\n  by_consequence:\n    read: 15\n    physical: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/surface\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/example\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/books\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/discover\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/template\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/earnings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/demand\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}/body\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}/unlock\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/signal\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/receipts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aiagentsarchive-com/agentic-access/aiagentsarchive-com-agentic-access.yml
summary_line: 19 operations · 4 acting
tags:
- Artificial Intelligence
- Agents
- Archives
- TokenEconomics
- Marketplace
---
