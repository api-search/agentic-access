---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 38
api_specs:
- filename: superdocs-app-account-api-openapi.yml
  format: yaml
  label: superdocs-app Account API
  slug: superdocs-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-account-api-openapi.yml
- filename: superdocs-app-agents-api-openapi.yml
  format: yaml
  label: superdocs-app Agents API
  slug: superdocs-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-agents-api-openapi.yml
- filename: superdocs-app-approval-api-openapi.yml
  format: yaml
  label: superdocs-app Approval API
  slug: superdocs-app-approval-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-approval-api-openapi.yml
- filename: superdocs-app-attachments-api-openapi.yml
  format: yaml
  label: superdocs-app Attachments API
  slug: superdocs-app-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-attachments-api-openapi.yml
- filename: superdocs-app-chat-api-openapi.yml
  format: yaml
  label: superdocs-app Chat API
  slug: superdocs-app-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-chat-api-openapi.yml
- filename: superdocs-app-documents-api-openapi.yml
  format: yaml
  label: superdocs-app Documents API
  slug: superdocs-app-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-documents-api-openapi.yml
- filename: superdocs-app-downloads-api-openapi.yml
  format: yaml
  label: superdocs-app Downloads API
  slug: superdocs-app-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-downloads-api-openapi.yml
- filename: superdocs-app-health-api-openapi.yml
  format: yaml
  label: superdocs-app Health API
  slug: superdocs-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-health-api-openapi.yml
- filename: superdocs-app-jobs-api-openapi.yml
  format: yaml
  label: superdocs-app Jobs API
  slug: superdocs-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-jobs-api-openapi.yml
- filename: superdocs-app-mcp-api-openapi.yml
  format: yaml
  label: superdocs-app MCP API
  slug: superdocs-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-mcp-api-openapi.yml
- filename: superdocs-app-promo-api-openapi.yml
  format: yaml
  label: superdocs-app Promo API
  slug: superdocs-app-promo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-promo-api-openapi.yml
- filename: superdocs-app-sessions-api-openapi.yml
  format: yaml
  label: superdocs-app Sessions API
  slug: superdocs-app-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-sessions-api-openapi.yml
- filename: superdocs-app-templates-api-openapi.yml
  format: yaml
  label: superdocs-app Templates API
  slug: superdocs-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-templates-api-openapi.yml
- filename: superdocs-app-typebar-api-universal-document-ai-api-openapi.yml
  format: yaml
  label: 'superdocs-app Typebar API: Universal Document AI API'
  slug: superdocs-app-typebar-api-universal-document-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-typebar-api-universal-document-ai-api-openapi.yml
- filename: superdocs-app-uploads-api-openapi.yml
  format: yaml
  label: superdocs-app Uploads API
  slug: superdocs-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-uploads-api-openapi.yml
- filename: superdocs-app-users-api-openapi.yml
  format: yaml
  label: superdocs-app Users API
  slug: superdocs-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-users-api-openapi.yml
- filename: superdocs-app-well-known-api-openapi.yml
  format: yaml
  label: superdocs-app .well Known API
  slug: superdocs-app-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-well-known-api-openapi.yml
consequence_counts:
  read: 38
  safety-critical: 2
  write: 42
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Superdocs App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/chat/{session_id}/continue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/users/me/api-keys/{key_id}
operation_count: 82
overview: 'superdocs-app exposes 82 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 42 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: superdocs-app
provider_slug: superdocs-app
slug: superdocs-app-agentic-access
source_filename: superdocs-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/superdocs-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    acting: 44\n    connected: 38\n  by_consequence:\n    write: 42\n    read: 38\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/chat\n  method: post\n  operationId: chat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId: list_sessions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: get\n  operationId: list_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/cross-session-memory\n  method: delete\n  operationId: clear_cross_session_memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{document_id}\n  method: get\n  operationId: get_document_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{document_id}\n  method: patch\n  operationId: rename_document\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{document_id}\n  method: delete\n  operationId: archive_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{document_id}/unarchive\n  method: post\n  operationId: unarchive_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v1/sessions/{session_id}/documents/open\n  method: post\n  operationId: open_documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/init\n  method: post\n  operationId: init_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/documents/{document_id}/save\n  method: post\n  operationId: save_human_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/documents/{document_id}/unarchive\n  method: post\n  operationId: restore_document_keep_editing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/documents/blank\n  method: post\n  operationId: new_blank_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/documents\n  method: get\n  operationId:\
  \ list_session_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/doc-events\n  method: get\n  operationId: session_document_events_v1_sessions__session_id__doc_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/documents/{document_id}/focus\n  method: post\n  operationId: focus_session_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/documents/{document_id}\n  method: delete\n  operationId: close_session_document\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/chunks/{chunk_id}/re-edit\n  method: post\n  operationId: re_edit_chunk_on_user_version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/history\n  method: get\n  operationId: get_session_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/revert\n  method: post\n  operationId: revert_session_to_message\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/redo\n  method: post\n  operationId: redo_revert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/upload\n  method: post\n  operationId: upload_attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/{attachment_id}\n\
  \  method: delete\n  operationId: delete_attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/status/{session_id}\n  method: get\n  operationId: get_attachment_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/upload\n  method: post\n  operationId: upload_document_to_editor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/images/upload\n  method: post\n  operationId:\
  \ upload_inline_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/images/upload-base64\n  method: post\n  operationId: upload_image_base64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/limits/increase-request\n  method: post\n  operationId: request_limit_increase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/documents/export\n  method: post\n  operationId: export_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/export/email-request\n  method: post\n  operationId: request_large_export_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/upload-base64\n  method: post\n  operationId: upload_document_base64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/upload-base64\n  method: post\n  operationId: upload_attachment_base64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/upload-base64\n  method: post\n  operationId: upload_template_base64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: list_jobs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/jobs\n  method: get\n  operationId: get_session_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/async\n  method: post\n  operationId: chat_async\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/stream-token\n  method: post\n  operationId: create_stream_token_v1_chat_stream_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/{session_id}/stream\n  method: get\n  operationId: stream_chat_progress_v1_chat__session_id__stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/{session_id}/approve\n  method: post\n  operationId: approve_change\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/{session_id}/continue\n  method: post\n  operationId: continue_chat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/poll/{session_id}\n  method: get\n  operationId: poll_session_updates_v1_poll__session_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/upload\n  method: post\n  operationId: upload_user_template\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: list_user_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{template_id}\n  method: delete\n  operationId: delete_user_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/me\n  method: get\n  operationId: get_current_user_profile_v1_users_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me\n  method: patch\n  operationId: update_user_profile_v1_users_me_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/me/usage\n  method: get\n  operationId: get_user_usage_stats_v1_users_me_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/sessions\n  method: get\n  operationId: get_user_sessions_v1_users_me_sessions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/sessions/{session_id}\n  method:\
  \ delete\n  operationId: delete_user_session_v1_users_me_sessions__session_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/me/limits\n  method: get\n  operationId: check_user_limits_v1_users_me_limits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/api-keys\n  method: get\n  operationId: list_api_keys_v1_users_me_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/api-keys\n  method: post\n  operationId: create_api_key_v1_users_me_api_keys_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/me/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_v1_users_me_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/promo/redeem\n  method: post\n  operationId: redeem_promo_v1_promo_redeem_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/users/me/promotions\n  method: get\n  operationId: list_my_promotions_v1_users_me_promotions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: request_upload_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{upload_id}/process\n  method: post\n  operationId: process_uploaded_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/downloads\n  method: post\n  operationId: request_download_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/challenge\n  method: get\n  operationId: agent_challenge_v1_agents_challenge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/signup\n  method: post\n  operationId: agent_signup_v1_agents_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/whoami\n  method: get\n  operationId: get_account_status\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/handoff\n  method: post\n  operationId: agent_handoff_v1_agents_handoff_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/adopt\n  method: post\n  operationId: agent_adopt_v1_agents_adopt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/adopt-info\n  method: get\n  operationId: agent_adopt_info_v1_agents_adopt_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/request-upgrade\n  method: post\n  operationId: agent_request_upgrade_v1_agents_request_upgrade_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/deep\n  method: get\n  operationId: health_check_deep_health_deep_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/.well-known/oauth-protected-resource\n  method: get\n  operationId: oauth_protected_resource_mcp__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: oauth_protected_resource__well_known_oauth_protected_resource_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: oauth_protected_resource__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/.well-known/oauth-authorization-server\n\
  \  method: get\n  operationId: oauth_authorization_server_mcp__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server/mcp\n  method: get\n  operationId: oauth_authorization_server__well_known_oauth_authorization_server_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: oauth_authorization_server__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/.well-known/openid-configuration\n  method: get\n  operationId: openid_configuration_mcp__well_known_openid_configuration_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openid-configuration/mcp\n  method: get\n  operationId: openid_configuration__well_known_openid_configuration_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: openid_configuration__well_known_openid_configuration_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: mcp_server_card__well_known_mcp_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp-server-card\n  method: get\n  operationId:\
  \ mcp_server_card__well_known_mcp_server_card_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: api_catalog__well_known_api_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/superdocs-app/agentic-access/superdocs-app-agentic-access.yml
summary_line: 82 operations · 44 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Document Editing
- REST API
- MCP
- Software-as-a-Service
---
