---
acting_count: 512
action_class_counts:
  acting: 512
  connected: 398
api_specs:
- filename: opply-openapi-original.yml
  format: yaml
  label: Opply API
  slug: opply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/openapi/opply-openapi-original.yml
consequence_counts:
  physical: 127
  read: 398
  safety-critical: 18
  write: 367
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Opply Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/app-orders/merchant-of-record/{uuid}/mark-dispatch-scheduled/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/app-orders/merchant-of-record/{uuid}/mark-order-dispatched/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/app-orders/supplier/{uuid}/mark-order-dispatched/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/buyer-onboarding/merchant-of-record/supplier-submissions/{id}/reset/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/files/attachments/{uuid}/confirm/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/files/message-attachments/{uuid}/confirm/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/inquiries/dispatch_address/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/inquiries/dispatch_address/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/orders/supplier/{order_uuid}/confirm-dispatch/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/task-recurrences/{uuid}/disable/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/users/admin_panel/users/{uuid}/reset_password/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/users/reset-password/commit/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/users/reset-password/init/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/users/users/set-admin/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/notifications/company-overrides/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2/notifications/company-overrides/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/notifications/company-overrides/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/notifications/debug-dispatch/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/agents/unleashed-invoice-assistant/invocations/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/agents/xero-invoice-assistant/invocations/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/agreements/brand/{uuid}/place-order/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/agreements/merchant-of-record/{uuid}/place-order/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/app-orders/admin/{uuid}/create-order-event/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/app-orders/admin/{uuid}/documents/{document_uuid}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/app-orders/admin/{uuid}/edit/
operation_count: 910
overview: 'Opply exposes 910 API operations that an AI agent could call, of which 512 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 398 read, 367 write, 127 physical, and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Opply
provider_slug: opply
slug: opply-agentic-access
source_filename: opply-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/opply-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 910\n  by_action_class:\n    connected: 398\n    acting: 512\n  by_consequence:\n    read: 398\n    write: 367\n    physical: 127\n    safety-critical: 18\n  human_in_the_loop_required: 18\noperations:\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: .well_known_oauth_authorization_server_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: .well_known_oauth_protected_resource_retrieve\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/api/v1/mcp/zendesk\n  method: get\n  operationId: .well_known_oauth_protected_resource_api_v1_mcp_zendesk_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/schema/\n  method: get\n  operationId: api_schema_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity-feed/\n  method: get\n  operationId: api_v1_activity_feed_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity-feed/{uuid}/\n  method: get\n  operationId: api_v1_activity_feed_retrieve\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity-feed/mark-read/\n  method: post\n  operationId: api_v1_activity_feed_mark_read_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/activity-feed/unread-count/\n  method: get\n  operationId: api_v1_activity_feed_unread_count_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/admin/installations/\n  method: get\n  operationId: api_v1_agents_admin_installations_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/admin/installations/{agent_uuid}/\n  method: patch\n  operationId: api_v1_agents_admin_installations_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/agent-task-runs/{run_uuid}/claim/\n  method: post\n  operationId: api_v1_agents_agent_task_runs_claim_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/agent-task-runs/{run_uuid}/complete/\n  method: post\n  operationId: api_v1_agents_agent_task_runs_complete_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/agent-task-runs/{run_uuid}/heartbeat/\n  method: post\n  operationId: api_v1_agents_agent_task_runs_heartbeat_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/buyer-onboarding/invocations/\n  method: post\n  operationId: api_v1_agents_buyer_onboarding_invocations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/debug/system-tasks/\n  method: get\n  operationId: api_v1_agents_debug_system_tasks_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/feedback/\n  method: post\n  operationId: api_v1_agents_feedback_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/fleet/\n  method: get\n  operationId: api_v1_agents_fleet_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/fleet/{slug}/\n\
  \  method: get\n  operationId: api_v1_agents_fleet_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/installations/me/\n  method: get\n  operationId: api_v1_agents_installations_me_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/mor-router/me/\n  method: get\n  operationId: api_v1_agents_mor_router_me_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/opply-assistant/invocations/\n  method: post\n  operationId: api_v1_agents_opply_assistant_invocations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/opply-assistant/sessions/me/\n  method: get\n  operationId: api_v1_agents_opply_assistant_sessions_me_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/opply-assistant/sessions/me/\n  method: delete\n  operationId: api_v1_agents_opply_assistant_sessions_me_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/opply-assistant/sessions/me/events/\n  method: get\n  operationId: api_v1_agents_opply_assistant_sessions_me_events_retrieve\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/unleashed-invoice-assistant/invocations/\n  method: post\n  operationId: api_v1_agents_unleashed_invoice_assistant_invocations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/xero-invoice-assistant/invocations/\n  method: post\n  operationId: api_v1_agents_xero_invoice_assistant_invocations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/brand/\n  method: get\n  operationId: api_v1_agreements_brand_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/brand/{uuid}/\n  method: get\n  operationId: api_v1_agreements_brand_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/brand/{uuid}/place-order/\n  method: post\n  operationId: api_v1_agreements_brand_place_order_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/agreements/brand/aggregate/\n  method: get\n  operationId: api_v1_agreements_brand_aggregate_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/lead-generation-jobs/\n  method: get\n  operationId: api_v1_agreements_lead_generation_jobs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/lead-generation-jobs/\n  method: post\n  operationId: api_v1_agreements_lead_generation_jobs_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/\n\
  \  method: get\n  operationId: api_v1_agreements_merchant_of_record_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/merchant-of-record/\n  method: post\n  operationId: api_v1_agreements_merchant_of_record_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/\n  method: get\n  operationId: api_v1_agreements_merchant_of_record_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/merchant-of-record/{uuid}/\n  method: put\n  operationId: api_v1_agreements_merchant_of_record_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/\n  method: patch\n  operationId: api_v1_agreements_merchant_of_record_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/\n  method: delete\n  operationId: api_v1_agreements_merchant_of_record_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/line-item/{line_item_uuid}/documents/\n  method: post\n  operationId: api_v1_agreements_merchant_of_record_line_item_documents_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/line-item/{line_item_uuid}/documents/{document_uuid}/\n  method: delete\n  operationId: api_v1_agreements_merchant_of_record_line_item_documents_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/agreements/merchant-of-record/{uuid}/orders/\n  method: get\n  operationId: api_v1_agreements_merchant_of_record_orders_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agreements/merchant-of-record/{uuid}/place-order/\n  method: post\n  operationId: api_v1_agreements_merchant_of_record_place_order_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/\n  method: get\n  operationId: api_v1_app_orders_admin_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/admin/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_admin_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/admin/{uuid}/create-order-event/\n  method: post\n  operationId: api_v1_app_orders_admin_create_order_event_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/{uuid}/documents/\n  method: get\n  operationId: api_v1_app_orders_admin_documents_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/admin/{uuid}/documents/{document_uuid}/\n  method: delete\n  operationId: api_v1_app_orders_admin_documents_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/{uuid}/edit/\n  method: put\n  operationId: api_v1_app_orders_admin_edit_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/{uuid}/mark-order-as-paid/\n\
  \  method: post\n  operationId: api_v1_app_orders_admin_mark_order_as_paid_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/{uuid}/mark-order-as-paid-out-to-supplier/\n  method: post\n  operationId: api_v1_app_orders_admin_mark_order_as_paid_out_to_supplier_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/admin/{uuid}/order-events/\n  method: get\n  operationId:\
  \ api_v1_app_orders_admin_order_events_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/admin/{uuid}/pricing/\n  method: get\n  operationId: api_v1_app_orders_admin_pricing_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/admin/{uuid}/upload-document/\n  method: post\n  operationId: api_v1_app_orders_admin_upload_document_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/alerts/\n  method: get\n  operationId: api_v1_app_orders_alerts_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/\n  method: get\n  operationId: api_v1_app_orders_brand_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_brand_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/{uuid}/client-notified-as-paid/\n  method: post\n  operationId: api_v1_app_orders_brand_client_notified_as_paid_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/{uuid}/invoice-url/\n  method: get\n  operationId: api_v1_app_orders_brand_invoice_url_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/{uuid}/mark-as-delivered/\n  method: post\n  operationId: api_v1_app_orders_brand_mark_as_delivered_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/{uuid}/mark-as-picked-up/\n  method: post\n  operationId: api_v1_app_orders_brand_mark_as_picked_up_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/{uuid}/order-activities/\n  method: get\n  operationId: api_v1_app_orders_brand_order_activities_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/{uuid}/purchase-order/pdf/\n  method: get\n  operationId: api_v1_app_orders_brand_purchase_order_pdf_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/{uuid}/repeat-spot-order/\n  method: post\n  operationId: api_v1_app_orders_brand_repeat_spot_order_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/activity-statement/\n  method: get\n  operationId: api_v1_app_orders_brand_activity_statement_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/aggregate/\n  method: get\n  operationId: api_v1_app_orders_brand_aggregate_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/all-order-activities/\n  method: get\n  operationId: api_v1_app_orders_brand_all_order_activities_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/grouped-statements/\n  method: get\n  operationId: api_v1_app_orders_brand_grouped_statements_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/grouped-statements/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_brand_grouped_statements_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/grouped-statements/{uuid}/csv/\n  method: get\n  operationId: api_v1_app_orders_brand_grouped_statements_csv_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /api/v1/app-orders/brand/grouped-statements/{uuid}/invoices/\n  method: get\n  operationId: api_v1_app_orders_brand_grouped_statements_invoices_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/grouped-statements/{uuid}/mark-transfer-sent/\n  method: post\n  operationId: api_v1_app_orders_brand_grouped_statements_mark_transfer_sent_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/order-adjustments/\n  method: get\n  operationId: api_v1_app_orders_brand_order_adjustments_list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/order-adjustments/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_brand_order_adjustments_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/outstanding-payments-summary/\n  method: get\n  operationId: api_v1_app_orders_brand_outstanding_payments_summary_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/payment-analytics/\n  method: get\n  operationId: api_v1_app_orders_brand_payment_analytics_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/payments/\n\
  \  method: get\n  operationId: api_v1_app_orders_brand_payments_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/payments/available-sections/\n  method: get\n  operationId: api_v1_app_orders_brand_payments_available_sections_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/payments/merchant-of-record/\n  method: get\n  operationId: api_v1_app_orders_brand_payments_merchant_of_record_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/payments/service-fees/\n  method: get\n  operationId: api_v1_app_orders_brand_payments_service_fees_retrieve\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/spot-buy-request/\n  method: post\n  operationId: api_v1_app_orders_brand_spot_buy_request_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/spot-buy-requests/\n  method: get\n  operationId: api_v1_app_orders_brand_spot_buy_requests_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/spot-buy-requests/{spot_buy_request_uuid}/cancel/\n  method: patch\n  operationId: api_v1_app_orders_brand_spot_buy_requests_cancel_partial_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/statements/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_brand_statements_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/statements/{uuid}/client-notified-as-paid/\n  method: post\n  operationId: api_v1_app_orders_brand_statements_client_notified_as_paid_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/brand/statements/{uuid}/invoice-pdf/\n  method: get\n  operationId: api_v1_app_orders_brand_statements_invoice_pdf_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/statements/{uuid}/invoice-url/\n  method: get\n  operationId: api_v1_app_orders_brand_statements_invoice_url_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/suppliers/\n  method: get\n  operationId: api_v1_app_orders_brand_suppliers_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/brand/two-credit-information/\n\
  \  method: get\n  operationId: api_v1_app_orders_brand_two_credit_information_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/forecasts/\n  method: get\n  operationId: api_v1_app_orders_forecasts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/merchant-of-record/\n  method: get\n  operationId: api_v1_app_orders_merchant_of_record_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/\n  method: get\n  operationId: api_v1_app_orders_merchant_of_record_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/approve/\n  method: post\n  operationId: api_v1_app_orders_merchant_of_record_approve_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/buyer-purchase-order/pdf/\n  method: get\n  operationId: api_v1_app_orders_merchant_of_record_buyer_purchase_order_pdf_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/change-payment-terms/\n  method: post\n  operationId: api_v1_app_orders_merchant_of_record_change_payment_terms_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/confirm-shipping-responsibility/\n  method: post\n  operationId: api_v1_app_orders_merchant_of_record_confirm_shipping_responsibility_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/create-order-event/\n  method: post\n  operationId: api_v1_app_orders_merchant_of_record_create_order_event_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-orders/merchant-of-record/{uuid}/documents/\n  method: get\n  operationId: api_v1_app_orders_merchant_of_record_documents_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app-orders/merchant-of-record/\n\n# --- truncated at 32 KB (311 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/agentic-access/opply-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/agentic-access/opply-agentic-access.yml
summary_line: 910 operations · 512 acting · 18 human-in-the-loop
tags:
- Company
- Food and Beverage
- Supply Chain
- Procurement
- Ordering
- Payments
- Sourcing
- Logistics
- AI Agents
- MCP
---
