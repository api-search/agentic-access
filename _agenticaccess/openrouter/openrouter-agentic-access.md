---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: openrouter-chat-api-openapi.yml
  format: yaml
  label: OpenRouter Chat API
  slug: openrouter-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-chat-api-openapi.yml
- filename: openrouter-completions-api-openapi.yml
  format: yaml
  label: OpenRouter Completions API
  slug: openrouter-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-completions-api-openapi.yml
- filename: openrouter-credits-api-openapi.yml
  format: yaml
  label: OpenRouter Credits API
  slug: openrouter-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-credits-api-openapi.yml
- filename: openrouter-generation-api-openapi.yml
  format: yaml
  label: OpenRouter Generation API
  slug: openrouter-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-generation-api-openapi.yml
- filename: openrouter-keys-api-openapi.yml
  format: yaml
  label: OpenRouter Keys API
  slug: openrouter-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-keys-api-openapi.yml
- filename: openrouter-models-api-openapi.yml
  format: yaml
  label: OpenRouter Models API
  slug: openrouter-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-models-api-openapi.yml
- filename: openrouter-providers-api-openapi.yml
  format: yaml
  label: OpenRouter Providers API
  slug: openrouter-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/openapi/openrouter-providers-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openrouter Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'OpenRouter exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenRouter
provider_slug: openrouter
slug: openrouter-agentic-access
source_filename: openrouter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openrouter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 5\n    connected: 7\n  by_consequence:\n    write: 5\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{author}/{slug}/endpoints\n  method: get\n  operationId: listModelEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generation\n  method: get\n  operationId: getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{hash}\n  method: get\n  operationId: getKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /keys/{hash}\n  method: delete\n  operationId: deleteKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{hash}\n  method: patch\n  operationId: updateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/agentic-access/openrouter-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Artificial Intelligence
- Gateway
- Large Language Models
- Router
---
