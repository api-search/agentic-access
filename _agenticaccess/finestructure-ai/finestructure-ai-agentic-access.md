---
acting_count: 262
action_class_counts:
  acting: 262
  connected: 110
api_specs:
- filename: finestructure-ai-bridge-api-openapi.yml
  format: yaml
  label: Fine Structure Bridge API
  slug: finestructure-ai-bridge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-bridge-api-openapi.yml
- filename: finestructure-ai-discovery-api-openapi.yml
  format: yaml
  label: Fine Structure Discovery API
  slug: finestructure-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-discovery-api-openapi.yml
- filename: finestructure-ai-mcp-api-openapi.yml
  format: yaml
  label: Fine Structure MCP API
  slug: finestructure-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-mcp-api-openapi.yml
- filename: finestructure-ai-tools-api-openapi.yml
  format: yaml
  label: Fine Structure Tools API
  slug: finestructure-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-tools-api-openapi.yml
consequence_counts:
  physical: 24
  read: 110
  safety-critical: 10
  write: 228
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Finestructure Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/archive_agent_goal
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/disable_whatsapp_trigger
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/lodging_disconnect_channel_manager
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/lodging_dismiss_calendar_conflict
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/lodging_dismiss_channel_booking
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/lodging_remove_calendar_feed
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/set_contract_reminders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/stop_agent_task
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/stop_voice_campaign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/void_contract
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/configure_email_domain_dns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/create_agent_team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/email_marketing_app_create_event_trigger
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/email_marketing_app_record_event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/email_marketing_configure_sender
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/invite_app_member
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_connect_channel_manager
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_get_attention
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_get_booking_inbox
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_get_guest_messages_settings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_list_balances
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/lodging_sync_channel_manager
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/preview_contract_invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/preview_saved_version
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/publish_creative
operation_count: 372
overview: 'Fine Structure exposes 372 API operations that an AI agent could call, of which 262 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 110 read, 228 write, 24 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fine Structure
provider_slug: finestructure-ai
slug: finestructure-ai-agentic-access
source_filename: finestructure-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/finestructure-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 372\n  by_action_class:\n    acting: 262\n    connected: 110\n  by_consequence:\n    write: 228\n    read: 110\n    physical: 24\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /api/mcp/tools/{tool_name}\n  method: post\n  operationId: call_tool_generic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: post\n  operationId:\
  \ mcp_jsonrpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/manifest\n  method: get\n  operationId: get_manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/health\n  method: get\n  operationId: health_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/create_app\n  method: post\n  operationId: create_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/agency_create_client\n  method: post\n  operationId: agency_create_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/agency_list_clients\n  method: post\n  operationId: agency_list_clients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/agency_create_client_app\n  method: post\n  operationId: agency_create_client_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/agency_create_claim_link\n  method: post\n  operationId: agency_create_claim_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/agency_get_claim_status\n  method: post\n  operationId: agency_get_claim_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_app\n\
  \  method: post\n  operationId: update_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/publish_app\n  method: post\n  operationId: publish_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_platform_guide\n  method: post\n  operationId: get_platform_guide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_recommended_workflow\n  method: post\n  operationId: get_recommended_workflow\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_job_status\n  method: post\n  operationId: get_job_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_app_status\n  method: post\n  operationId: get_app_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_app_links\n  method: post\n  operationId: get_app_links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/list_app_domains\n  method: post\n  operationId: list_app_domains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/set_app_subdomain\n  method: post\n  operationId: set_app_subdomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/check_subdomain_available\n  method: post\n  operationId: check_subdomain_available\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/add_custom_domain\n  method: post\n  operationId: add_custom_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_domain_verification\n  method: post\n  operationId: get_domain_verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/check_domain_verification\n  method: post\n  operationId: check_domain_verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/set_primary_domain\n  method: post\n  operationId: set_primary_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/remove_custom_domain\n  method: post\n  operationId: remove_custom_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_domain_ssl_status\n  method: post\n  operationId: get_domain_ssl_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/configure_domain_redirects\n  method: post\n  operationId: configure_domain_redirects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_apps\n  method: post\n  operationId: list_apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_app_files\n  method: post\n  operationId: get_app_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/read_app_file\n  method: post\n  operationId: read_app_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/mcp/tools/read_app_files\n  method: post\n  operationId: read_app_files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/write_app_file\n  method: post\n  operationId: write_app_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/patch_app_file\n  method: post\n  operationId: patch_app_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/rename_app_file\n  method: post\n  operationId: rename_app_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_app_detail\n  method: post\n  operationId: get_app_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_entities\n  method: post\n  operationId: get_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/query_entity\n  method: post\n  operationId:\
  \ query_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/seed_entity\n  method: post\n  operationId: seed_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_entity_records\n  method: post\n  operationId: create_entity_records\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_entity_record\n  method: post\n  operationId: update_entity_record\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_entity_records\n  method: post\n  operationId: update_entity_records\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/delete_entity_records\n  method: post\n  operationId: delete_entity_records\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/mcp/tools/get_pages\n  method: post\n  operationId: get_pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_errors\n  method: post\n  operationId: get_errors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_app_analytics\n  method: post\n  operationId: get_app_analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_preview_url\n  method: post\n  operationId: get_preview_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/list_saved_versions\n  method: post\n  operationId:\
  \ list_saved_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/restore_saved_version\n  method: post\n  operationId: restore_saved_version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_change_set\n  method: post\n  operationId: create_change_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/add_file_change\n  method: post\n  operationId: add_file_change\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/validate_change_set\n  method: post\n  operationId: validate_change_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/apply_change_set\n  method: post\n  operationId: apply_change_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/mcp/tools/discard_change_set\n  method: post\n  operationId: discard_change_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/validate_app\n  method: post\n  operationId: validate_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/inspect_preview\n  method: post\n  operationId: inspect_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_app_security_context\n  method: post\n  operationId: get_app_security_context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/set_route_policy\n  method: post\n  operationId: set_route_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/set_function_policy\n  method: post\n  operationId: set_function_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/invoke_function\n  method: post\n  operationId: invoke_function\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_platform_request\n  method: post\n  operationId: create_platform_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_platform_request\n  method: post\n  operationId: get_platform_request\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/list_platform_requests\n  method: post\n  operationId: list_platform_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/reply_platform_request\n  method: post\n  operationId: reply_platform_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_platform_request\n  method: post\n  operationId: update_platform_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/set_entity_policy\n  method: post\n  operationId: set_entity_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_app_members\n  method: post\n  operationId: list_app_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/invite_app_member\n  method: post\n  operationId: invite_app_member\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_app_member_role\n  method: post\n  operationId: update_app_member_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/remove_app_member\n  method: post\n  operationId: remove_app_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/block_app_member\n  method: post\n  operationId: block_app_member\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/unblock_app_member\n  method: post\n  operationId: unblock_app_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/verify_app_member\n  method: post\n  operationId: verify_app_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/mcp/tools/get_app_security_audit\n  method: post\n  operationId: get_app_security_audit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/compare_saved_versions\n  method: post\n  operationId: compare_saved_versions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/compare_current_to_version\n  method: post\n  operationId: compare_current_to_version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/mcp/tools/restore_file_from_version\n  method: post\n  operationId: restore_file_from_version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_entity_schema\n  method: post\n  operationId: create_entity_schema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_entity_schema\n  method: post\n  operationId: update_entity_schema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/validate_entity_relationships\n  method: post\n  operationId: validate_entity_relationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_entity_metadata\n  method: post\n  operationId: update_entity_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_secret_keys\n  method: post\n  operationId: list_secret_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/set_secret\n  method: post\n  operationId: set_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/delete_secret\n  method: post\n  operationId: delete_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp/tools/list_integrations\n  method: post\n  operationId: list_integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/configure_integration\n  method: post\n  operationId: configure_integration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_ab_tests\n  method: post\n  operationId: list_ab_tests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/create_ab_test\n  method: post\n  operationId: create_ab_test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_ab_test\n  method: post\n  operationId: update_ab_test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/delete_ab_test\n  method: post\n  operationId: delete_ab_test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/get_ab_test_stats\n  method: post\n  operationId:\
  \ get_ab_test_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/email_marketing_status\n  method: post\n  operationId: email_marketing_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_configure_sender\n  method: post\n  operationId: email_marketing_configure_sender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp/tools/email_marketing_update_template\n  method: post\n  operationId: email_marketing_update_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_create_broadcast\n  method: post\n  operationId: email_marketing_create_broadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_create_sequence\n  method: post\n  operationId: email_marketing_create_sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_create_variable_trigger\n  method: post\n  operationId: email_marketing_create_variable_trigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_trigger_variable\n  method: post\n  operationId: email_marketing_trigger_variable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp/tools/email_marketing_app_status\n  method: post\n  operationId: email_marketing_app_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/email_marketing_app_configure\n  method: post\n  operationId: email_marketing_app_configure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (120 KB total) ---\n# Full source: https://artifacts.apis.io/finestructure-ai/agentic-access/finestructure-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/finestructure-ai/agentic-access/finestructure-ai-agentic-access.yml
summary_line: 372 operations · 262 acting · 10 human-in-the-loop
tags:
- AI
- Automation
- Platform
- Integration
- Business
---
