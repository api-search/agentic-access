---
acting_count: 272
action_class_counts:
  acting: 272
  connected: 206
api_specs:
- filename: unisson-openapi-original.json
  format: json
  label: Unisson Platform API
  slug: unisson-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/openapi/unisson-openapi-original.json
consequence_counts:
  physical: 10
  read: 206
  safety-critical: 28
  write: 234
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 28
kind: agentic-access
layout: agentic-access
method: generated
name: Unisson Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/agents/{agent_id}/triggers/{trigger_id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/apis/recordings/manual/{session_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/chat/conversations/{conversation_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{customer_id}/guests/invitations/{invitation_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{customer_id}/integrations/granola
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/checkout/accounts/{account_id}/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/checkout/accounts/{account_id}/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/mirakl/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/mirakl/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/productboard/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/productboard/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/razorpay/accounts/{account_id}/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/razorpay/accounts/{account_id}/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/samsara/accounts/{account_id}/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/samsara/accounts/{account_id}/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/snyk/accounts/{account_id}/assignments/{user_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/integrations/snyk/accounts/{account_id}/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/organizations/me/access-control/defaults
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/organizations/me/access-control/members/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/me/access-control/members/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/me/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/skills/{skill_id}/instruction-versions/{version_id}/revert
operation_count: 478
overview: 'Unisson exposes 478 API operations that an AI agent could call, of which 272 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 206 read, 234 write, 10 physical, and 28 safety-critical.


  28 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unisson
provider_slug: unisson
slug: unisson-agentic-access
source_filename: unisson-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/unisson-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 478\n  by_action_class:\n    connected: 206\n    acting: 272\n  by_consequence:\n    read: 206\n    write: 234\n    safety-critical: 28\n    physical: 10\n  human_in_the_loop_required: 28\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /readyz\n  method: get\n  operationId: readyz_readyz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents\n  method: get\n  operationId: list_agents_api_v1_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents\n  method: post\n  operationId: create_agent_api_v1_agents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/templates\n  method: get\n  operationId: list_templates_api_v1_agents_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/generate-from-description\n  method: post\n  operationId: generate_agent_from_description_api_v1_agents_generate_from_description_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/improve-instructions\n  method: post\n  operationId: improve_agent_instructions_api_v1_agents_improve_instructions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/from-template/{template_id}\n  method: post\n  operationId:\
  \ create_from_template_api_v1_agents_from_template__template_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}\n  method: get\n  operationId: get_agent_api_v1_agents__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}\n  method: put\n  operationId: update_agent_api_v1_agents__agent_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}\n\
  \  method: delete\n  operationId: delete_agent_api_v1_agents__agent_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/instruction-versions\n  method: get\n  operationId: list_instruction_versions_api_v1_agents__agent_id__instruction_versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}/instruction-versions/{version_id}\n  method: get\n  operationId: get_instruction_version_api_v1_agents__agent_id__instruction_versions__version_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/agents/{agent_id}/instruction-versions/{version_id}/revert\n  method: post\n  operationId: revert_instruction_version_api_v1_agents__agent_id__instruction_versions__version_id__revert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/files\n  method: get\n  operationId: list_agent_files_api_v1_agents__agent_id__files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}/files\n  method: post\n  operationId: upload_agent_file_api_v1_agents__agent_id__files_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/files/{filename}\n  method: delete\n  operationId: delete_agent_file_api_v1_agents__agent_id__files__filename__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/triggers\n  method: post\n  operationId: create_trigger_api_v1_agents__agent_id__triggers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/triggers\n\
  \  method: get\n  operationId: list_triggers_api_v1_agents__agent_id__triggers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}/triggers/{trigger_id}\n  method: get\n  operationId: get_trigger_api_v1_agents__agent_id__triggers__trigger_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}/triggers/{trigger_id}\n  method: patch\n  operationId: update_trigger_api_v1_agents__agent_id__triggers__trigger_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/triggers/{trigger_id}\n\
  \  method: delete\n  operationId: delete_trigger_api_v1_agents__agent_id__triggers__trigger_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/triggers/{trigger_id}/enable\n  method: post\n  operationId: enable_trigger_api_v1_agents__agent_id__triggers__trigger_id__enable_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/triggers/{trigger_id}/disable\n  method: post\n  operationId: disable_trigger_api_v1_agents__agent_id__triggers__trigger_id__disable_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/triggers/webhook/{webhook_token}\n  method: post\n  operationId: handle_webhook_api_v1_triggers_webhook__webhook_token__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/test-cases\n  method: get\n  operationId: list_test_cases_api_v1_agents__agent_id__test_cases_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v1/agents/{agent_id}/test-cases\n  method: post\n  operationId: create_test_case_api_v1_agents__agent_id__test_cases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/test-cases/{case_id}\n  method: patch\n  operationId: update_test_case_api_v1_agents__agent_id__test_cases__case_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/test-cases/{case_id}\n  method: delete\n  operationId: delete_test_case_api_v1_agents__agent_id__test_cases__case_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/eval-runs\n  method: post\n  operationId: create_eval_run_api_v1_agents__agent_id__eval_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/eval-runs\n  method: get\n  operationId: list_eval_runs_api_v1_agents__agent_id__eval_runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{agent_id}/eval-runs/{run_id}/cancel\n\
  \  method: post\n  operationId: cancel_eval_run_api_v1_agents__agent_id__eval_runs__run_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{agent_id}/eval-runs/{run_id}\n  method: get\n  operationId: get_eval_run_api_v1_agents__agent_id__eval_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/overview\n  method: get\n  operationId: get_analytics_overview_api_v1_analytics_overview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/me\n  method: get\n  operationId: get_current_user_info_api_v1_auth_me_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations\n  method: post\n  operationId: create_conversation_api_v1_chat_conversations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations\n  method: get\n  operationId: list_conversations_api_v1_chat_conversations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations/builder\n  method: post\n  operationId: get_or_create_builder_conversation_api_v1_chat_conversations_builder_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}\n  method: get\n  operationId: get_conversation_api_v1_chat_conversations__conversation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations/{conversation_id}\n  method: delete\n  operationId: delete_conversation_api_v1_chat_conversations__conversation_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/context\n\
  \  method: get\n  operationId: get_conversation_context_api_v1_chat_conversations__conversation_id__context_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/files\n  method: get\n  operationId: list_chat_files_api_v1_chat_files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/files\n  method: delete\n  operationId: delete_chat_file_api_v1_chat_files_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/files/content\n  method: get\n  operationId: get_chat_file_content_api_v1_chat_files_content_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations/{conversation_id}/stop\n  method: post\n  operationId: stop_conversation_stream_api_v1_chat_conversations__conversation_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/stream\n  method: get\n  operationId: resume_message_stream_api_v1_chat_conversations__conversation_id__stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations/{conversation_id}/turns/{turn_id}/stream\n\
  \  method: get\n  operationId: stream_durable_turn_api_v1_chat_conversations__conversation_id__turns__turn_id__stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/transcribe\n  method: post\n  operationId: transcribe_audio_api_v1_chat_transcribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/messages\n  method: post\n  operationId: send_message_api_v1_chat_conversations__conversation_id__messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/executor-health\n  method: get\n  operationId: chat_executor_health_api_v1_chat_executor_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat/conversations/{conversation_id}/turns\n  method: post\n  operationId: accept_conversation_turn_api_v1_chat_conversations__conversation_id__turns_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/turns\n  method: post\n  operationId: create_conversation_with_turn_api_v1_chat_conversations_turns_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/execute-task\n  method: post\n  operationId: execute_task_api_v1_chat_conversations__conversation_id__execute_task_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/apply-kb-edits\n  method: post\n  operationId: apply_kb_edits_api_v1_chat_conversations__conversation_id__apply_kb_edits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/proposals/{message_id}/accept\n  method: post\n  operationId: accept_proposal_api_v1_chat_conversations__conversation_id__proposals__message_id__accept_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chat/conversations/{conversation_id}/proposals/{message_id}/refuse\n  method: post\n  operationId: refuse_proposal_api_v1_chat_conversations__conversation_id__proposals__message_id__refuse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/debrief/{run_id}\n  method: get\n  operationId: get_debrief_api_v1_debrief__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/debrief/{run_id}/init\n  method: post\n  operationId: init_debrief_api_v1_debrief__run_id__init_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/debrief/{run_id}/message\n  method: post\n  operationId: send_debrief_message_api_v1_debrief__run_id__message_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/debrief/{run_id}/apply-proposal\n  method: post\n  operationId: apply_debrief_proposal_api_v1_debrief__run_id__apply_proposal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me\n  method: get\n  operationId: get_my_organization_api_v1_organizations_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/members\n  method: get\n  operationId:\
  \ list_organization_members_api_v1_organizations_me_members_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/access-control\n  method: get\n  operationId: get_access_control_api_v1_organizations_me_access_control_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/access-control/defaults\n  method: put\n  operationId: update_member_permission_defaults_api_v1_organizations_me_access_control_defaults_put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/organizations/me/access-control/members/{user_id}\n\
  \  method: put\n  operationId: update_member_permission_overrides_api_v1_organizations_me_access_control_members__user_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/organizations/me/access-control/members/{user_id}\n  method: delete\n  operationId: reset_member_permission_overrides_api_v1_organizations_me_access_control_members__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/organizations/me/browser-context-settings\n\
  \  method: patch\n  operationId: update_browser_context_settings_api_v1_organizations_me_browser_context_settings_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/default-start-url\n  method: patch\n  operationId: update_default_start_url_api_v1_organizations_me_default_start_url_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/allowed-domains\n  method: patch\n  operationId: update_allowed_domains_api_v1_organizations_me_allowed_domains_patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/slack-notification-level\n  method: patch\n  operationId: update_slack_notification_level_api_v1_organizations_me_slack_notification_level_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/proxy\n  method: patch\n  operationId: update_proxy_settings_api_v1_organizations_me_proxy_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/residential-proxy\n  method: patch\n  operationId: update_residential_proxy_api_v1_organizations_me_residential_proxy_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/residential-proxy-geolocation\n  method: patch\n  operationId: update_residential_proxy_geolocation_api_v1_organizations_me_residential_proxy_geolocation_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/organizations/me/language\n  method: patch\n  operationId: update_language_api_v1_organizations_me_language_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/flash-mode\n  method: patch\n  operationId: update_flash_mode_api_v1_organizations_me_flash_mode_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/raw-liveview-auth\n  method: patch\n  operationId: update_raw_liveview_auth_enabled_api_v1_organizations_me_raw_liveview_auth_patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/network-recording\n  method: patch\n  operationId: update_network_recording_enabled_api_v1_organizations_me_network_recording_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/auto-create-api\n  method: patch\n  operationId: update_auto_generate_api_api_v1_organizations_me_auto_create_api_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/require-action-confirmation\n  method: patch\n  operationId: update_require_action_confirmation_api_v1_organizations_me_require_action_confirmation_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/execution-settings\n  method: get\n  operationId: get_execution_settings_api_v1_organizations_me_execution_settings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/execution-settings\n  method: patch\n  operationId:\
  \ update_execution_settings_api_v1_organizations_me_execution_settings_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/proxy/test\n  method: post\n  operationId: test_proxy_connection_api_v1_organizations_proxy_test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/api-keys\n  method: post\n  operationId: create_api_key_api_v1_organizations_me_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/api-keys\n  method: get\n  operationId: list_api_keys_api_v1_organizations_me_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/api-keys/{key_id}\n  method: get\n  operationId: get_api_key_api_v1_organizations_me_api_keys__key_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/me/api-keys/{key_id}\n  method: patch\n  operationId: update_api_key_api_v1_organizations_me_api_keys__key_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/me/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_api_v1_organizations_me_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/organizations/me/api-keys/{key_id}/generate-identity-secret\n  metho\n\n# --- truncated at 32 KB (167 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/agentic-access/unisson-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/agentic-access/unisson-agentic-access.yml
summary_line: 478 operations · 272 acting · 28 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Success
- B2B Software
- Implementation
- Automation
- Agents
---
