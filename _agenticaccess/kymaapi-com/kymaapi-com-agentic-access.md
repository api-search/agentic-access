---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 24
api_specs:
- filename: kymaapi-com-audio-api-openapi.yml
  format: yaml
  label: kymaapi-com Audio API
  slug: kymaapi-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-audio-api-openapi.yml
- filename: kymaapi-com-auth-api-openapi.yml
  format: yaml
  label: kymaapi-com Auth API
  slug: kymaapi-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-auth-api-openapi.yml
- filename: kymaapi-com-chat-api-openapi.yml
  format: yaml
  label: kymaapi-com Chat API
  slug: kymaapi-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-chat-api-openapi.yml
- filename: kymaapi-com-completions-api-openapi.yml
  format: yaml
  label: kymaapi-com Completions API
  slug: kymaapi-com-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-completions-api-openapi.yml
- filename: kymaapi-com-credits-api-openapi.yml
  format: yaml
  label: kymaapi-com Credits API
  slug: kymaapi-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-credits-api-openapi.yml
- filename: kymaapi-com-decisions-api-openapi.yml
  format: yaml
  label: kymaapi-com Decisions API
  slug: kymaapi-com-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-decisions-api-openapi.yml
- filename: kymaapi-com-discovery-api-openapi.yml
  format: yaml
  label: kymaapi-com Discovery API
  slug: kymaapi-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-discovery-api-openapi.yml
- filename: kymaapi-com-embeddings-api-openapi.yml
  format: yaml
  label: kymaapi-com Embeddings API
  slug: kymaapi-com-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-embeddings-api-openapi.yml
- filename: kymaapi-com-images-api-openapi.yml
  format: yaml
  label: kymaapi-com Images API
  slug: kymaapi-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-images-api-openapi.yml
- filename: kymaapi-com-models-api-openapi.yml
  format: yaml
  label: kymaapi-com Models API
  slug: kymaapi-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-models-api-openapi.yml
- filename: kymaapi-com-video-api-openapi.yml
  format: yaml
  label: kymaapi-com Video API
  slug: kymaapi-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-video-api-openapi.yml
consequence_counts:
  read: 24
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kymaapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'kymaapi-com exposes 52 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 28 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kymaapi-com
provider_slug: kymaapi-com
slug: kymaapi-com-agentic-access
source_filename: kymaapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/kymaapi-com-openapi.json, openapi/kymaapi-com-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    acting: 28\n    connected: 24\n  by_consequence:\n    write: 28\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decisions\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n\
  \  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImageGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/generations\n  method: post\n  operationId: createVideoGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createAudioTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/understand\n  method: post\n  operationId: createAudioUnderstand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/music\n  method: post\n  operationId: createMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/sfx\n  method: post\n  operationId: createSoundEffect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n\
  \  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/recommend\n  method: get\n  operationId: recommendModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /credits/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/uptime\n  method: get\n  operationId: getUptime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/limits\n  method: get\n  operationId: getLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method:\
  \ post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decisions\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImageGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /videos/generations\n  method: post\n  operationId: createVideoGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createAudioTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/understand\n  method: post\n  operationId: createAudioUnderstand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/music\n  method: post\n  operationId: createMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/sfx\n  method: post\n  operationId: createSoundEffect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/recommend\n  method: get\n  operationId: recommendModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/uptime\n  method: get\n  operationId: getUptime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/limits\n  method: get\n  operationId: getLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/kymaapi-com/agentic-access/kymaapi-com-agentic-access.yml
summary_line: 52 operations · 28 acting
tags:
- LLM
- API Gateway
- Artificial Intelligence
- Machine Learning
- Developer Tools
---
