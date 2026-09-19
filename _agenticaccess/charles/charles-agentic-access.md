---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 18
api_specs:
- filename: charles-languages-api-openapi.yml
  format: yaml
  label: LINDAT Translation Languages API
  slug: charles-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-languages-api-openapi.yml
- filename: charles-models-api-openapi.yml
  format: yaml
  label: LINDAT Translation Models API
  slug: charles-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-models-api-openapi.yml
- filename: charles-root-api-openapi.yml
  format: yaml
  label: LINDAT Translation Root API
  slug: charles-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-root-api-openapi.yml
- filename: charles-udpipe-api-openapi.yml
  format: yaml
  label: LINDAT UDPipe API
  slug: lindat-udpipe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-udpipe-api-openapi.yml
- filename: charles-nametag-api-openapi.yml
  format: yaml
  label: LINDAT NameTag API
  slug: lindat-nametag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-nametag-api-openapi.yml
- filename: charles-morphodita-api-openapi.yml
  format: yaml
  label: LINDAT MorphoDiTa API
  slug: lindat-morphodita
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-morphodita-api-openapi.yml
- filename: charles-korektor-api-openapi.yml
  format: yaml
  label: LINDAT Korektor API
  slug: lindat-korektor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-korektor-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Charles Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /models/{model}
operation_count: 23
overview: 'Charles University exposes 23 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Charles University
provider_slug: charles
slug: charles-agentic-access
source_filename: charles-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/charles-korektor-api-openapi.yml, openapi/charles-languages-api-openapi.yml,\n  openapi/charles-models-api-openapi.yml, openapi/charles-morphodita-api-openapi.yml, openapi/charles-nametag-api-openapi.yml,\n  openapi/charles-root-api-openapi.yml, openapi/charles-udpipe-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 18\n    acting: 5\n  by_consequence:\n    read: 18\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /models\n  method: get\n  operationId: listKorektorModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /correct\n  method: get\n  operationId: correctText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggestions\n  method: get\n  operationId: suggestCorrections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages/\n  method: get\n  operationId: get_language_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages/\n  method: post\n  operationId: post_language_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /languages/{language}\n  method: get\n  operationId: get_language_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/\n  method: get\n  operationId: get_model_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: get\n  operationId: get_model_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: post\n  operationId: post_model_item\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listMorphoDiTaModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tag\n  method: get\n  operationId: tagText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze\n  method: get\n  operationId: analyzeText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate\n  method: get\n  operationId: generateForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenize\n  method: get\n  operationId: tokenizeTextMorphoDiTa\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listNameTagModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recognize\n  method: get\n  operationId: recognizeEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recognize\n  method: post\n  operationId: recognizeEntitiesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenize\n  method: get\n  operationId: tokenizeText\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenize\n  method: post\n  operationId: tokenizeTextPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: get_root_resource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listUDPipeModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process\n  method: get\n  operationId: processText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process\n  method: post\n  operationId: processTextPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/agentic-access/charles-agentic-access.yml
summary_line: 23 operations · 5 acting
tags:
- University
- Higher Education
- Education
- Research
- Czechia
- Europe
- Language Technology
- Natural Language Processing
- Machine Translation
- Research Repository
- Identity Federation
- OAI-PMH
- CLARIN
---
