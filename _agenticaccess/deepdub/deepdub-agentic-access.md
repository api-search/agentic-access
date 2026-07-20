---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 9
api_specs:
- filename: deepdub-api-openapi-original.json
  format: json
  label: Deepdub Text-to-Speech API
  slug: deepdub-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-api-openapi-original.json
- filename: deepdub-managed-dub-openapi-original.json
  format: json
  label: Deepdub Managed Dubbing API
  slug: deepdub-managed-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-managed-dub-openapi-original.json
consequence_counts:
  read: 9
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deepdub Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Deepdub exposes 24 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deepdub
provider_slug: deepdub
slug: deepdub-agentic-access
source_filename: deepdub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/deepdub-api-openapi-original.json, openapi/deepdub-managed-dub-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 15\n    connected: 9\n  by_consequence:\n    write: 15\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /tts\n  method: post\n  operationId: generateTTS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gender-detection/classify\n  method: post\n  operationId: classifyGender\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gender-detection/classify/upload\n  method: post\n  operationId: classifyGenderUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice\n  method: get\n  operationId: getVoicePrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voice\n  method: post\n  operationId: createVoicePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice\n  method: put\n  operationId: updateVoicePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice/{prompt_id}\n  method: get\n  operationId: getVoicePromptById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voice/{prompt_id}\n  method: delete\n  operationId: deleteVoicePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage/concurrent\n  method: get\n  operationId: getUsageConcurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/concurrent/by-model\n  method: get\n  operationId: getUsageConcurrentByModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/{id}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/{id}\n  method: put\n  operationId: updateIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/{id}\n  method: delete\n  operationId: deleteIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /concurrent_connections/batch\n  method: get\n  operationId: getConcurrentConnectionsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /concurrent_connections/{model_id}\n  method: get\n  operationId: getConcurrentConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concurrent_connections/{model_id}\n  method: put\n  operationId: updateConcurrentConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dubbing/job\n  method: post\n  operationId: create_dubbing_job_dubbing_job_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /dubbing/job/{request_id}\n  method: get\n  operationId: get_dubbing_job_dubbing_job__request_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dubbing/job/{request_id}\n  method: put\n  operationId: update_request_handler_dubbing_job__request_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dubbing/job/{request_id}\n  method: delete\n  operationId: cancel_request_handler_dubbing_job__request_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dubbing/job/{request_id}\n  method: patch\n  operationId: create_redubbing_job_handler_dubbing_job__request_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dubbing/jobs\n  method: get\n  operationId: list_dubbing_jobs_dubbing_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dubbing/job/{request_id}/sources\n  method: post\n  operationId: add_source_handler_dubbing_job__request_id__sources_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/agentic-access/deepdub-agentic-access.yml
summary_line: 24 operations · 15 acting
tags:
- Company
- Voice
- Text to Speech
- Dubbing
- Localization
- Speech Synthesis
- Voice Cloning
- Media
- Artificial Intelligence
- Audio
---
