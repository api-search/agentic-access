---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 17
api_specs:
- filename: linkace-bulk-api-openapi.yml
  format: yaml
  label: LinkAce Bulk API
  slug: linkace-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-bulk-api-openapi.yml
- filename: linkace-general-api-openapi.yml
  format: yaml
  label: LinkAce General API
  slug: linkace-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-general-api-openapi.yml
- filename: linkace-links-api-openapi.yml
  format: yaml
  label: LinkAce Links API
  slug: linkace-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-links-api-openapi.yml
- filename: linkace-lists-api-openapi.yml
  format: yaml
  label: LinkAce Lists API
  slug: linkace-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-lists-api-openapi.yml
- filename: linkace-notes-api-openapi.yml
  format: yaml
  label: LinkAce Notes API
  slug: linkace-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-notes-api-openapi.yml
- filename: linkace-search-api-openapi.yml
  format: yaml
  label: LinkAce Search API
  slug: linkace-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-search-api-openapi.yml
- filename: linkace-tags-api-openapi.yml
  format: yaml
  label: LinkAce Tags API
  slug: linkace-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-tags-api-openapi.yml
- filename: linkace-trash-api-openapi.yml
  format: yaml
  label: LinkAce Trash API
  slug: linkace-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-trash-api-openapi.yml
consequence_counts:
  read: 17
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Linkace Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 38
overview: 'LinkAce exposes 38 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LinkAce
provider_slug: linkace
slug: linkace-agentic-access
source_filename: linkace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/LinkAce-API.v2.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 17\n    acting: 21\n  by_consequence:\n    read: 17\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /api/version\n  method: get\n  operationId: get-api-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/links\n  method: get\n  operationId: get-api-v2-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/links\n  method: post\n\
  \  operationId: post-api-v2-links\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/links/{link_id}\n  method: get\n  operationId: get-api-v2-links-link_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/links/{link_id}\n  method: patch\n  operationId: patch-api-v2-links-link_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/links/{link_id}\n  method: delete\n  operationId: delete-api-v2-links-link_id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/search/links\n  method: get\n  operationId: get-api-v2-search-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/links/{link_id}/notes\n  method: get\n  operationId: get-api-v2-links-link_id-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/lists\n  method: get\n  operationId: get-api-v2-lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/lists\n  method:\
  \ post\n  operationId: post-api-v2-lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/lists/{list_id}\n  method: get\n  operationId: get-api-v2-lists-list_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/lists/{list_id}\n  method: patch\n  operationId: patch-api-v2-lists-list_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/lists/{list_id}\n  method: delete\n  operationId: delete-api-v2-lists-list_id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/lists/{list_id}/links\n  method: get\n  operationId: get-api-v2-lists-list_id-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/lists\n  method: get\n  operationId: get-api-v2-search-lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tags\n  method: get\n  operationId: get-api-v2-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tags\n  method:\
  \ post\n  operationId: post-api-v2-tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tags/{tag_id}\n  method: get\n  operationId: get-api-v2-tags-tag_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tags/{tag_id}\n  method: patch\n  operationId: patch-api-v2-tags-tag_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tags/{tag_id}\n  method: delete\n  operationId: delete-api-v2-tags-tag_id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tags/{tag_id}/links\n  method: get\n  operationId: get-api-v2-tags-tag_id-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bulk/links\n  method: post\n  operationId: post-api-v2-bulk-links\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/links\n  method: patch\n  operationId: patch-api-v2-bulk-links\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/lists\n  method: post\n  operationId: post-api-v2-bulk-lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/lists\n  method: patch\n  operationId: patch-api-v2-bulk-lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/tags\n  method: post\n\
  \  operationId: post-api-v2-bulk-tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/tags\n  method: patch\n  operationId: post-api-v2-bulk-tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bulk/delete\n  method: delete\n  operationId: post-api-v2-bulk-deletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v2/search/tags\n  method: get\n  operationId: get-api-v2-search-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/notes\n  method: post\n  operationId: post-api-v2-notes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/notes/{note_id}\n  method: patch\n  operationId: patch-api-v2-notes-note_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/notes/{note_id}\n\
  \  method: delete\n  operationId: delete-api-v2-notes-note_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/trash/links\n  method: get\n  operationId: get-api-v2-trash-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/trash/lists\n  method: get\n  operationId: get-api-v2-trash-lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/trash/tags\n  method: get\n  operationId: get-api-v2-trash-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v2/trash/notes\n  method: get\n  operationId: get-api-v2-trash-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/trash/clear\n  method: delete\n  operationId: delete-api-v2-trash-clear\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/trash/restore\n  method: patch\n  operationId: patch-api-v2-trash-restore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/linkace/agentic-access/linkace-agentic-access.yml
summary_line: 38 operations · 21 acting
tags:
- Company
- Open Source
- Bookmarking
- Self-Hosted
---
