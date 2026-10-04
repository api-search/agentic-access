---
acting_count: 110
action_class_counts:
  acting: 110
  connected: 51
api_specs:
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip Events API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-authentication-api-openapi.yml
  format: yaml
  label: Zulip Authentication API
  slug: zulip-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-authentication-api-openapi.yml
- filename: zulip-bots-api-openapi.yml
  format: yaml
  label: Zulip Bots API
  slug: zulip-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-bots-api-openapi.yml
- filename: zulip-channels-api-openapi.yml
  format: yaml
  label: Zulip Channels API
  slug: zulip-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-channels-api-openapi.yml
- filename: zulip-drafts-api-openapi.yml
  format: yaml
  label: Zulip Drafts API
  slug: zulip-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-drafts-api-openapi.yml
- filename: zulip-invites-api-openapi.yml
  format: yaml
  label: Zulip Invites API
  slug: zulip-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-invites-api-openapi.yml
- filename: zulip-messages-api-openapi.yml
  format: yaml
  label: Zulip Messages API
  slug: zulip-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-messages-api-openapi.yml
- filename: zulip-mobile-api-openapi.yml
  format: yaml
  label: Zulip Mobile API
  slug: zulip-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-mobile-api-openapi.yml
- filename: zulip-navigation-views-api-openapi.yml
  format: yaml
  label: Zulip Navigation Views API
  slug: zulip-navigation-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-navigation-views-api-openapi.yml
- filename: zulip-real-time-events-api-openapi.yml
  format: yaml
  label: Zulip Real Time Events API
  slug: zulip-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-real-time-events-api-openapi.yml
- filename: zulip-reminders-api-openapi.yml
  format: yaml
  label: Zulip Reminders API
  slug: zulip-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-reminders-api-openapi.yml
- filename: zulip-scheduled-messages-api-openapi.yml
  format: yaml
  label: Zulip Scheduled Messages API
  slug: zulip-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-scheduled-messages-api-openapi.yml
- filename: zulip-server-and-organizations-api-openapi.yml
  format: yaml
  label: Zulip Server And Organizations API
  slug: zulip-server-and-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-server-and-organizations-api-openapi.yml
- filename: zulip-users-api-openapi.yml
  format: yaml
  label: Zulip Users API
  slug: zulip-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-users-api-openapi.yml
- filename: zulip-webhooks-api-openapi.yml
  format: yaml
  label: Zulip Webhooks API
  slug: zulip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-webhooks-api-openapi.yml
consequence_counts:
  physical: 8
  read: 51
  safety-critical: 2
  write: 100
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Zulip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /invites/multiuse/{invite_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /invites/{invite_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /channel_folders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invites
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invites/{invite_id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile_push/e2ee/test_notification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile_push/test_notification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /realm/linkifiers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /realm/profile_fields
operation_count: 161
overview: 'Zulip exposes 161 API operations that an AI agent could call, of which 110 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read, 100 write, 8 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zulip
provider_slug: zulip
slug: zulip-agentic-access
source_filename: zulip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/zulip-authentication-api-openapi.yml, openapi/zulip-bots-api-openapi.yml, openapi/zulip-channels-api-openapi.yml,\n  openapi/zulip-drafts-api-openapi.yml, openapi/zulip-invites-api-openapi.yml, openapi/zulip-messages-api-openapi.yml,\n  openapi/zulip-mobile-api-openapi.yml, openapi/zulip-navigation-views-api-openapi.yml, openapi/zulip-real-time-events-api-openapi.yml,\n  openapi/zulip-reminders-api-openapi.yml, openapi/zulip-scheduled-messages-api-openapi.yml,\n  openapi/zulip-server-and-organizations-api-openapi.yml, openapi/zulip-users-api-openapi.yml,\n  openapi/zulip-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 161\n  by_action_class:\n    connected:\
  \ 51\n    acting: 110\n  by_consequence:\n    read: 51\n    write: 100\n    physical: 8\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /fetch_api_key\n  method: post\n  operationId: fetch-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jwt/fetch_api_key\n  method: post\n  operationId: jwt-fetch-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dev_fetch_api_key\n  method: post\n  operationId: dev-fetch-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dev_list_users\n  method: get\n  operationId: dev-list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /bot_storage\n  method: get\n  operationId: get-bot-storage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bot_storage\n  method: put\n  operationId: update-bot-storage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bot_storage\n  method: delete\n  operationId: remove-bot-storage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_stream_id\n  method: get\n  operationId:\
  \ get-stream-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /default_streams\n  method: post\n  operationId: add-default-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /default_streams\n  method: delete\n  operationId: remove-default-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/{stream_id}/topics\n  method: get\n  operationId: get-stream-topics\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/subscriptions\n  method: get\n  operationId: get-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/subscriptions\n  method: post\n  operationId: subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/subscriptions\n  method: patch\n  operationId: update-subscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /users/me/subscriptions\n  method: delete\n  operationId: unsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/subscriptions/muted_topics\n  method: patch\n  operationId: mute-topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user_topics\n  method: post\n  operationId: update-user-topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/subscriptions/{stream_id}\n  method: get\n  operationId: get-subscription-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}/channels\n  method: get\n  operationId: get-user-channels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/subscriptions/properties\n  method: post\n  operationId: update-subscription-settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /users/me/subscriptions/{stream_id}\n  method: patch\n  operationId: update-subscription-property\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{stream_id}/members\n  method: get\n  operationId: get-subscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams\n  method: get\n  operationId: get-streams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{stream_id}\n  method: get\n  operationId: get-stream-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /streams/{stream_id}\n  method: delete\n  operationId: archive-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{stream_id}\n  method: patch\n  operationId: update-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{stream_id}/email_address\n  method: get\n  operationId: get-stream-email-address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /streams/{stream_id}/delete_topic\n  method: post\n  operationId: delete-topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/create\n  method: post\n  operationId: create-channel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel_folders/create\n  method: post\n  operationId: create-channel-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel_folders\n  method: get\n  operationId: get-channel-folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel_folders\n  method: patch\n  operationId: patch-channel-folders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel_folders/{channel_folder_id}\n  method: patch\n  operationId: update-channel-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/bigbluebutton/create\n  method: get\n  operationId: create-big-blue-button-video-call\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/nextcloud_talk/create\n  method: post\n  operationId: create-nextcloud-talk-video-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/webex/create\n  method: post\n  operationId: create-webex-video-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/constructorgroups/create\n  method: post\n  operationId: create-constructor-groups-video-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drafts\n  method: get\n  operationId: get-drafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drafts\n  method: post\n  operationId: create-drafts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /drafts/{draft_id}\n  method: patch\n  operationId: edit-draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drafts/{draft_id}\n  method: delete\n  operationId: delete-draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_snippets\n  method: get\n  operationId: get-saved-snippets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saved_snippets\n  method: post\n  operationId: create-saved-snippet\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_snippets/{saved_snippet_id}\n  method: patch\n  operationId: edit-saved-snippet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_snippets/{saved_snippet_id}\n  method: delete\n  operationId: delete-saved-snippet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /invites\n  method: get\n  operationId: get-invites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invites\n  method: post\n  operationId: send-invites\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites/multiuse\n  method: post\n  operationId: create-invite-link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites/{invite_id}\n\
  \  method: delete\n  operationId: revoke-email-invite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /invites/multiuse/{invite_id}\n  method: delete\n  operationId: revoke-invite-link\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /invites/{invite_id}/resend\n  method: post\n  operationId: resend-email-invite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mark_all_as_read\n  method: post\n  operationId: mark-all-as-read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mark_stream_as_read\n  method: post\n  operationId: mark-stream-as-read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mark_topic_as_read\n  method: post\n  operationId: mark-topic-as-read\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: get-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  operationId: send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/history\n  method: get\n  operationId: get-message-history\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/flags\n  method: post\n  operationId: update-message-flags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/flags/narrow\n  method: post\n  operationId: update-message-flags-for-narrow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/render\n  method: post\n  operationId: render-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/reactions\n  method: post\n  operationId: add-reaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/reactions\n  method: delete\n  operationId: remove-reaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/read_receipts\n  method: get\n  operationId: get-read-receipts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/matches_narrow\n  method: get\n  operationId: check-messages-match-narrow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{message_id}\n  method: get\n  operationId: get-message\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{message_id}\n  method: patch\n  operationId: update-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}\n  method:\
  \ delete\n  operationId: delete-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/report\n  method: post\n  operationId: report-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user_uploads\n  method: post\n  operationId: upload-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /thumbnail/status/{realm_id_str}/{filename}\n  method: get\n  operationId: check-thumbnail-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user_uploads/{realm_id_str}/{filename}\n  method: get\n  operationId: get-file-temporary-url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile_push/test_notification\n  method: post\n  operationId: test-notify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile_push/e2ee/test_notification\n  method: post\n\
  \  operationId: e2ee-test-notify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile_push/register\n  method: post\n  operationId: register-push-device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remotes/push/e2ee/register\n  method: post\n  operationId: register-remote-push-device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register_client_device\n  method: post\n  operationId: register-client-device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remove_client_device\n  method: post\n  operationId: remove-client-device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /navigation_views\n  method: get\n  operationId: get-navigation-views\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /navigation_views\n  method: post\n  operationId: add-navigation-view\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /navigation_views/{fragment}\n  method: patch\n  operationId: edit-navigation-view\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /navigation_views/{fragment}\n  method: delete\n  operationId: remove-navigation-view\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: get-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: delete\n  operationId: delete-queue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: post\n  operationId: register-queue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /real-time\n  method: post\n  operationId: postRealTime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest-error-handling\n  method: post\n  operationId: rest-error-handling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reminders\n  method: get\n  operationId: get-reminders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reminders\n  method: post\n  operationId: create-message-reminder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reminders/{reminder_id}\n  method: delete\n  operationId: delete-reminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled_messages\n  method: get\n  operationId: get-scheduled-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled_messages\n  method: post\n  operationId: create-scheduled-message\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled_messages/{scheduled_message_id}\n  method: patch\n  operationId: update-scheduled-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled_messages/{scheduled_message_id}\n  method: delete\n  operationId: delete-scheduled-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /realm/emoji/{emoji_name}\n  method: post\n  operationId: upload-custom-emoji\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realm/emoji/{emoji_name}\n  method: delete\n  operationId: deactivate-custom-emoji\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realm/emoji\n  method: get\n  operationId: get-custom-emoji\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realm/presence\n  method: get\n  operationId:\
  \ get-presence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realm/domains\n  method: get\n  operationId: get-realm-domains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realm/domains\n  method: post\n  operationId: add-realm-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realm/domains/{domain}\n  method: patch\n  operationId: patch-realm-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realm/domains/{domain}\n  method: delete\n  operationId: delete-realm-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realm/profile_fields\n  method: get\n  operationId: get-custom-profile-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realm/profile_fields\n  method: patch\n  operationId: reorder-custom-profile-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (49 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/agentic-access/zulip-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/agentic-access/zulip-agentic-access.yml
summary_line: 161 operations · 110 acting · 2 human-in-the-loop
tags:
- Collaboration
- Messaging
- Team Chat
- Webhook
---
