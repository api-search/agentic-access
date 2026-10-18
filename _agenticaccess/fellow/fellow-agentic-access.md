---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: fellow-action-items-api-openapi.yml
  format: yaml
  label: Fellow Action Items API
  slug: fellow-action-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/openapi/fellow-action-items-api-openapi.yml
- filename: fellow-notes-api-openapi.yml
  format: yaml
  label: Fellow Notes API
  slug: fellow-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/openapi/fellow-notes-api-openapi.yml
- filename: fellow-recordings-api-openapi.yml
  format: yaml
  label: Fellow Recordings API
  slug: fellow-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/openapi/fellow-recordings-api-openapi.yml
- filename: fellow-users-api-openapi.yml
  format: yaml
  label: Fellow Users API
  slug: fellow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/openapi/fellow-users-api-openapi.yml
- filename: fellow-webhooks-api-openapi.yml
  format: yaml
  label: Fellow Webhooks API
  slug: fellow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/openapi/fellow-webhooks-api-openapi.yml
consequence_counts:
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fellow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Fellow exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fellow
provider_slug: fellow
slug: fellow-agentic-access
source_filename: fellow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/fellow-developer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/action_item/{action_item_id}\n  method: get\n  operationId: apps_developer_api_api_get_action_item_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/action_item/{action_item_id}/archive\n  method: post\n  operationId: apps_developer_api_api_archive_action_item\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/action_item/{action_item_id}/complete\n  method: post\n  operationId: apps_developer_api_api_mark_action_item_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/action_items\n  method: post\n  operationId: apps_developer_api_api_get_action_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: apps_developer_api_api_get_authenticated_user\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/note/{note_id}\n  method: get\n  operationId: apps_developer_api_api_get_note_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/note/{note_id}\n  method: delete\n  operationId: apps_developer_api_api_delete_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/note/{note_id}/agenda\n  method: post\n  operationId: apps_developer_api_api_write_note_agenda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/note/{note_id}/agenda/append\n  method: post\n  operationId: apps_developer_api_api_append_note_agenda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/note/{note_id}/agenda/find-replace\n  method: post\n  operationId: apps_developer_api_api_find_replace_note_agenda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/note/{note_id}/agenda/prepend\n  method: post\n  operationId: apps_developer_api_api_prepend_note_agenda\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/notes\n  method: post\n  operationId: apps_developer_api_api_get_notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recording/{recording_id}\n  method: get\n  operationId: apps_developer_api_api_get_recording_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recording/{recording_id}\n  method: delete\n  operationId: apps_developer_api_api_delete_recording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recordings\n  method: post\n  operationId: apps_developer_api_api_get_recordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recordings/upload\n  method: post\n  operationId: apps_developer_api_api_upload_recording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recordings/upload/list\n  method: post\n  operationId: apps_developer_api_api_list_uploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recordings/upload/{recording_id}\n  method: get\n  operationId: apps_developer_api_api_get_upload_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook\n  method: post\n  operationId: apps_developer_api_api_create_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook/{webhook_id}\n  method: get\n  operationId: apps_developer_api_api_get_webhook_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook/{webhook_id}\n  method: patch\n \
  \ operationId: apps_developer_api_api_update_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook/{webhook_id}\n  method: delete\n  operationId: apps_developer_api_api_delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks\n  method: get\n  operationId: apps_developer_api_api_list_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/agentic-access/fellow-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Company
- Software-as-a-Service
- Meetings
- Artificial Intelligence
- Meeting Notes
- Transcription
- Productivity
- Action Items
- Webhook
- MCP
---
