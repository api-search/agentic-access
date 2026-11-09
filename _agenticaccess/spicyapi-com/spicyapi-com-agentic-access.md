---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 27
api_specs:
- filename: spicyapi-com-agent-tools-api-openapi.yml
  format: yaml
  label: spicyapi-com Agent tools API
  slug: spicyapi-com-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-agent-tools-api-openapi.yml
- filename: spicyapi-com-audio-api-openapi.yml
  format: yaml
  label: spicyapi-com Audio API
  slug: spicyapi-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-audio-api-openapi.yml
- filename: spicyapi-com-characters-api-openapi.yml
  format: yaml
  label: spicyapi-com Characters API
  slug: spicyapi-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-characters-api-openapi.yml
- filename: spicyapi-com-core-api-openapi.yml
  format: yaml
  label: spicyapi-com Core API
  slug: spicyapi-com-core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-core-api-openapi.yml
- filename: spicyapi-com-default-api-openapi.yml
  format: yaml
  label: spicyapi-com Default API
  slug: spicyapi-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-default-api-openapi.yml
- filename: spicyapi-com-embeddings-api-openapi.yml
  format: yaml
  label: spicyapi-com Embeddings API
  slug: spicyapi-com-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-embeddings-api-openapi.yml
- filename: spicyapi-com-guarded-api-openapi.yml
  format: yaml
  label: spicyapi-com Guarded API
  slug: spicyapi-com-guarded-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-guarded-api-openapi.yml
- filename: spicyapi-com-images-api-openapi.yml
  format: yaml
  label: spicyapi-com Images API
  slug: spicyapi-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-images-api-openapi.yml
- filename: spicyapi-com-live-calls-api-openapi.yml
  format: yaml
  label: spicyapi-com Live calls API
  slug: spicyapi-com-live-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-live-calls-api-openapi.yml
- filename: spicyapi-com-moderation-api-openapi.yml
  format: yaml
  label: spicyapi-com Moderation API
  slug: spicyapi-com-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-moderation-api-openapi.yml
- filename: spicyapi-com-video-api-openapi.yml
  format: yaml
  label: spicyapi-com Video API
  slug: spicyapi-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-video-api-openapi.yml
- filename: spicyapi-com-chat-completions-api-openapi.yml
  format: yaml
  label: spicyapi-com Chat Completions API
  slug: spicyapi-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spicyapi-com/openapi/spicyapi-com-chat-completions-api-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 1
  write: 39
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Spicyapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/tools/revoke_api_key
operation_count: 67
overview: 'spicyapi-com exposes 67 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 39 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: spicyapi-com
provider_slug: spicyapi-com
slug: spicyapi-com-agentic-access
source_filename: spicyapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/spicyapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 67\n  by_action_class:\n    connected: 27\n    acting: 40\n  by_consequence:\n    read: 27\n    write: 39\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/generations\n\
  \  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/edits\n  method: post\n  operationId: editImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/styles\n  method: get\n  operationId: listStyles\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/moderations\n  method: post\n  operationId: moderations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/end-users/{user}\n  method: delete\n  operationId: eraseEndUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/moderations/appeals\n  method: post\n  operationId: moderationAppeals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: post\n  operationId: createCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: get\n  operationId: listCharacters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/characters/import\n  method: post\n  operationId: importCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters/{id}\n  method: delete\n  operationId: deleteCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters/{id}/views\n  method: post\n  operationId: addCharacterView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters/{id}/views/{view_id}\n  method: delete\n  operationId: deleteCharacterView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n  method: post\n  operationId: createVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices/{id}\n  method: delete\n  operationId: deleteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio\n  method: post\n  operationId: uploadAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio\n  method: get\n  operationId: listAudio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/{id}\n  method: delete\n  operationId: deleteAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/generations\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/videos/tasks/{id}\n  method: get\n  operationId: getVideoTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/edits\n  method: post\n  operationId: createVideoEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/motions\n  method: get\n  operationId: listMotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/actions\n  method: get\n  operationId: listActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/images/actions\n  method: get\n  operationId: listImageActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  operationId: chatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/sessions\n  method: post\n  operationId: createRealtimeSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime\n  method: get\n  operationId: realtimeWebsocket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_models\n  method: post\n  operationId: tool_list_models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/estimate_cost\n  method: post\n  operationId:\
  \ tool_estimate_cost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/get_account\n  method: post\n  operationId: tool_get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_images\n  method: post\n  operationId: tool_list_images\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_characters\n  method: post\n  operationId: tool_list_characters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/tools/create_character\n  method: post\n  operationId: tool_create_character\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/add_character_view\n  method: post\n  operationId: tool_add_character_view\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/delete_character\n  method: post\n  operationId: tool_delete_character\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/generate_image\n  method: post\n  operationId: tool_generate_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/edit_image\n  method: post\n  operationId: tool_edit_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/generate_video\n  method: post\n  operationId: tool_generate_video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/edit_video\n  method: post\n  operationId: tool_edit_video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/list_motions\n  method: post\n  operationId: tool_list_motions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_actions\n  method: post\n  operationId: tool_list_actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/tools/list_image_actions\n  method: post\n  operationId: tool_list_image_actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_styles\n  method: post\n  operationId: tool_list_styles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/upload_audio\n  method: post\n  operationId: tool_upload_audio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/list_audio\n  method: post\n  operationId: tool_list_audio\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/delete_audio\n  method: post\n  operationId: tool_delete_audio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/transcribe_audio\n  method: post\n  operationId: tool_transcribe_audio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/generate_speech\n  method: post\n  operationId: tool_generate_speech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/list_voices\n  method: post\n  operationId: tool_list_voices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/create_voice\n  method: post\n  operationId: tool_create_voice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/delete_voice\n  method: post\n  operationId: tool_delete_voice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/create_embeddings\n  method: post\n  operationId: tool_create_embeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/get_job\n  method: post\n  operationId: tool_get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/list_jobs\n  method: post\n  operationId: tool_list_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/get_usage\n  method:\
  \ post\n  operationId: tool_get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/create_api_key\n  method: post\n  operationId: tool_create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/revoke_api_key\n  method: post\n  operationId: tool_revoke_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/tools/get_topup_link\n  method:\
  \ post\n  operationId: tool_get_topup_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/set_spend_limit\n  method: post\n  operationId: tool_set_spend_limit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/read_acceptable_use\n  method: post\n  operationId: tool_read_acceptable_use\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/spicyapi-com/agentic-access/spicyapi-com-agentic-access.yml
summary_line: 67 operations · 40 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Adult
- Image Generation
- Video Generation
- Voice
---
