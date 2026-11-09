---
acting_count: 138
action_class_counts:
  acting: 138
  connected: 70
api_specs:
- filename: beatra-ai-account-api-openapi.yml
  format: yaml
  label: Beatra AI Account API
  slug: beatra-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-account-api-openapi.yml
- filename: beatra-ai-account-feedback-api-openapi.yml
  format: yaml
  label: Beatra AI Account Feedback API
  slug: beatra-ai-account-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-account-feedback-api-openapi.yml
- filename: beatra-ai-audio-api-openapi.yml
  format: yaml
  label: Beatra AI Audio API
  slug: beatra-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-audio-api-openapi.yml
- filename: beatra-ai-catalog-api-openapi.yml
  format: yaml
  label: Beatra AI Catalog API
  slug: beatra-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-catalog-api-openapi.yml
- filename: beatra-ai-health-api-openapi.yml
  format: yaml
  label: Beatra AI Health API
  slug: beatra-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-health-api-openapi.yml
- filename: beatra-ai-images-api-openapi.yml
  format: yaml
  label: Beatra AI Images API
  slug: beatra-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-images-api-openapi.yml
- filename: beatra-ai-mcp-device-authorization-api-openapi.yml
  format: yaml
  label: Beatra AI MCP Device Authorization API
  slug: beatra-ai-mcp-device-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-mcp-device-authorization-api-openapi.yml
- filename: beatra-ai-music-api-openapi.yml
  format: yaml
  label: Beatra AI Music API
  slug: beatra-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-music-api-openapi.yml
- filename: beatra-ai-payments-api-openapi.yml
  format: yaml
  label: Beatra AI Payments API
  slug: beatra-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-payments-api-openapi.yml
- filename: beatra-ai-tasks-api-openapi.yml
  format: yaml
  label: Beatra AI Tasks API
  slug: beatra-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-tasks-api-openapi.yml
- filename: beatra-ai-uploads-api-openapi.yml
  format: yaml
  label: Beatra AI Uploads API
  slug: beatra-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-uploads-api-openapi.yml
- filename: beatra-ai-videos-api-openapi.yml
  format: yaml
  label: Beatra AI Videos API
  slug: beatra-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-videos-api-openapi.yml
- filename: beatra-ai-voices-api-openapi.yml
  format: yaml
  label: Beatra AI Voices API
  slug: beatra-ai-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-voices-api-openapi.yml
- filename: beatra-ai-webhooks-api-openapi.yml
  format: yaml
  label: Beatra AI Webhooks API
  slug: beatra-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-webhooks-api-openapi.yml
- filename: beatra-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Beatra AI Chat Completions API
  slug: beatra-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatra-ai/openapi/beatra-ai-chat-completions-api-openapi.yml
consequence_counts:
  physical: 18
  read: 70
  safety-critical: 4
  write: 116
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Beatra Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /account/api-keys/{api_key_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /account/connected-agents/{installation_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/work-shares/artifact/{artifact_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/device/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/feedback/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/invoices/{invoice_request_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-miniapp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-miniapp/cashier-result
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-miniapp/opened
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-miniapp/sign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-virtual
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-virtual/cashier-result
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/wechat-virtual/sign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/{payment_order_id}/mock-complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-orders/{payment_order_id}/payer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/webhooks/stripe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/images/image-to-image
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/images/image-to-image
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/videos/reference-to-video
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/videos/reference-to-video
operation_count: 208
overview: 'Beatra AI exposes 208 API operations that an AI agent could call, of which 138 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 70 read, 116 write, 18 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beatra AI
provider_slug: beatra-ai
slug: beatra-ai-agentic-access
source_filename: beatra-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/beatra-ai-api-openapi.json, openapi/beatra-ai-docs-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 208\n  by_action_class:\n    connected: 70\n    acting: 138\n  by_consequence:\n    read: 70\n    write: 116\n    physical: 18\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/models\n  method: get\n  operationId: list_models_openai_compat_v1_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/models\n  method: get\n  operationId: list_catalog_models_v1_catalog_models_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/capabilities\n  method: get\n  operationId: list_capabilities_v1_catalog_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/capabilities/{capability}\n  method: get\n  operationId: get_capability_v1_catalog_capabilities__capability__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/models/{model}\n  method: get\n  operationId: get_model_v1_catalog_models__model__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  operationId: chat_completions_v1_chat_completions_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method: post\n  operationId: images_generations_v1_images_generations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/image-to-image\n  method: post\n  operationId: images_i2i_v1_images_image_to_image_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/edits\n  method: post\n  operationId: images_edits_v1_images_edits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/responses\n  method: post\n  operationId: images_responses_v1_images_responses_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/prompts/enhance\n  method: post\n  operationId: videos_enhance_prompt_v1_videos_prompts_enhance_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/text-to-video\n  method: post\n  operationId: videos_t2v_v1_videos_text_to_video_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/image-to-video\n  method: post\n  operationId: videos_i2v_v1_videos_image_to_video_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/reference-to-video\n\
  \  method: post\n  operationId: videos_r2v_v1_videos_reference_to_video_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/frames-to-video\n  method: post\n  operationId: videos_f2v_v1_videos_frames_to_video_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/edit\n  method: post\n  operationId: videos_edit_v1_videos_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/extend\n  method: post\n  operationId: videos_extend_v1_videos_extend_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/compose\n  method: post\n  operationId: videos_compose_v1_videos_compose_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/responses\n  method: post\n  operationId: videos_responses_v1_videos_responses_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music/text-to-music\n  method: post\n  operationId: text_to_music_v1_music_text_to_music_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music/reference-audio-to-music\n  method: post\n  operationId: ref_audio_to_music_v1_music_reference_audio_to_music_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/speech\n  method: post\n  operationId: text_to_speech_v1_audio_speech_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/speech/validate\n  method: post\n  operationId: validate_text_to_speech_v1_audio_speech_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n  method: get\n  operationId: list_voices_v1_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices\n  method: post\n  operationId: clone_voice_v1_voices_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices/{voice_id}\n  method: get\n  operationId: get_voice_v1_voices__voice_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices/{voice_id}\n  method: delete\n  operationId: delete_voice_v1_voices__voice_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/voices/{voice_id}/activate\n  method: post\n  operationId: activate_voice_v1_voices__voice_id__activate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: post\n  operationId: upload_v1_uploads_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks\n  method: get\n  operationId: list_tasks_v1_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/tasks/{task_id}\n  method: get\n  operationId: get_task_v1_tasks__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/{task_id}/cancel\n  method: post\n  operationId: cancel_task_v1_tasks__task_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/readyz\n  method: get\n  operationId: readyz_v1_readyz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/livez\n  method: get\n  operationId: livez_v1_livez_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{provider_id}\n  method: post\n  operationId: receive_webhooks__provider_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/oauth/{provider}/start\n  method: get\n  operationId: oauth_start_account_oauth__provider__start_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/oauth/google/id-token\n  method: post\n  operationId:\
  \ oauth_google_id_token_account_oauth_google_id_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/oauth/apple/id-token\n  method: post\n  operationId: oauth_apple_id_token_account_oauth_apple_id_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/oauth/{provider}/callback\n  method: post\n  operationId: oauth_callback_account_oauth__provider__callback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/visitor-context\n  method: get\n  operationId: visitor_context_account_visitor_context_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/country-options\n  method: get\n  operationId: country_options_account_country_options_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/profile\n  method: get\n  operationId: profile_account_profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/profile\n  method: patch\n  operationId: update_profile_account_profile_patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/acct-hint\n  method: get\n  operationId: acct_hint_account_acct_hint_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/profile/display-name\n  method: patch\n  operationId: update_display_name_account_profile_display_name_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/avatar\n  method: put\n  operationId: update_avatar_account_profile_avatar_put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/avatar\n  method: delete\n  operationId: delete_avatar_account_profile_avatar_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/delete\n  method: post\n  operationId: delete_account_account_delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /account/auth/challenges\n  method: post\n  operationId: create_auth_challenge_account_auth_challenges_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/auth/challenges/{challenge_id}\n  method: get\n  operationId: auth_challenge_status_account_auth_challenges__challenge_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/auth/challenges/{challenge_id}/verify\n  method: post\n  operationId: verify_auth_challenge_account_auth_challenges__challenge_id__verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/auth/wechat-miniprogram/grant\n  method: post\n  operationId: grant_wechat_miniprogram_login_account_auth_wechat_miniprogram_grant_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/auth/wechat-miniprogram/redeem\n  method: post\n  operationId: redeem_wechat_miniprogram_login_account_auth_wechat_miniprogram_redeem_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /account/session/logout\n  method: post\n  operationId: logout_browser_session_account_session_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/session/renew\n  method: post\n  operationId: renew_browser_session_account_session_renew_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/agent-link/land\n  method: post\n  operationId: land_agent_link_account_agent_link_land_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/session/handoff\n  method: post\n  operationId: issue_session_handoff_account_session_handoff_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/session/handoff/redeem\n  method: post\n  operationId: redeem_session_handoff_account_session_handoff_redeem_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /account/session/handoff/peek\n  method: post\n  operationId: peek_session_handoff_account_session_handoff_peek_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/me\n  method: get\n  operationId: me_account_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/billing\n  method: get\n  operationId: billing_account_billing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/billing/overview\n  method: get\n  operationId: billing_overview_account_billing_overview_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/billing/ledger\n  method: get\n  operationId: billing_ledger_account_billing_ledger_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/billing/catalog\n  method: get\n  operationId: billing_catalog_account_billing_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/connected-agents\n  method: get\n  operationId: connected_agents_account_connected_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/connected-agents/{installation_id}/connection\n  method: get\n  operationId: connected_agent_connection_account_connected_agents__installation_id__connection_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/connected-agents/{installation_id}\n  method: patch\n  operationId: rename_connected_agent_account_connected_agents__installation_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/connected-agents/{installation_id}\n  method: delete\n  operationId: dismiss_connected_agent_account_connected_agents__installation_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /account/connected-agents/{installation_id}/revoke\n  method: post\n  operationId: revoke_connected_agent_account_connected_agents__installation_id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/payment-orders\n  method: get\n  operationId: payment_orders_account_payment_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/payment-orders\n  method: post\n  operationId: create_payment_order_account_payment_orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/payment-orders/{payment_order_id}/status\n  method: get\n  operationId: payment_order_status_account_payment_orders__payment_order_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/payment-orders/{payment_order_id}/receipt\n  method: get\n  operationId: payment_order_receipt_account_payment_orders__payment_order_id__receipt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/invoiceable-orders\n  method: get\n  operationId: invoiceable_orders_account_invoiceable_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/invoices\n  method: get\n  operationId: list_invoices_account_invoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/invoices\n  method: post\n  operationId: create_invoice_account_invoices_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/offers/free-video\n  method: get\n  operationId: read_free_video_offer_account_offers_free_video_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /account/offers/free-video/claim\n  method: post\n  operationId: claim_free_video_offer_account_offers_free_video_claim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/invoices/{invoice_request_id}/cancel\n  method: post\n  operationId: cancel_invoice_account_invoices__invoice_request_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/invoices/{invoice_request_id}/file\n  method: get\n  operationId: invoice_file_account_invoices__invoice_request_id__file_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/subscriptions\n  method: get\n  operationId: subscriptions_account_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/subscriptions/{subscription_id}/cancel\n  method: post\n  operationId: cancel_subscription_account_subscriptions__subscription_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/payment-orders/{payment_order_id}/payer\n  method: post\n  operationId: complete_payment_order_payer_account_payment_orders__payment_order_id__payer_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/wechat-payer/start\n  method: post\n  operationId: start_wechat_payer_account_wechat_payer_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/wechat-payer\n  method: post\n  operationId: complete_wechat_payer_account_wechat_payer_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/payment-orders/{payment_order_id}/mock-complete\n  method: post\n  operationId: mock_complete_payment_order_account_payment_orders__payment_order_id__mock_complete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/work-shares\n  method: post\n  operationId: create_work_share_account_work_shares_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /account/work-shares/artifact/{artifact_id}\n  method: get\n  operationId: work_share_state_account_work_shares_artifact__artifact_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/work-shares/artifact/{artifact_id}\n  method: delete\n  operationId: revoke_work_share_account_work_shares_artifact__artifact_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/work-shares/{share_id}\n  method: get\n  operationId: open_work_share_account_work_shares__share_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /account/wechat/js-sdk\n  method: post\n  operationId: wechat_js_sdk_config_account_wechat_js_sdk_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/assets\n  method: get\n  operationId: assets_account_assets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/capabilities\n  method: get\n  operationId: capabilities_account_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/api-keys\n  method: post\n  operationId: create_key_account_api_keys_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/api-keys\n  method: get\n  operationId: list_keys_account_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (70 KB total) ---\n# Full source: https://artifacts.apis.io/beatra-ai/agentic-access/beatra-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/beatra-ai/agentic-access/beatra-ai-agentic-access.yml
summary_line: 208 operations · 138 acting · 4 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Multi-Modal
- Generation
- Social Data
---
