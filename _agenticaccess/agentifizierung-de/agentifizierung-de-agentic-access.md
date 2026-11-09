---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: agentifizierung-de-a2a-api-openapi.yml
  format: yaml
  label: Agentifizierung A2a API
  slug: agentifizierung-de-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentifizierung-de/openapi/agentifizierung-de-a2a-api-openapi.yml
- filename: agentifizierung-de-index-md-api-openapi.yml
  format: yaml
  label: Agentifizierung Index.md API
  slug: agentifizierung-de-index-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentifizierung-de/openapi/agentifizierung-de-index-md-api-openapi.yml
- filename: agentifizierung-de-llms-full-txt-api-openapi.yml
  format: yaml
  label: Agentifizierung Llms Full.txt API
  slug: agentifizierung-de-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentifizierung-de/openapi/agentifizierung-de-llms-full-txt-api-openapi.yml
- filename: agentifizierung-de-llms-txt-api-openapi.yml
  format: yaml
  label: Agentifizierung Llms.txt API
  slug: agentifizierung-de-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentifizierung-de/openapi/agentifizierung-de-llms-txt-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentifizierung De Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/v1/message:send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/v1/message:send
operation_count: 14
overview: 'Agentifizierung exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentifizierung
provider_slug: agentifizierung-de
slug: agentifizierung-de-agentic-access
source_filename: agentifizierung-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentifizierung-de-openapi.json, openapi/agentifizierung-de.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /a2a/v1\n  method: get\n  operationId: getA2AServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/v1\n  method: post\n  operationId: sendA2ARpcMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/v1/skills\n  method: get\n  operationId: getA2ASkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/v1/message:send\n  method: post\n  operationId: sendA2AMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{slug}/index.md\n  method: get\n  operationId: getPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/v1\n  method: get\n  operationId: getA2AServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/v1\n  method: post\n  operationId: sendA2ARpcMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/v1/skills\n  method: get\n  operationId: getA2ASkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/v1/message:send\n  method: post\n  operationId: sendA2AMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{slug}/index.md\n  method: get\n  operationId: getPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentifizierung-de/agentic-access/agentifizierung-de-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Artificial Intelligence
- Machine Learning
- Automation
- Digital Transformation
- Business
---
