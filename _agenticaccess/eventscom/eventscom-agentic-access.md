---
acting_count: 598
action_class_counts:
  acting: 598
  connected: 381
api_specs:
- filename: eventscom-datagol-platform-openapi.yml
  format: yaml
  label: DataGol Platform API (Saasxl)
  slug: datagol-platform-api-saasxl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventscom/refs/heads/main/openapi/eventscom-datagol-platform-openapi.yml
- filename: eventscom-datagol-ai-openapi.yml
  format: yaml
  label: DataGol AI API
  slug: datagol-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventscom/refs/heads/main/openapi/eventscom-datagol-ai-openapi.yml
- filename: eventscom-datagol-python-agent-openapi.yml
  format: yaml
  label: DataGol Python Agent API
  slug: datagol-python-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventscom/refs/heads/main/openapi/eventscom-datagol-python-agent-openapi.yml
consequence_counts:
  physical: 16
  read: 381
  safety-critical: 291
  write: 291
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 291
kind: agentic-access
layout: agentic-access
method: generated
name: Eventscom Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/api/v1/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/api/v1/config/migration/agentSettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agents/api/v1/config/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agents/api/v1/config/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/api/v1/templates
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agents/api/v1/templates/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agents/api/v1/templates/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ai/api/v2/conversations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/conversations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/conversations/migratePermissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai/api/v2/conversations/{conversationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/dataSourceTables/embeddings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/dataSourceTables/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/demos/document-validation/controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/home-chat-agent/vector-store/reset-workspace
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/messages/{conversation_id}/{message_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/api/v2/python-agent/{conversation_id}/{message_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alerts/api/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /alerts/api/v1/{alertId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /alerts/api/v1/{alertId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alerts/api/v1/{alertId}/activate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alerts/api/v1/{alertId}/deactivate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/test/workflow/api-post/cancel/{requestId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/test/workflow/api-post/dummy-endpoint
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/test/workflow/api-post/dummy-endpoint
operation_count: 979
overview: 'Events.com exposes 979 API operations that an AI agent could call, of which 598 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 381 read, 291 write, 16 physical, and 291 safety-critical.


  291 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Events.com
provider_slug: eventscom
slug: eventscom-agentic-access
source_filename: eventscom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/eventscom-datagol-ai-openapi.yml, openapi/eventscom-datagol-platform-openapi.yml,\n  openapi/eventscom-datagol-python-agent-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 979\n  by_action_class:\n    connected: 381\n    acting: 598\n  by_consequence:\n    read: 381\n    write: 291\n    physical: 16\n    safety-critical: 291\n  human_in_the_loop_required: 291\noperations:\n- path: /ai/api/v2/health-check\n  method: get\n  operationId: health_check_ai_api_v2_health_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/sqlParser/dataSources\n  method: post\n\
  \  operationId: sql_parser_data_source_ai_api_v2_sqlParser_dataSources_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/sqlParser/columns\n  method: post\n  operationId: sql_parser_columns_ai_api_v2_sqlParser_columns_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/sqlParser/links\n  method: post\n  operationId: sql_parser_relationships_ai_api_v2_sqlParser_links_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/sqlParser/subQueries\n  method: post\n  operationId: sql_parser_relationships_ai_api_v2_sqlParser_subQueries_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/sqlParser/removeComments\n  method: post\n  operationId: remove_comments_ai_api_v2_sqlParser_removeComments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/sqlParser/changeDialect\n  method: post\n  operationId: change_dialect_ai_api_v2_sqlParser_changeDialect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations\n  method: post\n  operationId: create_conversation_ai_api_v2_conversations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations\n  method: get\n  operationId: get_all_conversations_by_user_element_ai_api_v2_conversations_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/conversations\n  method: put\n  operationId: update_conversation_ai_api_v2_conversations_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations/{conversation_id}\n  method: get\n  operationId: get_conversation_by_id_ai_api_v2_conversations__conversation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/conversations/{conversation_id}\n  method: delete\n  operationId: delete_ai_api_v2_conversations__conversation_id__delete\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations/{conversation_id}/messages\n  method: get\n  operationId: get_messages_by_conversation_id_ai_api_v2_conversations__conversation_id__messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/conversations/{conversation_id}/messages/{message_id}\n  method: put\n  operationId: update_message_by_conid_and_msgid_ai_api_v2_conversations__conversation_id__messages__message_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations/{conversation_id}/messages/{message_id}\n  method: delete\n  operationId: delete_message_by_conid_and_msgid_ai_api_v2_conversations__conversation_id__messages__message_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/conversations/messages/pinned\n  method: get\n  operationId: get_pinned_messages_by_user_id_ai_api_v2_conversations_messages_pinned_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/messages/complete\n  method: post\n  operationId: post_completion_generic_ai_api_v2_messages_complete_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/messages\n  method: post\n  operationId: send_message_to_agent_ai_api_v2_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/messages/{conversation_id}/{message_id}/stop\n  method: post\n  operationId: stop_streaming_agent_run_ai_api_v2_messages__conversation_id___message_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/api/v2/messages/streaming\n  method: post\n  operationId: send_message_to_streaming_agent_ai_api_v2_messages_streaming_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/messages/streaming/{conversation_id}/{message_id}\n  method: get\n  operationId: stream_message_events_ai_api_v2_messages_streaming__conversation_id___message_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /ai/api/v2/runs/active\n  method: get\n  operationId: list_active_runs_ai_api_v2_runs_active_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/mcp/tools\n  method: post\n  operationId: list_mcp_tools_ai_api_v2_mcp_tools_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ai-generate/internal/completion\n  method: post\n  operationId: ai_generate_internal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ai/api/v2/ai-generate/internal/databar/get-enrichments\n  method: get\n  operationId: get_databar_enrichment_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/ai-generate/internal/databar/run-enrichment\n  method: post\n  operationId: run_databar_enrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v1/builder/chat/complete\n  method: post\n  operationId: chat_completion_ai_api_v1_builder_chat_complete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v1/builder/chat/complete/stream\n  method: post\n  operationId: chat_completion_stream_ai_api_v1_builder_chat_complete_stream_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/dashboard/generate-dashboard\n  method: post\n  operationId: generate_dashboard_ai_api_v2_dashboard_generate_dashboard_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/dashboard/widget/summary\n  method: post\n  operationId: generate_summary_ai_api_v2_dashboard_widget_summary_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/dashboard/summary\n  method: post\n  operationId: generate_dashboard_summary_ai_api_v2_dashboard_summary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/run\n  method: post\n  operationId: run_ai_api_v2_home_chat_agent_run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/update-message\n  method: put\n  operationId: update_message_ai_api_v2_home_chat_agent_update_message_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/delete-messages\n  method: post\n  operationId: delete_chat_message_ai_api_v2_home_chat_agent_delete_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/conversations\n  method: get\n  operationId:\
  \ get_conversations_ai_api_v2_home_chat_agent_conversations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/home-chat-agent/conversations\n  method: post\n  operationId: create_conversation_ai_api_v2_home_chat_agent_conversations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/conversations/{thread_id}/name\n  method: put\n  operationId: update_conversation_name_ai_api_v2_home_chat_agent_conversations__thread_id__name_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/conversations/{thread_id}\n  method: delete\n  operationId: delete_conversation_ai_api_v2_home_chat_agent_conversations__thread_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/state/{thread_id}\n  method: get\n  operationId: get_conversation_state_ai_api_v2_home_chat_agent_state__thread_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/home-chat-agent/vector-store/sync-workspace\n  method: post\n  operationId: vector_store_sync_workspace_ai_api_v2_home_chat_agent_vector_store_sync_workspace_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/vector-store/reset-workspace\n  method: post\n  operationId: vector_store_reset_workspace_ai_api_v2_home_chat_agent_vector_store_reset_workspace_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/api/v2/home-chat-agent/vector-store/advanced-search-resources\n  method: post\n  operationId: vector_store_advanced_search_resources_ai_api_v2_home_chat_agent_vector_store_advanced_search_resources_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/home-chat-agent/hello-world\n  method: post\n  operationId: hello_world_ai_api_v2_home_chat_agent_hello_world_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models\n  method: post\n  operationId: create_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models\n  method: get\n  operationId: get_models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}\n  method: get\n  operationId: get_model\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}\n  method: put\n  operationId: update_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}\n\
  \  method: delete\n  operationId: delete_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ml/dashboard/models/config\n  method: get\n  operationId: get_model_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}/train\n  method: post\n  operationId: train_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}/history\n\
  \  method: get\n  operationId: model_training_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/ml/dashboard/{elementType}/{elementId}/models/{modelId}/predict\n  method: post\n  operationId: predict_using_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/feedback\n  method: post\n  operationId: post_message_feedback_ai_api_v2_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /ai/api/v2/research\n  method: post\n  operationId: research_ai_api_v2_research_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/research/download\n  method: post\n  operationId: download_pdf_ai_api_v2_research_download_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/global-id/execute\n  method: post\n  operationId: execute_global_id_algorithm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/jira/schema\n  method: get\n  operationId: get_jira_schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/jira/issues/create\n  method: post\n  operationId: create_issue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/execute\n  method: post\n  operationId: execute_data_extraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/execute-file-upload\n  method: post\n  operationId: execute_data_extraction_file_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/schema/generate\n  method: post\n  operationId: generate_data_extraction_schema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/schema/generate-from-content\n  method: post\n  operationId: generate_data_extraction_schema_from_content\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/advanced/execute\n  method: post\n  operationId: run_data_extraction_test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/extract-data/advanced/execute-file-upload\n  method: post\n  operationId: run_data_extraction_test_file_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/knowledge-graph/status\n  method: get\n  operationId: get_knowledge_graph_status_ai_api_v2_knowledge_graph_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/knowledge-graph\n  method: get\n  operationId: get_knowledge_graph_ai_api_v2_knowledge_graph_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/bi-rag/index-page\n  method: post\n  operationId: index_page_ai_api_v2_bi_rag_index_page_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /ai/api/v2/bi-rag/index-workspace\n  method: post\n  operationId: index_workspace_ai_api_v2_bi_rag_index_workspace_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/bi-rag/add-widget\n  method: post\n  operationId: add_widget_ai_api_v2_bi_rag_add_widget_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/bi-rag/remove-widget\n  method: delete\n  operationId: remove_indexed_widget_ai_api_v2_bi_rag_remove_widget_delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/bi-rag/update-widget\n  method: post\n  operationId: update_indexed_widget_ai_api_v2_bi_rag_update_widget_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/bi-rag/delete-all-widgets\n  method: post\n  operationId: delete_all_widgets_ai_api_v2_bi_rag_delete_all_widgets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /ai/api/v2/python-agent/query\n  method: post\n  operationId: query_agent_ai_api_v2_python_agent_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/python-agent/submit-feedback\n  method: post\n  operationId: submit_feedback_ai_api_v2_python_agent_submit_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/python-agent/session/{session_id}/status\n  method: get\n  operationId: get_session_status_ai_api_v2_python_agent_session__session_id__status_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/python-agent/session/{session_id}\n  method: delete\n  operationId: cleanup_session_ai_api_v2_python_agent_session__session_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/{agent_type}/download-data\n  method: post\n  operationId: download_agent_data_ai_api_v2__agent_type__download_data_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /ai/api/v2/demos/document-validation/validate\n  method: post\n  operationId: validate_documents_ai_api_v2_demos_document_validation_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/demos/document-validation/controls\n  method: post\n  operationId: generate_controls_ai_api_v2_demos_document_validation_controls_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/api/v2/dataSourceTables/search\n  method: post\n  operationId: search_tables_ai_api_v2_dataSourceTables_search_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/api/v2/dataSourceTables/embeddings\n  method: post\n  operationId: create_embeddings_ai_api_v2_dataSourceTables_embeddings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/api/v2/internal/{auth_token}/conversation/check-access\n  method: get\n  operationId: check_conversation_access_ai_api_v2_internal__auth_token__conversation_check_access_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/internal/{auth_token}/conversation/thread-details\n  method: get\n  operationId: get_conversation_details_ai_api_v2_internal__auth_token__conversation_thread_details_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/internal/{auth_token}/file-search/create-store\n  method: post\n  operationId: create_file_search_store_ai_api_v2_internal__auth_token__file_search_create_store_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/api/v2/internal/{auth_token}/agent/by-thread\n  method: get\n  operationId: get_custom_agent_for_thread_ai_api_v2_internal__auth_token__agent_by_thread_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/internal/{auth_token}/message/status\n  method: get\n  operationId: get_message_status_ai_api_v2_internal__auth_token__message_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/api/v2/file-search/store\n  method: post\n  operationId: store_file_ai_api_v2_file_search_store_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max\n\n# --- truncated at 32 KB (316 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/eventscom/refs/heads/main/agentic-access/eventscom-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventscom/refs/heads/main/agentic-access/eventscom-agentic-access.yml
summary_line: 979 operations · 598 acting · 291 human-in-the-loop
tags:
- event-management
- ticketing
- event-registration
- event-marketing
- sponsorship
- event-discovery
- data-platform
- business-intelligence
- artificial-intelligence
- mcp
- agent-native
- no-code
---
