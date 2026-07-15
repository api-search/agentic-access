---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Tables API
  slug: glide-apps-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Big Tables Rows API
  slug: glide-apps-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Stash & Bulk API
  slug: glide-apps-stash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Queries API
  slug: glide-apps-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Glide Apps Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Glide exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Glide
provider_slug: glide-apps
slug: glide-apps-agentic-access
source_filename: glide-apps-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/glide-apps-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 4\n    acting: 8\n  by_consequence:\n    read: 4\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /tables\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableID}\n  method: put\n  operationId: overwriteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableID}/rows\n  method: head\n  operationId: getRowsVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{tableID}/rows\n  method: get\n  operationId: getRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{tableID}/rows\n  method: post\n  operationId: addRows\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableID}/rows/{rowID}\n  method: get\n  operationId: getRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{tableID}/rows/{rowID}\n  method: patch\n  operationId: updateRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableID}/rows/{rowID}\n  method: delete\n  operationId: deleteRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableID}/queries\n  method: post\n  operationId: queryTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stashes/{stashID}/{serial}\n  method: put\n  operationId: setStashChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stashes/{stashID}\n  method: delete\n  operationId: deleteStash\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/agentic-access/glide-apps-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- No Code
- App Builder
- Tables
- Big Tables
- Data
- AI
---
