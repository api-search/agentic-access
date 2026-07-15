---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Media Upload API
  slug: blotato-media-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Posts Publishing API
  slug: blotato-posts-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato AI Content API
  slug: blotato-ai-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Accounts API
  slug: blotato-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
consequence_counts:
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blotato Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Blotato exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blotato
provider_slug: blotato
slug: blotato-agentic-access
source_filename: blotato-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/blotato-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 3\n    connected: 7\n  by_consequence:\n    write: 3\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts\n  method: post\n  operationId: publishPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/{postSubmissionId}\n  method: get\n  operationId: getPostStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/accounts/{accountId}/subaccounts\n  method: get\n  operationId: listSubaccounts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/pinterest/boards\n  method: get\n  operationId: listPinterestBoards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/templates\n  method: get\n  operationId: listVisualTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/from-templates\n  method: post\n  operationId: createVisual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/creations/{id}\n  method: get\n  operationId: getVisualStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/agentic-access/blotato-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Social Media
- Publishing
- AI Content
- Automation
- Content Creation
---
