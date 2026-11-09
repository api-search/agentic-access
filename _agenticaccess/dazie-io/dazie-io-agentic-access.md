---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: dazie-io-account-api-openapi.yml
  format: yaml
  label: dazie Account API
  slug: dazie-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-account-api-openapi.yml
- filename: dazie-io-calls-api-openapi.yml
  format: yaml
  label: dazie Calls API
  slug: dazie-io-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-calls-api-openapi.yml
- filename: dazie-io-journal-api-openapi.yml
  format: yaml
  label: dazie Journal API
  slug: dazie-io-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-journal-api-openapi.yml
- filename: dazie-io-memories-api-openapi.yml
  format: yaml
  label: dazie Memories API
  slug: dazie-io-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-memories-api-openapi.yml
- filename: dazie-io-to-dos-api-openapi.yml
  format: yaml
  label: dazie To Dos API
  slug: dazie-io-to-dos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-to-dos-api-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dazie Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'dazie exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dazie
provider_slug: dazie-io
slug: dazie-io-agentic-access
source_filename: dazie-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dazie-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journal-entries\n  method: get\n  operationId: listJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journal-entries\n  method: post\n  operationId:\
  \ createJournalEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journal-entries/{id}\n  method: get\n  operationId: getJournalEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /todos\n  method: get\n  operationId: listTodos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /todos\n  method: post\n  operationId: addTodo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /todos/{id}\n  method: patch\n  operationId: updateTodo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memories\n  method: get\n  operationId: listMemories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memories\n  method: post\n  operationId: addMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedules\n  method: get\n  operationId: getCallSchedule\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dazie-io/agentic-access/dazie-io-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Company
- Voice
- Journaling
- Artificial Intelligence
- Productivity
- Early-Access
---
