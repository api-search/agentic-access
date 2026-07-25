---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 12
api_specs:
- filename: slng-account-api-openapi.yml
  format: yaml
  label: SLNG Account API
  slug: slng-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-account-api-openapi.yml
- filename: slng-agents-api-openapi.yml
  format: yaml
  label: SLNG Agents API
  slug: slng-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-agents-api-openapi.yml
- filename: slng-calls-api-openapi.yml
  format: yaml
  label: SLNG Calls API
  slug: slng-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-calls-api-openapi.yml
- filename: slng-catalog-api-openapi.yml
  format: yaml
  label: SLNG Catalog API
  slug: slng-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-catalog-api-openapi.yml
- filename: slng-deepgram-aura-2-api-openapi.yml
  format: yaml
  label: SLNG Deepgram Aura 2 API
  slug: slng-deepgram-aura-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-deepgram-aura-2-api-openapi.yml
- filename: slng-deepgram-nova-3-api-openapi.yml
  format: yaml
  label: SLNG Deepgram Nova 3 API
  slug: slng-deepgram-nova-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-deepgram-nova-3-api-openapi.yml
- filename: slng-inworld-max-1-5-api-openapi.yml
  format: yaml
  label: SLNG Inworld Max 1.5 API
  slug: slng-inworld-max-1-5-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-inworld-max-1-5-api-openapi.yml
- filename: slng-orpheus-english-api-openapi.yml
  format: yaml
  label: SLNG Orpheus English API
  slug: slng-orpheus-english-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-orpheus-english-api-openapi.yml
- filename: slng-pronunciation-dictionaries-api-openapi.yml
  format: yaml
  label: SLNG Pronunciation dictionaries API
  slug: slng-pronunciation-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-pronunciation-dictionaries-api-openapi.yml
- filename: slng-rime-arcana-v2-api-openapi.yml
  format: yaml
  label: SLNG Rime Arcana v2 API
  slug: slng-rime-arcana-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-arcana-v2-api-openapi.yml
- filename: slng-rime-arcana-v3-api-openapi.yml
  format: yaml
  label: SLNG Rime Arcana v3 API
  slug: slng-rime-arcana-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-arcana-v3-api-openapi.yml
- filename: slng-rime-coda-api-openapi.yml
  format: yaml
  label: SLNG Rime Coda API
  slug: slng-rime-coda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-rime-coda-api-openapi.yml
- filename: slng-sessions-api-openapi.yml
  format: yaml
  label: SLNG Sessions API
  slug: slng-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-sessions-api-openapi.yml
- filename: slng-speechmatics-api-openapi.yml
  format: yaml
  label: SLNG Speechmatics API
  slug: slng-speechmatics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-speechmatics-api-openapi.yml
- filename: slng-whisper-large-v3-api-openapi.yml
  format: yaml
  label: SLNG Whisper Large v3 API
  slug: slng-whisper-large-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-whisper-large-v3-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Slng Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agents/{agent_id}/calls
operation_count: 43
overview: 'SLNG exposes 43 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 30 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SLNG
provider_slug: slng
slug: slng-agentic-access
source_filename: slng-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/slng-agents-openapi.yml, openapi/slng-batch-openapi.json, openapi/slng-management-slng-openapi.yml,\n  openapi/slng-me-openapi.json, openapi/slng-stt-slng-openapi.yml, openapi/slng-tts-pronunciation-dictionaries-openapi.yml,\n  openapi/slng-tts-slng-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 12\n    acting: 31\n  by_consequence:\n    read: 12\n    write: 30\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: put\n  operationId: replaceAgent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/duplicate\n  method: post\n  operationId: duplicateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/calls\n\
  \  method: post\n  operationId: dispatchCall\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agents/{agent_id}/calls\n  method: get\n  operationId: listAgentCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}/calls/{call_id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}/calls/{call_id}/tool-executions\n  method: post\n  operationId: submitCallToolExecution\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/web-sessions\n  method: post\n  operationId: createWebSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/jobs\n  method: post\n  operationId: batchJobsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/jobs\n  method: get\n  operationId: batchJobsList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/jobs/{jobId}\n  method: get\n  operationId: batchJobsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/jobs/{jobId}\n  method: delete\n  operationId: batchJobsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/jobs/{jobId}/files\n  method: get\n  operationId: batchJobsFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/models\n  method: get\n\
  \  operationId: catalog-models-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/models/{model_code}\n  method: get\n  operationId: catalog-models-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: meGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stt/slng/openai/whisper:large-v3\n  method: post\n  operationId: sttWhisperLargeV3Receive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/stt/slng/deepgram/nova:3-en\n  method: post\n  operationId: slng/deepgram/nova:3-en\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stt/slng/deepgram/nova:3-es\n  method: post\n  operationId: slng/deepgram/nova:3-es\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stt/slng/deepgram/nova:3-hi\n  method: post\n  operationId: slng/deepgram/nova:3-hi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stt/slng/deepgram/nova:3-multi\n  method: post\n  operationId: slng/deepgram/nova:3-multi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pronunciation/dictionaries\n  method: post\n  operationId: pronunciation-dictionaries-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pronunciation/dictionaries\n  method: get\n  operationId: pronunciation-dictionaries-list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pronunciation/dictionaries/{name}\n  method: get\n  operationId: pronunciation-dictionaries-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pronunciation/dictionaries/{name}\n  method: delete\n  operationId: pronunciation-dictionaries-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/canopylabs/orpheus:en\n  method: post\n  operationId: slng/canopylabs/orpheus:en\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:ar\n  method: post\n  operationId: rime/arcana:ar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:de\n  method: post\n  operationId: rime/arcana:de\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:en\n  method: post\n  operationId: rime/arcana:en\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:es\n  method: post\n  operationId: rime/arcana:es\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:fr\n  method: post\n  operationId: rime/arcana:fr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:3-en\n  method:\
  \ post\n  operationId: rime/arcana:3-en\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:3-es\n  method: post\n  operationId: rime/arcana:3-es\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:3-hi\n  method: post\n  operationId: rime/arcana:3-hi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/arcana:3-fr\n  method: post\n  operationId: rime/arcana:3-fr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/rime/coda:0-id\n  method: post\n  operationId: rime/coda:0-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/deepgram/aura:2-en\n  method: post\n  operationId: slng/deepgram/aura:2-en\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/deepgram/aura:2-es\n  method: post\n  operationId: slng/deepgram/aura:2-es\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tts/slng/inworld/max:1.5\n  method: post\n  operationId: slng/inworld/max:1.5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/agentic-access/slng-agentic-access.yml
summary_line: 43 operations · 31 acting · 1 human-in-the-loop
tags:
- Company
- Speech
- Voice
- Speech to Text
- Text to Speech
- Voice AI
- Voice Agents
- Transcription
- Speech Recognition
- Artificial Intelligence
- API Gateway
---
