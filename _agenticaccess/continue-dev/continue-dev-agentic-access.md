---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: continue-dev-hub-ide-api-openapi.yml
  format: yaml
  label: Continue Hub IDE API
  slug: continue-hub-ide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/openapi/continue-dev-hub-ide-api-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Continue Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Continue exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Continue
provider_slug: continue-dev
slug: continue-dev-agentic-access
source_filename: continue-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/continue-dev-hub-ide-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ide/list-assistants\n  method: get\n  operationId: listAssistants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ide/get-assistant/{ownerSlug}/{packageSlug}\n  method: get\n  operationId: getAssistant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /ide/free-trial-status\n  method: get\n  operationId: getFreeTrialStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ide/get-models-add-on-checkout-url\n  method: get\n  operationId: getModelsAddOnCheckoutUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ide/policy\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ide/sync-secrets\n  method: post\n  operationId: syncSecrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ide/list-assistant-full-slugs\n  method: get\n  operationId: listAssistantFullSlugs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ide/list-organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/agentic-access/continue-dev-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- AI
- Artificial Intelligence
- Developer Tools
- Code Assistant
- Open Source
- VS Code
- JetBrains
- CLI
- MCP
- Apache 2.0
---
