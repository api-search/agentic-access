---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Apps API
  slug: aci-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Functions API
  slug: aci-dev-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev App Configurations API
  slug: aci-dev-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Linked Accounts API
  slug: aci-dev-linked-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aci Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'ACI.dev exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ACI.dev
provider_slug: aci-dev
slug: aci-dev-agentic-access
source_filename: aci-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aci-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/apps/search\n  method: get\n  operationId: apps-search_apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_name}\n  method: get\n  operationId: apps-get_app_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/functions/search\n\
  \  method: get\n  operationId: functions-search_functions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/functions/{function_name}/definition\n  method: get\n  operationId: functions-get_function_definition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/functions/{function_name}/execute\n  method: post\n  operationId: functions-execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app-configurations\n  method: post\n  operationId: app-configurations-create_app_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app-configurations\n  method: get\n  operationId: app-configurations-list_app_configurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app-configurations/{app_name}\n  method: get\n  operationId: app-configurations-get_app_configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app-configurations/{app_name}\n  method: delete\n  operationId: app-configurations-delete_app_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app-configurations/{app_name}\n  method: patch\n  operationId: app-configurations-update_app_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/linked-accounts/oauth2\n  method: get\n  operationId: linked-accounts-link_oauth2_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linked-accounts/oauth2/callback\n  method: get\n  operationId: linked-accounts-linked_accounts_oauth2_callback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/linked-accounts\n  method: get\n  operationId: linked-accounts-list_linked_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linked-accounts/{linked_account_id}\n  method: get\n  operationId: linked-accounts-get_linked_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linked-accounts/{linked_account_id}\n  method: delete\n  operationId: linked-accounts-delete_linked_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/agentic-access/aci-dev-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Agent Infrastructure
- Agents
- AI
- Artificial Intelligence
- Function Calling
- MCP
- Model Context Protocol
- OAuth
- Open Source
- Tool Calling
- VibeOps
---
