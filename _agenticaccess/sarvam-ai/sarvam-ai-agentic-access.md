---
acting_count: 7
action_class_counts:
  acting: 7
api_specs:
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Chat Completions (LLM) API
  slug: sarvam-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Speech-to-Text API
  slug: sarvam-ai-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Speech-to-Text Translate API
  slug: sarvam-ai-speech-to-text-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Text-to-Speech API
  slug: sarvam-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Translate API
  slug: sarvam-ai-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Transliterate API
  slug: sarvam-ai-transliterate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
- filename: sarvam-ai-openapi.yml
  format: yaml
  label: Sarvam AI Language Identification API
  slug: sarvam-ai-language-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-openapi.yml
consequence_counts:
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sarvam Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Sarvam AI exposes 7 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sarvam AI
provider_slug: sarvam-ai
slug: sarvam-ai-agentic-access
source_filename: sarvam-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sarvam-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 7\n  by_consequence:\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /speech-to-text\n  method: post\n  operationId: transcribeSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /speech-to-text-translate\n  method: post\n  operationId: translateSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text-to-speech\n  method: post\n  operationId: convertTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translate\n  method: post\n  operationId: translateText\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transliterate\n  method: post\n  operationId: transliterateText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text-lid\n  method: post\n  operationId: identifyLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/agentic-access/sarvam-ai-agentic-access.yml
summary_line: 7 operations · 7 acting
tags:
- AI
- LLM
- Speech to Text
- Text to Speech
- Translation
- Indian Languages
---
