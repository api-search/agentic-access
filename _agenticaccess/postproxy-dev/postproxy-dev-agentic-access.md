---
acting_count: 91
action_class_counts:
  acting: 91
  connected: 66
api_specs:
- filename: postproxy-dev-api-keys-api-openapi.yml
  format: yaml
  label: postproxy-dev API Keys API
  slug: postproxy-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-api-keys-api-openapi.yml
- filename: postproxy-dev-calendar-api-openapi.yml
  format: yaml
  label: postproxy-dev Calendar API
  slug: postproxy-dev-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-calendar-api-openapi.yml
- filename: postproxy-dev-comments-api-openapi.yml
  format: yaml
  label: postproxy-dev Comments API
  slug: postproxy-dev-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-comments-api-openapi.yml
- filename: postproxy-dev-direct-messages-api-openapi.yml
  format: yaml
  label: postproxy-dev Direct Messages API
  slug: postproxy-dev-direct-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-direct-messages-api-openapi.yml
- filename: postproxy-dev-facebook-page-api-openapi.yml
  format: yaml
  label: postproxy-dev Facebook Page API
  slug: postproxy-dev-facebook-page-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-facebook-page-api-openapi.yml
- filename: postproxy-dev-google-business-api-openapi.yml
  format: yaml
  label: postproxy-dev Google Business API
  slug: postproxy-dev-google-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-google-business-api-openapi.yml
- filename: postproxy-dev-instagram-api-openapi.yml
  format: yaml
  label: postproxy-dev Instagram API
  slug: postproxy-dev-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-instagram-api-openapi.yml
- filename: postproxy-dev-pinterest-api-openapi.yml
  format: yaml
  label: postproxy-dev Pinterest API
  slug: postproxy-dev-pinterest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-pinterest-api-openapi.yml
- filename: postproxy-dev-placements-api-openapi.yml
  format: yaml
  label: postproxy-dev Placements API
  slug: postproxy-dev-placements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-placements-api-openapi.yml
- filename: postproxy-dev-posts-api-openapi.yml
  format: yaml
  label: postproxy-dev Posts API
  slug: postproxy-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-posts-api-openapi.yml
- filename: postproxy-dev-profile-comments-api-openapi.yml
  format: yaml
  label: postproxy-dev Profile Comments API
  slug: postproxy-dev-profile-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-profile-comments-api-openapi.yml
- filename: postproxy-dev-profile-groups-api-openapi.yml
  format: yaml
  label: postproxy-dev Profile Groups API
  slug: postproxy-dev-profile-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-profile-groups-api-openapi.yml
- filename: postproxy-dev-profiles-api-openapi.yml
  format: yaml
  label: postproxy-dev Profiles API
  slug: postproxy-dev-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-profiles-api-openapi.yml
- filename: postproxy-dev-queues-api-openapi.yml
  format: yaml
  label: postproxy-dev Queues API
  slug: postproxy-dev-queues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-queues-api-openapi.yml
- filename: postproxy-dev-webhooks-api-openapi.yml
  format: yaml
  label: postproxy-dev Webhooks API
  slug: postproxy-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-webhooks-api-openapi.yml
- filename: postproxy-dev-youtube-api-openapi.yml
  format: yaml
  label: postproxy-dev YouTube API
  slug: postproxy-dev-youtube-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-youtube-api-openapi.yml
- filename: postproxy-dev-whats-app-api-openapi.yml
  format: yaml
  label: postproxy-dev Whats App API
  slug: postproxy-dev-whats-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postproxy-dev/openapi/postproxy-dev-whats-app-api-openapi.yml
consequence_counts:
  physical: 2
  read: 66
  safety-critical: 6
  write: 83
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Postproxy Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/api_keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chats/{id}/pass_thread_control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chats/{id}/release_thread_control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chats/{id}/request_thread_control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chats/{id}/stop_typing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chats/{id}/take_thread_control
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chats/{chat_id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/profiles/{profile_id}/whatsapp/send_conversion_event
operation_count: 157
overview: 'postproxy-dev exposes 157 API operations that an AI agent could call, of which 91 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read, 83 write, 2 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: postproxy-dev
provider_slug: postproxy-dev
slug: postproxy-dev-agentic-access
source_filename: postproxy-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/postproxy-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 157\n  by_action_class:\n    connected: 66\n    acting: 91\n  by_consequence:\n    read: 66\n    write: 83\n    physical: 2\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /api/comments\n  method: get\n  operationId: comments_list_across_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts/{post_id}/comments\n  method: get\n  operationId: comments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/posts/{post_id}/comments\n  method: post\n  operationId: comments_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}\n  method: get\n  operationId: comments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts/{post_id}/comments/{id}\n  method: patch\n  operationId: comments_edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/posts/{post_id}/comments/{id}\n  method: delete\n  operationId: comments_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/hide\n  method: post\n  operationId: comments_hide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/unhide\n  method: post\n  operationId: comments_unhide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/like\n  method: post\n  operationId: comments_like\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/unlike\n  method: post\n  operationId: comments_unlike\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/pin\n  method: post\n  operationId: comments_pin\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/unpin\n  method: post\n  operationId: comments_unpin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{post_id}/comments/{id}/private_reply\n  method: post\n  operationId: dm_comment_private_reply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/profiles/{profile_id}/comments\n  method: get\n  operationId: profile_comments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/comments\n  method: post\n  operationId: profile_comments_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/comments/{id}\n  method: get\n  operationId: profile_comments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/comments/{id}\n  method: delete\n  operationId: profile_comments_delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/chats\n  method: get\n  operationId: dm_chats_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/chats\n  method: post\n  operationId: dm_chat_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chats/{id}\n  method: get\n  operationId: dm_chat_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chats/{chat_id}/messages\n  method: get\n  operationId: dm_messages_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chats/{chat_id}/messages\n  method: post\n  operationId: dm_message_send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}\n  method: get\n  operationId: dm_message_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/messages/{id}\n  method: patch\n  operationId: dm_message_edit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}/react\n  method: post\n  operationId: dm_message_react\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}/unreact\n  method: delete\n  operationId: dm_message_unreact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/chats/{id}/archive\n  method: post\n  operationId: dm_chat_archive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chats/{id}/archive\n  method: delete\n  operationId: dm_chat_unarchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chats/{id}/start_typing\n  method: post\n  operationId: dm_chat_start_typing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chats/{id}/stop_typing\n  method: post\n  operationId: dm_chat_stop_typing\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chats/{id}/pass_thread_control\n  method: post\n  operationId: dm_chat_pass_thread_control\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chats/{id}/take_thread_control\n  method: post\n  operationId: dm_chat_take_thread_control\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chats/{id}/release_thread_control\n  method: post\n  operationId: dm_chat_release_thread_control\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chats/{id}/request_thread_control\n  method: post\n  operationId: dm_chat_request_thread_control\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chats/{id}/thread_owner\n  method: get\n  operationId: dm_chat_thread_owner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/ice_breakers\n  method: get\n  operationId: dm_ice_breakers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/ice_breakers\n  method: post\n  operationId: dm_ice_breakers_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/profiles/{id}/ice_breakers\n  method: delete\n  operationId: dm_ice_breakers_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts\n  method: get\n  operationId: posts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts\n  method: post\n  operationId: posts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/stats\n  method: get\n  operationId: posts_stats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts/{id}\n  method: get\n  operationId: posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts/{id}\n  method: patch\n  operationId: posts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{id}\n  method: delete\n  operationId: posts_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/posts/{id}/publish\n  method: post\n  operationId: posts_publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/posts/{id}/delete_on_platform\n  method: post\n  operationId: posts_delete_on_platform\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/post_queues\n  method: get\n  operationId: queues_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/post_queues\n\
  \  method: post\n  operationId: queues_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/post_queues/{id}\n  method: get\n  operationId: queues_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/post_queues/{id}\n  method: patch\n  operationId: queues_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/post_queues/{id}\n  method: delete\n  operationId: queues_delete\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/post_queues/{id}/next_slot\n  method: get\n  operationId: queues_next_slot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar\n  method: get\n  operationId: calendar_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles\n  method: get\n  operationId: profiles_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}\n  method: get\n  operationId: profiles_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}\n  method: delete\n  operationId: profiles_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{id}/placements\n  method: get\n  operationId: profiles_placements_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/assign_placement_to_group\n  method: patch\n  operationId: profiles_assign_placement_to_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{id}/assign_to_group\n  method: patch\n  operationId: profiles_assign_to_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{id}/stats\n  method: get\n  operationId: profiles_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/follower_history\n  method: get\n  operationId: profiles_follower_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/daily_stats\n\
  \  method: get\n  operationId: profiles_daily_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/participants/{user_id}\n  method: get\n  operationId: profiles_participant_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/resolve_mention\n  method: get\n  operationId: profiles_resolve_mention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/backfill_posts\n  method: post\n  operationId: profiles_backfill_posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{id}/post_syncs\n  method: get\n  operationId: profiles_post_syncs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/post_syncs/{post_sync_id}\n  method: get\n  operationId: profiles_post_syncs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/backfill_chats\n  method: post\n  operationId: profiles_backfill_chats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{id}/chat_syncs\n  method: get\n\
  \  operationId: profiles_chat_syncs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{id}/chat_syncs/{chat_sync_id}\n  method: get\n  operationId: profiles_chat_syncs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/location\n  method: get\n  operationId: gb_location_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/update_location\n  method: patch\n  operationId: gb_location_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/available_location_categories\n  method: get\n  operationId: gb_location_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/update_hours\n  method: patch\n  operationId: gb_hours_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/attributes\n  method: get\n  operationId: gb_attributes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/profiles/{profile_id}/google_business/available_attributes\n  method: get\n  operationId: gb_attributes_available\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/update_attributes\n  method: patch\n  operationId: gb_attributes_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/service_list\n  method: get\n  operationId: gb_service_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/update_service_list\n\
  \  method: patch\n  operationId: gb_service_list_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/food_menus\n  method: get\n  operationId: gb_food_menus_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/update_food_menus\n  method: patch\n  operationId: gb_food_menus_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/profiles/{profile_id}/google_business/place_action_links\n  method: get\n  operationId: gb_place_action_links_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/available_place_action_types\n  method: get\n  operationId: gb_place_action_types_available\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/google_business/create_place_action_link\n  method: post\n  operationId: gb_place_action_link_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/update_place_action_link\n\
  \  method: patch\n  operationId: gb_place_action_link_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/delete_place_action_link\n  method: delete\n  operationId: gb_place_action_link_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/media\n  method: get\n  operationId: gb_media_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/profiles/{profile_id}/google_business/create_media\n  method: post\n  operationId: gb_media_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/delete_media\n  method: delete\n  operationId: gb_media_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/google_business/search_keywords\n  method: get\n  operationId: gb_search_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/facebook/page\n  method: get\n  operationId: fb_page_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/facebook/update_page\n  method: patch\n  operationId: fb_page_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/pinterest/create_board\n  method: post\n  operationId: pinterest_board_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/pinterest/delete_board\n  method: delete\n  operationId: pinterest_board_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/youtube/playlists\n  method: get\n  operationId: youtube_playlists_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/youtube/create_playlist\n  method: post\n  operationId: youtube_playlist_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/youtube/update_playlist\n  method: patch\n  operationId: youtube_playlist_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/youtube/delete_playlist\n  method: delete\n  operationId: youtube_playlist_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/instagram/available_audio\n  method: get\n  operationId: ig_available_audio\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/instagram/collaboration_invites\n  method: get\n  operationId: ig_collaboration_invites_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profiles/{profile_id}/instagram/accept_collaboration_invite\n  method: post\n  operationId: ig_collaboration_invite_accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles/{profile_id}/instagram/decline_collaboration_invite\n  method: post\n  operationId: ig_collaboration_invite_decline\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/placements\n  method: get\n  operationId: placements_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/placements/{id}/set_active_profile\n  method: patch\n  operationId: placements_set_active_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (48 KB total) ---\n# Full source: https://artifacts.apis.io/postproxy-dev/agentic-access/postproxy-dev-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/postproxy-dev/agentic-access/postproxy-dev-agentic-access.yml
summary_line: 157 operations · 91 acting · 6 human-in-the-loop
tags:
- Social Media
- Software-as-a-Service
- Marketing
- Automation
---
