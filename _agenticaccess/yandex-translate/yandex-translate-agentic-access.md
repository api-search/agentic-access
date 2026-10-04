---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: yandex-translate-language-detection-api-openapi.yml
  format: yaml
  label: Yandex Translate API Language Detection API
  slug: yandex-translate-language-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/openapi/yandex-translate-language-detection-api-openapi.yml
- filename: yandex-translate-languages-api-openapi.yml
  format: yaml
  label: Yandex Translate API Languages API
  slug: yandex-translate-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/openapi/yandex-translate-languages-api-openapi.yml
- filename: yandex-translate-translation-api-openapi.yml
  format: yaml
  label: Yandex Translate API Translation API
  slug: yandex-translate-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/openapi/yandex-translate-translation-api-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yandex Translate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Yandex Translate API exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yandex Translate API
provider_slug: yandex-translate
slug: yandex-translate-agentic-access
source_filename: yandex-translate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/yandex-translate-language-detection-api-openapi.yml, openapi/yandex-translate-languages-api-openapi.yml,\n  openapi/yandex-translate-translation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /translate/v2/detect\n  method: post\n  operationId: detectLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /translate/v2/languages\n  method: post\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translate/v2/translate\n  method: post\n  operationId: translate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/agentic-access/yandex-translate-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Machine Translation
- Natural Language Processing
- Language Detection
- Translation Dictionary
- Multilingual
- Yandex Cloud
- Localization
- Internationalization
---
