---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: chroniclingamerica-openapi.yml
  format: yaml
  label: Chronicling America Search API
  slug: chronicling-america-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-openapi.yml
- filename: chroniclingamerica-openapi.yml
  format: yaml
  label: Chronicling America Titles API
  slug: chronicling-america-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-openapi.yml
- filename: chroniclingamerica-openapi.yml
  format: yaml
  label: Chronicling America Pages API
  slug: chronicling-america-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chroniclingamerica Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Chronicling America exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chronicling America
provider_slug: chroniclingamerica
slug: chroniclingamerica-agentic-access
source_filename: chroniclingamerica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chroniclingamerica-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /search/pages/results/\n  method: get\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/titles/results/\n  method: get\n  operationId: searchTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles.json\n  method: get\n  operationId:\
  \ listTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{lccn}.json\n  method: get\n  operationId: getTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{lccn}/issues.json\n  method: get\n  operationId: listIssuesByTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{lccn}/issues/{date}/ed-{edition}.json\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{lccn}/issues/{date}/ed-{edition}/seq-{sequence}.json\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{lccn}/issues/{date}/ed-{edition}/seq-{sequence}/ocr.txt\n  method: get\n  operationId: getPageOcrText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches.json\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches/{batch_name}.json\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newspapers.json\n  method: get\n  operationId: listNewspapers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/agentic-access/chroniclingamerica-agentic-access.yml
summary_line: 11 operations
tags:
- Newspapers
- Historical
- Archives
- Library of Congress
- Government
- Digitized
- OCR
- Search
- Cultural Heritage
---
