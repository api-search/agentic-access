---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 3
api_specs:
- filename: convai-character-api-openapi.yml
  format: yaml
  label: Convai Character API
  slug: convai-character-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-character-api-openapi.yml
- filename: convai-interaction-api-openapi.yml
  format: yaml
  label: Convai Interaction API
  slug: convai-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-interaction-api-openapi.yml
- filename: convai-knowledge-bank-api-openapi.yml
  format: yaml
  label: Convai Knowledge Bank API
  slug: convai-knowledge-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-knowledge-bank-api-openapi.yml
- filename: convai-tts-api-openapi.yml
  format: yaml
  label: Convai Text-to-Speech API
  slug: convai-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-tts-api-openapi.yml
- filename: convai-narrative-design-api-openapi.yml
  format: yaml
  label: Convai Narrative Design API
  slug: convai-narrative-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-narrative-design-api-openapi.yml
- filename: convai-chat-history-api-openapi.yml
  format: yaml
  label: Convai Chat History API
  slug: convai-chat-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-chat-history-api-openapi.yml
- filename: convai-custom-llm-api-openapi.yml
  format: yaml
  label: Convai Custom LLM API
  slug: convai-custom-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-custom-llm-api-openapi.yml
- filename: convai-evaluation-api-openapi.yml
  format: yaml
  label: Convai Evaluation API
  slug: convai-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-evaluation-api-openapi.yml
- filename: convai-streaming-transcription-api-openapi.yml
  format: yaml
  label: Convai Streaming Transcription API
  slug: convai-streaming-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-streaming-transcription-api-openapi.yml
- filename: convai-live-api-openapi.yml
  format: yaml
  label: Convai Live API
  slug: convai-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-live-api-openapi.yml
consequence_counts:
  read: 3
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Convai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'Convai exposes 34 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 31 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Convai
provider_slug: convai-com
slug: convai-com-agentic-access
source_filename: convai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/convai-character-api-openapi.yml, openapi/convai-chat-history-api-openapi.yml,\n  openapi/convai-custom-llm-api-openapi.yml, openapi/convai-evaluation-api-openapi.yml, openapi/convai-interaction-api-openapi.yml,\n  openapi/convai-knowledge-bank-api-openapi.yml, openapi/convai-live-api-openapi.yml, openapi/convai-narrative-design-api-openapi.yml,\n  openapi/convai-streaming-transcription-api-openapi.yml, openapi/convai-tts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 31\n    connected: 3\n  by_consequence:\n    write: 31\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /character/create\n  method: post\n  operationId:\
  \ createCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/get\n  method: post\n  operationId: getCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/update\n  method: post\n  operationId: updateCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /character/list\n  method: post\n  operationId: listCharacters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/delete\n  method: post\n  operationId: deleteCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/clone_character\n  method: post\n  operationId: cloneCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /character/chat-history/list-sessions\n  method: post\n  operationId: listSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/chat-history/get-session\n  method: post\n  operationId: getSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-llm/register\n  method: post\n  operationId: registerCustomLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-llm/update\n  method: post\n  operationId: updateCustomLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-llm/deregister\n  method: post\n  operationId: deregisterCustomLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-llm/list\n  method: post\n  operationId: listCustomLLMs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluation/evaluate-session\n  method: post\n  operationId: evaluateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/getResponse\n  method: post\n  operationId: getCharacterResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/knowledge-bank/upload\n  method: post\n  operationId: uploadKnowledgeBank\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/knowledge-bank/update\n  method: post\n  operationId: updateKnowledgeBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/knowledge-bank/list\n  method: post\n  operationId: listKnowledgeBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /character/knowledge-bank/delete\n  method: post\n  operationId: deleteKnowledgeBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connect\n  method: post\n  operationId: connectLiveSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/toggle-is-narrative-driven\n  method: post\n  operationId: toggleNarrativeDriven\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/create-section\n  method: post\n  operationId: createSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/edit-section\n  method: post\n  operationId: editSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/get-section\n  method: post\n  operationId: getSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/list-sections\n  method: post\n  operationId: listSections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/delete-section\n  method: post\n  operationId: deleteSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/create-trigger\n  method: post\n  operationId: createTrigger\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/update-trigger\n  method: post\n  operationId: updateTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/get-trigger\n  method: post\n  operationId: getTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /character/narrative/list-triggers\n  method: post\n  operationId: listTriggers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character/narrative/delete-trigger\n  method: post\n  operationId: deleteTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stream\n  method: get\n  operationId: openTranscriptionStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts\n  method: post\n  operationId: synthesizeSpeech\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/get_available_voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/get_available_languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/agentic-access/convai-com-agentic-access.yml
summary_line: 34 operations · 31 acting
tags:
- AI
- Conversational AI
- Characters
- NPCs
- Virtual Worlds
- Games
- Avatars
- Speech
- TTS
- WebRTC
---
