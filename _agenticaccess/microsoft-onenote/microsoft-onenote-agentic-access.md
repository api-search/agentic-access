---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: microsoft-onenote-openapi.yml
  format: yaml
  label: Microsoft Graph OneNote API
  slug: graph-onenote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-openapi.yml
consequence_counts:
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Onenote Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Microsoft OneNote exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft OneNote
provider_slug: microsoft-onenote
slug: microsoft-onenote-agentic-access
source_filename: microsoft-onenote-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-onenote-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /me/onenote/notebooks\n  method: get\n  operationId: listNotebooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/notebooks\n  method: post\n  operationId: createNotebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/notebooks/{notebookId}\n  method: get\n  operationId: getNotebook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/notebooks/{notebookId}/sections\n  method: get\n  operationId: listNotebookSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/notebooks/{notebookId}/sections\n  method: post\n  operationId: createNotebookSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/notebooks/{notebookId}/sectionGroups\n\
  \  method: get\n  operationId: listNotebookSectionGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/notebooks/{notebookId}/sectionGroups\n  method: post\n  operationId: createNotebookSectionGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/sections/{sectionId}\n  method: get\n  operationId: getSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/sections/{sectionId}/pages\n  method: get\n  operationId: listSectionPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/sections/{sectionId}/pages\n  method: post\n  operationId: createSectionPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/pages/{pageId}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/pages/{pageId}\n  method: delete\n  operationId: deletePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/pages/{pageId}/content\n  method: get\n  operationId: getPageContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/onenote/pages/{pageId}/content\n  method: patch\n  operationId: updatePageContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /me/onenote/sectionGroups\n  method: get\n  operationId: listSectionGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/agentic-access/microsoft-onenote-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- Microsoft
- Microsoft 365
- Notebooks
- Notes
- Productivity
---
