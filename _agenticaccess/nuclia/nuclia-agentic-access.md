---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Knowledge Boxes API
  slug: knowledge-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Resources & Ingestion API
  slug: resources-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Search & Find API
  slug: search-find-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Ask & Chat (RAG) API
  slug: ask-chat-rag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Predict (NUA) API
  slug: predict-nua-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
consequence_counts:
  read: 9
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nuclia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Nuclia exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nuclia
provider_slug: nuclia
slug: nuclia-agentic-access
source_filename: nuclia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nuclia-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 9\n    acting: 14\n  by_consequence:\n    read: 9\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/kb/{kbid}\n  method: get\n  operationId: getKnowledgeBox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/counters\n  method: get\n  operationId: getKnowledgeBoxCounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/labelsets\n\
  \  method: get\n  operationId: getLabelSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/labelset/{labelset}\n  method: put\n  operationId: setLabelSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/resource\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/resources\n  method: get\n  operationId: listResources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/resource/{rid}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/resource/{rid}\n  method: patch\n  operationId: modifyResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/resource/{rid}\n  method: delete\n  operationId: deleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/resource/{rid}/file/{field}\n  method: put\n  operationId: uploadFileField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/upload\n  method: post\n  operationId: uploadToKnowledgeBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/find\n  method: post\n  operationId: find\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/suggest\n  method: get\n  operationId: suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kb/{kbid}/ask\n  method: post\n  operationId: ask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/kb/{kbid}/summarize\n  method: post\n  operationId: summarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/predict/chat\n  method: post\n  operationId: predictChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/predict/summarize\n  method: post\n  operationId: predictSummarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/predict/rephrase\n  method: post\n  operationId: predictRephrase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/predict/tokens\n  method: get\n  operationId: predictTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predict/sentence\n  method: get\n  operationId: predictSentence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predict/rerank\n  method: post\n  operationId: predictRerank\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/predict/models\n  method: get\n  operationId: listPredictModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/agentic-access/nuclia-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- AI
- RAG
- Search
- Knowledge Base
- Unstructured Data
---
