---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: captions-mirage-openapi-original.json
  format: json
  label: Mirage Video API
  slug: mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/openapi/captions-mirage-openapi-original.json
consequence_counts:
  read: 12
  safety-critical: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Captions Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /internal/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /internal/rate-limits/overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /internal/rate-limits/overrides/{identifier}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /internal/rate-limits/overrides/{identifier}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /internal/rate-limits/overrides/{identifier}/invalidate-cache
operation_count: 23
overview: 'Captions exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 6 write, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Captions
provider_slug: captions
slug: captions-agentic-access
source_filename: captions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/captions-mirage-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 11\n    connected: 12\n  by_consequence:\n    write: 6\n    read: 12\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /v1/videos\n  method: post\n  operationId: create_video_generation_v1_videos_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: get\n  operationId: list_videos_v1_videos_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{video_id}\n  method: get\n  operationId: get_video_status_v1_videos__video_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{video_id}/content\n  method: get\n  operationId: get_video_content_v1_videos__video_id__content_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/captions\n  method: post\n  operationId: create_captioned_video_v1_videos_captions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/videos/captions/templates\n  method: get\n  operationId: list_caption_templates_v1_videos_captions_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/captions/templates/{template_id}\n  method: get\n  operationId: get_caption_template_v1_videos_captions_templates__template_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/text-to-speech/{voice_id}\n  method: post\n  operationId: generate_text_to_speech_v1_audio_text_to_speech__voice_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/meta/text_overlays\n  method: post\n  operationId: create_meta_text_overlay_v1_meta_text_overlays_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meta/text_overlays/{text_overlay_id}\n  method: get\n  operationId: get_meta_text_overlay_v1_meta_text_overlays__text_overlay_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/api-keys/generate\n  method: post\n  operationId: create_api_key_internal_api_keys_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internal/api-keys/{key_id}\n  method: post\n  operationId: revoke_api_key_internal_api_keys__key_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /internal/api-keys/user/{user_id}\n  method: get\n  operationId: list_user_api_keys_internal_api_keys_user__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/videos\n  method: post\n  operationId: create_video_internal_videos_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internal/videos/{video_id}\n  method: get\n  operationId: get_video_internal_videos__video_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/rate-limits/overrides\n  method: post\n  operationId: create_rate_limit_override_internal_rate_limits_overrides_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /internal/rate-limits/overrides\n  method: get\n  operationId: list_rate_limit_overrides_internal_rate_limits_overrides_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/rate-limits/overrides/{identifier}\n  method: get\n  operationId: get_rate_limit_override_internal_rate_limits_overrides__identifier__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/rate-limits/overrides/{identifier}\n  method: put\n  operationId: update_rate_limit_override_internal_rate_limits_overrides__identifier__put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /internal/rate-limits/overrides/{identifier}\n  method: delete\n  operationId:\
  \ delete_rate_limit_override_internal_rate_limits_overrides__identifier__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /internal/rate-limits/overrides/{identifier}/invalidate-cache\n  method: post\n  operationId: invalidate_rate_limit_override_cache_internal_rate_limits_overrides__identifier__invalidate_cache_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions/refs/heads/main/agentic-access/captions-agentic-access.yml
summary_line: 23 operations · 11 acting · 5 human-in-the-loop
tags:
- Company
- Video
- Artificial Intelligence
- Video Editing
- Video Generation
- Captions
- Subtitles
- Text to Speech
- AI Avatars
- Content Creation
- Media
---
