---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Translation API
  slug: unbabel-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Machine Translation API
  slug: unbabel-machine-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Language Pairs API
  slug: unbabel-language-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Tone and Topic API
  slug: unbabel-tone-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Word Count API
  slug: unbabel-word-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Account API
  slug: unbabel-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Notifications API
  slug: unbabel-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unbabel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Unbabel exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unbabel
provider_slug: unbabel
slug: unbabel-agentic-access
source_filename: unbabel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unbabel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /translation/\n  method: get\n  operationId: listTranslations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/\n  method: patch\n  operationId: bulkUpdateTranslations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/{uid}/\n  method: get\n  operationId: getTranslation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mt_translation/\n  method: get\n  operationId: listMachineTranslations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mt_translation/\n  method: post\n  operationId: createMachineTranslation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mt_translation/{uid}/\n  method: get\n  operationId: getMachineTranslation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mt_translation/{uid}/\n  method: patch\n  operationId: upgradeMachineTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /language_pair/\n  method: get\n  operationId: listLanguagePairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tone/\n  method: get\n  operationId: listTones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wordcount/\n  method: post\n  operationId: calculateWordCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/agentic-access/unbabel-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Translation
- Localization
- Language Operations
- LangOps
- Machine Translation
- Human in the Loop
- AI
---
