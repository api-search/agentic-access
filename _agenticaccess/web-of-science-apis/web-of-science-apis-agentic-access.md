---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: web-of-science-starter-openapi.yml
  format: yaml
  label: Web of Science Starter API
  slug: web-of-science-starter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-starter-openapi.yml
- filename: web-of-science-expanded-openapi.yml
  format: yaml
  label: Web of Science API Expanded
  slug: web-of-science-expanded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-expanded-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Web Of Science Apis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Web of Science APIs exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Web of Science APIs
provider_slug: web-of-science-apis
slug: web-of-science-apis-agentic-access
source_filename: web-of-science-apis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/web-of-science-expanded-openapi.yml, openapi/web-of-science-starter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: searchDocumentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: searchDocumentsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/{queryId}\n  method: get\n  operationId: getQueryResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordids/{queryId}\n  method: get\n  operationId: getRecordIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /id/{uniqueId}\n  method: get\n  operationId: getRecordById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /citing\n  method: get\n  operationId: getCitingArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /references\n  method: get\n  operationId: getReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related\n  method: get\n  operationId: getRelatedRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /citation-report/{queryId}\n  method: get\n  operationId: getCitationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /category-context/{uniqueId}\n  method: get\n  operationId: getCategoryContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: get\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{uid}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journals\n  method: get\n  operationId: getJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journals/{id}\n  method: get\n  operationId: getJournal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/agentic-access/web-of-science-apis-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Research
- Academic
- Bibliometrics
- Citations
- Science
- Scholarly
---
