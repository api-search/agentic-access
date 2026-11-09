---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: cloudmcp-cloud-mcp-api-api-openapi.yml
  format: yaml
  label: Cloud MCP Cloud MCP API
  slug: cloudmcp-cloud-mcp-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-cloud-mcp-api-api-openapi.yml
- filename: cloudmcp-credit-api-openapi.yml
  format: yaml
  label: Cloud MCP Credit API
  slug: cloudmcp-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-credit-api-openapi.yml
- filename: cloudmcp-dashboard-api-openapi.yml
  format: yaml
  label: Cloud MCP Dashboard API
  slug: cloudmcp-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-dashboard-api-openapi.yml
- filename: cloudmcp-orders-api-openapi.yml
  format: yaml
  label: Cloud MCP Orders API
  slug: cloudmcp-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-orders-api-openapi.yml
- filename: cloudmcp-plants-api-openapi.yml
  format: yaml
  label: Cloud MCP Plants API
  slug: cloudmcp-plants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-plants-api-openapi.yml
- filename: cloudmcp-user-api-openapi.yml
  format: yaml
  label: Cloud MCP User API
  slug: cloudmcp-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-user-api-openapi.yml
- filename: cloudmcp-users-api-openapi.yml
  format: yaml
  label: Cloud MCP Users API
  slug: cloudmcp-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmcp/openapi/cloudmcp-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudmcp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 12
overview: 'Cloud MCP exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloud MCP
provider_slug: cloudmcp
slug: cloudmcp-agentic-access
source_filename: cloudmcp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cloudmcp-cloud-mcp-api-api-openapi.yml, openapi/cloudmcp-credit-api-openapi.yml,\n  openapi/cloudmcp-dashboard-api-openapi.yml, openapi/cloudmcp-orders-api-openapi.yml, openapi/cloudmcp-plants-api-openapi.yml,\n  openapi/cloudmcp-user-api-openapi.yml, openapi/cloudmcp-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 6\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/{v1id}\n  method: post\n  operationId: post_v1_v1id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit/accounts\n  method: post\n  operationId: post_credit_accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard\n  method: get\n  operationId: get_dashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: get_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: post_orders\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plants\n  method: get\n  operationId: get_plants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plants\n  method: post\n  operationId: post_plants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plants/{id}\n  method: delete\n  operationId: delete_plants_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plants/{id}\n  method: get\n  operationId: get_plants_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: post\n  operationId: post_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: get_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId:\
  \ post_users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cloudmcp/agentic-access/cloudmcp-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Company
- Artificial Intelligence
- Integration
- Tools
- Automation
---
