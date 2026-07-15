---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 23
api_specs:
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Voices API
  slug: respeecher-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Speech-to-Speech Conversion API
  slug: respeecher-speech-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Text-to-Speech API
  slug: respeecher-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Calibration API
  slug: respeecher-calibration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Recordings API
  slug: respeecher-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Projects and Folders API
  slug: respeecher-projects-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Credits API
  slug: respeecher-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-asyncapi.yml
  format: yaml
  label: Respeecher Space Real-Time TTS API
  slug: respeecher-space-realtime-tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/asyncapi/respeecher-asyncapi.yml
consequence_counts:
  physical: 3
  read: 23
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Respeecher Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/recordings/conversion-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/orders/retry/{recording_id}
operation_count: 54
overview: 'Respeecher exposes 54 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 28 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Respeecher
provider_slug: respeecher
slug: respeecher-agentic-access
source_filename: respeecher-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/respeecher-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 23\n    acting: 31\n  by_consequence:\n    read: 23\n    write: 28\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/healtz\n  method: get\n  operationId: healtz_api_healtz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/login\n  method: post\n  operationId: login_api_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/logout\n  method: post\n  operationId: logout_api_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth\n  method: post\n  operationId: authenticate_api_auth_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calibration\n  method: get\n  operationId: calibration_list_api_calibration_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calibration\n  method: post\n  operationId: calibrate_api_calibration_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calibration/{calibration_id}\n  method: get\n  operationId: calibration_get_api_calibration__calibration_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calibration/{calibration_id}\n  method: delete\n  operationId: calibration_delete_api_calibration__calibration_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calibration/{calibration_id}\n  method: patch\n  operationId: calibration_rename_api_calibration__calibration_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calibration/{calibration_id}/enable\n  method: put\n  operationId: calibration_enable_api_calibration__calibration_id__enable_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/credits\n  method: get\n  operationId: get_credits_api_credits_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/models\n  method: get\n  operationId: model_list_api_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: get\n  operationId: project_list_api_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: post\n  operationId: project_create_api_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/by-url\n  method:\
  \ get\n  operationId: project_get_by_url_api_projects_by_url_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}\n  method: put\n  operationId: project_update_api_projects__project_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}\n  method: delete\n  operationId: project_delete_api_projects__project_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/projects/{project_id}\n  method: patch\n  operationId: project_rename_api_projects__project_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/export\n  method: get\n  operationId: project_export_api_projects__project_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/folders\n  method: get\n  operationId: folder_list_api_folders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/folders\n  method: post\n  operationId: folder_create_api_folders_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/folders/{folder_id}\n  method: get\n  operationId: folder_get_api_folders__folder_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/folders/{folder_id}\n  method: delete\n  operationId: folder_delete_api_folders__folder_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/folders/{folder_id}\n  method: patch\n  operationId: folder_rename_api_folders__folder_id__patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings\n  method: get\n  operationId: recording_list_api_recordings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recordings\n  method: post\n  operationId: recording_create_api_recordings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/originals\n  method: get\n  operationId: recording_list_originals_api_recordings_originals_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recordings/{recording_id}\n  method: get\n  operationId: recording_get_api_recordings__recording_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recordings/{recording_id}\n  method: put\n  operationId: recording_put_api_recordings__recording_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/{recording_id}\n  method: delete\n  operationId: recording_delete_api_recordings__recording_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/{recording_id}\n  method: patch\n  operationId: recording_patch_api_recordings__recording_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/conversions\n  method: get\n  operationId: recording_list_conversions_api_recordings_conversions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recordings/tts\n  method: post\n  operationId: recording_create_tts_api_recordings_tts_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/conversion-order\n  method: post\n  operationId: recording_conversion_order_api_recordings_conversion_order_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/conversion-redo/{recording_id}\n  method: post\n  operationId: recording_conversion_redo_api_recordings_conversion_redo__recording_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recordings/export\n  method: get\n  operationId: take_export_api_recordings_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tts-voices\n  method: get\n  operationId: tts_voice_list_api_tts_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notes\n  method: get\n  operationId: note_list_api_notes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notes\n  method: put\n  operationId: note_update_api_notes_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notes\n  method: post\n  operationId: note_create_api_notes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notes\n  method: delete\n  operationId: note_delete_api_notes_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stats\n  method: get\n  operationId: get_stats_api_stats_get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats/projects\n  method: post\n  operationId: get_project_stats_api_stats_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stats/folders\n  method: post\n  operationId: get_folder_stats_api_stats_folders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{file_url}\n  method: get\n  operationId: get_file_api__file_url__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recordings/tts\n  method: post\n  operationId: recording_create_tts_v2_api_v2_recordings_tts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders\n  method: post\n  operationId: conversion_order_create_api_v2_orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders/retry/{recording_id}\n  method:\
  \ post\n  operationId: conversion_order_retry_api_v2_orders_retry__recording_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/voices\n  method: get\n  operationId: voice_list_api_v2_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/voices/search\n  method: get\n  operationId: voice_search_api_v2_voices_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/voices/favorite/{voice_id}\n  method: post\n  operationId: voice_favorite_api_v2_voices_favorite__voice_id__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/voices/settings\n  method: post\n  operationId: voice_settings_api_v2_voices_settings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accents/samples\n  method: get\n  operationId: accent_get_samples_api_v2_accents_samples_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/narration-styles/samples\n  method: get\n  operationId: narration_style_get_samples_api_v2_narration_styles_samples_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/agentic-access/respeecher-agentic-access.yml
summary_line: 54 operations · 31 acting
tags:
- Voice AI
- Voice Cloning
- Speech to Speech
- Text to Speech
- Voice Conversion
- Real Time
- Media and Entertainment
---
