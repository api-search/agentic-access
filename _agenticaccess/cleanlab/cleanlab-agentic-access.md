---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: cleanlab-openapi.yml
  format: yaml
  label: Trustworthy Language Model (TLM)
  slug: trustworthy-language-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
- filename: cleanlab-openapi.yml
  format: yaml
  label: Cleanlab Studio
  slug: cleanlab-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
- filename: cleanlab-openapi.yml
  format: yaml
  label: Codex
  slug: codex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
consequence_counts:
  physical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cleanlab Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/deployment/{model_id}/predict
operation_count: 3
overview: 'Cleanlab exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cleanlab
provider_slug: cleanlab
slug: cleanlab-agentic-access
source_filename: cleanlab-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cleanlab-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/openai_trustworthy_llm/v1/chat/completions\n  method: post\n  operationId: createTrustworthyChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/codex/projects/{project_id}/validate\n  method: post\n  operationId: validateResponse\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deployment/{model_id}/predict\n  method: post\n  operationId: predict\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/agentic-access/cleanlab-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- AI
- LLM
- Trustworthiness
- Data Quality
- Guardrails
---
