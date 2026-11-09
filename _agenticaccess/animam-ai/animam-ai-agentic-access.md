---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 8
api_specs:
- filename: animam-ai-corpus-api-openapi.yml
  format: yaml
  label: Animam.ai Corpus API
  slug: animam-ai-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-corpus-api-openapi.yml
- filename: animam-ai-segments-api-openapi.yml
  format: yaml
  label: Animam.ai Segments API
  slug: animam-ai-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-segments-api-openapi.yml
- filename: animam-ai-tenants-api-openapi.yml
  format: yaml
  label: Animam.ai Tenants API
  slug: animam-ai-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-tenants-api-openapi.yml
consequence_counts:
  read: 8
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Animam Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Animam.ai exposes 26 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Animam.ai
provider_slug: animam-ai
slug: animam-ai-agentic-access
source_filename: animam-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/animam-ai-openapi.json, openapi/animam-ai-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 8\n    acting: 18\n  by_consequence:\n    read: 8\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /tenants/{slug}/corpus\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - corpus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/corpus\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/bulk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/sync\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - corpus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/corpus/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:read\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/mcp-tools\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/segments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - segments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/segments\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/segments/{slugOrId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - corpus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/corpus\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/bulk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/sync\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /tenants/{slug}/corpus/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - corpus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/corpus/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/corpus/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - corpus:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/mcp-tools\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/segments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - segments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{slug}/segments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{slug}/segments/{slugOrId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/animam-ai/agentic-access/animam-ai-agentic-access.yml
summary_line: 26 operations · 18 acting
tags:
- Artificial Intelligence
- Automation
- Lead Generation
- Chatbots
- Software-as-a-Service
---
