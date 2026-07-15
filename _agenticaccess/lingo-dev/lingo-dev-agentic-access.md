---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev Engine API (Localize)
  slug: engine-api-localize
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev SDK
  slug: sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lingo Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Lingo.dev exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lingo.dev
provider_slug: lingo-dev
slug: lingo-dev-agentic-access
source_filename: lingo-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lingo-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 4\n    connected: 3\n  by_consequence:\n    write: 4\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /process/localize\n  method: post\n  operationId: localize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process/recognize\n  method: post\n  operationId: recognize\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process/estimate\n  method: post\n  operationId: estimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/localization\n  method: post\n  operationId: createLocalizationJobGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/localization\n  method: get\n  operationId: listLocalizationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/localization/{groupId}\n  method: get\n  operationId: getLocalizationJobGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/agentic-access/lingo-dev-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- AI
- Localization
- Translation
- i18n
- Developer Tools
---
