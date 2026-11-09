---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 7
api_specs:
- filename: oruk-ai-affect-api-openapi.yml
  format: yaml
  label: oruk-ai Affect API
  slug: oruk-ai-affect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-affect-api-openapi.yml
- filename: oruk-ai-audio-api-openapi.yml
  format: yaml
  label: oruk-ai Audio API
  slug: oruk-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-audio-api-openapi.yml
- filename: oruk-ai-client-token-api-openapi.yml
  format: yaml
  label: oruk-ai Client Token API
  slug: oruk-ai-client-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-client-token-api-openapi.yml
- filename: oruk-ai-livez-api-openapi.yml
  format: yaml
  label: oruk-ai Livez API
  slug: oruk-ai-livez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-livez-api-openapi.yml
- filename: oruk-ai-models-api-openapi.yml
  format: yaml
  label: oruk-ai Models API
  slug: oruk-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-models-api-openapi.yml
- filename: oruk-ai-orukzero-api-openapi.yml
  format: yaml
  label: oruk-ai Oruk Zero API
  slug: oruk-ai-orukzero-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-orukzero-api-openapi.yml
- filename: oruk-ai-pricing-api-openapi.yml
  format: yaml
  label: oruk-ai Pricing API
  slug: oruk-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-pricing-api-openapi.yml
- filename: oruk-ai-readyz-api-openapi.yml
  format: yaml
  label: oruk-ai Readyz API
  slug: oruk-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-readyz-api-openapi.yml
consequence_counts:
  read: 7
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oruk Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'oruk-ai exposes 19 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: oruk-ai
provider_slug: oruk-ai
slug: oruk-ai-agentic-access
source_filename: oruk-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/oruk-ai.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 12\n    connected: 7\n  by_consequence:\n    write: 12\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/emotions\n  method: post\n  operationId: createEmotionAnalysis\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/styles\n  method: post\n  operationId: createStyleAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/affect\n  method: post\n  operationId: createAffectAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/analysis\n  method: post\n  operationId:\
  \ createSpeechAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/proficiency\n  method: post\n  operationId: createSpeechProficiency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livez\n  method: get\n  operationId: getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/client-token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/resonance-2/health\n  method: get\n  operationId: health_v1_audio_resonance_2_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/resonance-2\n  method: post\n  operationId: classify_v1_audio_resonance_2_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/oruk-resonance-2/access\n  method: get\n  operationId: getResonance2Access\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/oruk-resonance-2/access\n  method: post\n  operationId: requestResonance2Access\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/sessions\n  method: post\n  operationId: prepareSpectra2Session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/stream-sessions\n  method: post\n  operationId: prepareSpectra2DirectStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/synthetic-speech\n  method: post\n  operationId: detect_v1_audio_synthetic_speech_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/orukzero/access\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/oruk-ai/agentic-access/oruk-ai-agentic-access.yml
summary_line: 19 operations · 12 acting
tags:
- Company
- Speech
- Artificial Intelligence
- Transcription
- Voice
---
