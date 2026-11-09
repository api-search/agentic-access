---
acting_count: 65
action_class_counts:
  acting: 65
  connected: 76
api_specs:
- filename: logbrew-account-api-openapi.yml
  format: yaml
  label: LogBrew Account API
  slug: logbrew-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-account-api-openapi.yml
- filename: logbrew-actions-api-openapi.yml
  format: yaml
  label: LogBrew Actions API
  slug: logbrew-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-actions-api-openapi.yml
- filename: logbrew-alerts-api-openapi.yml
  format: yaml
  label: LogBrew Alerts API
  slug: logbrew-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-alerts-api-openapi.yml
- filename: logbrew-billing-api-openapi.yml
  format: yaml
  label: LogBrew Billing API
  slug: logbrew-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-billing-api-openapi.yml
- filename: logbrew-connected-clients-api-openapi.yml
  format: yaml
  label: LogBrew Connected clients API
  slug: logbrew-connected-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-connected-clients-api-openapi.yml
- filename: logbrew-debug-files-api-openapi.yml
  format: yaml
  label: LogBrew Debug files API
  slug: logbrew-debug-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-debug-files-api-openapi.yml
- filename: logbrew-ingestion-api-openapi.yml
  format: yaml
  label: LogBrew Ingestion API
  slug: logbrew-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-ingestion-api-openapi.yml
- filename: logbrew-issues-api-openapi.yml
  format: yaml
  label: LogBrew Issues API
  slug: logbrew-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-issues-api-openapi.yml
- filename: logbrew-live-feed-api-openapi.yml
  format: yaml
  label: LogBrew Live feed API
  slug: logbrew-live-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-live-feed-api-openapi.yml
- filename: logbrew-logs-api-openapi.yml
  format: yaml
  label: LogBrew Logs API
  slug: logbrew-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-logs-api-openapi.yml
- filename: logbrew-metrics-api-openapi.yml
  format: yaml
  label: LogBrew Metrics API
  slug: logbrew-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-metrics-api-openapi.yml
- filename: logbrew-organizations-api-openapi.yml
  format: yaml
  label: LogBrew Organizations API
  slug: logbrew-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-organizations-api-openapi.yml
- filename: logbrew-product-analytics-api-openapi.yml
  format: yaml
  label: LogBrew Product analytics API
  slug: logbrew-product-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-product-analytics-api-openapi.yml
- filename: logbrew-projects-api-openapi.yml
  format: yaml
  label: LogBrew Projects API
  slug: logbrew-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-projects-api-openapi.yml
- filename: logbrew-releases-api-openapi.yml
  format: yaml
  label: LogBrew Releases API
  slug: logbrew-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-releases-api-openapi.yml
- filename: logbrew-support-api-openapi.yml
  format: yaml
  label: LogBrew Support API
  slug: logbrew-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-support-api-openapi.yml
- filename: logbrew-traces-api-openapi.yml
  format: yaml
  label: LogBrew Traces API
  slug: logbrew-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-traces-api-openapi.yml
- filename: logbrew-volume-api-openapi.yml
  format: yaml
  label: LogBrew Volume API
  slug: logbrew-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logbrew/openapi/logbrew-volume-api-openapi.yml
consequence_counts:
  physical: 10
  read: 76
  safety-critical: 6
  write: 49
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Logbrew Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/devices/{device_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/mcp/grants/{grant_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/organizations/{organization_id}/invitations/{invitation_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/organizations/{organization_id}/projects/{project_id}/members/{member_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/projects/{project_id}/ingest-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/portal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/native-debug-artifact-uploads
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/projects/{project_id}/test-event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/projects/{project_id}/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/projects/{project_id}/webhooks/{webhook_id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/telemetry/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/telemetry/ingest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/telemetry/issues/ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/events
operation_count: 141
overview: 'LogBrew exposes 141 API operations that an AI agent could call, of which 65 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 76 read, 49 write, 10 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LogBrew
provider_slug: logbrew
slug: logbrew-agentic-access
source_filename: logbrew-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/logbrew-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 141\n  by_action_class:\n    connected: 76\n    acting: 65\n  by_consequence:\n    read: 76\n    write: 49\n    safety-critical: 6\n    physical: 10\n  human_in_the_loop_required: 6\noperations:\n- path: /api/account/invitations\n  method: get\n  operationId: list_my_invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/subscription\n  method: get\n  operationId: get_subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/account/usage\n  method: get\n  operationId: get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/usage/history\n  method: get\n  operationId: get_usage_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/account\n  method: delete\n  operationId: delete_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/account\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/account\n  method: patch\n  operationId: update_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: sign_out\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/logout-all\n  method: post\n  operationId: sign_out_everywhere\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/read-key\n  method: get\n  operationId: get_read_key_scope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/refresh\n  method: post\n  operationId: refresh_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/restore\n  method: post\n  operationId: restore_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/catalog\n  method: get\n  operationId: get_billing_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/checkout\n  method: post\n  operationId: create_checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/overview\n  method: get\n  operationId: get_billing_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/portal\n  method: post\n\
  \  operationId: open_billing_portal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/devices\n  method: post\n  operationId: register_device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/devices/{device_id}\n  method: delete\n  operationId: unregister_device\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/feed/live\n  method: get\n  operationId: open_live_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed/ticket\n  method: post\n  operationId: create_live_feed_ticket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logs\n  method: get\n  operationId: list_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logs/attributes\n  method: get\n  operationId: list_log_attributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/logs/usage\n  method: get\n  operationId: get_log_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logs/{log_id}\n  method: get\n  operationId: get_log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logs/{log_id}/investigation\n  method: get\n  operationId: investigate_log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logs/{log_id}/triage-rule\n  method: put\n  operationId: set_log_triage_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/grants\n  method: get\n  operationId: list_connected_clients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/grants/{grant_id}\n  method: delete\n  operationId: disconnect_client\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/native-debug-artifact-uploads\n  method: post\n  operationId: start_debug_file_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - artifact\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/native-debug-artifact-uploads/{session_id}/chunks/{chunk_sha256}\n  method: put\n  operationId: upload_debug_file_chunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - artifact\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/native-debug-artifact-uploads/{session_id}/complete\n  method: post\n  operationId: complete_debug_file_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - artifact\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/native-debug-artifacts\n  method: get\n  operationId: find_debug_file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/preferences\n  method: get\n  operationId: get_notification_preferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/preferences\n  method: put\n  operationId: update_notification_preferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications/preferences/projects/{project_id}\n  method: delete\n  operationId: clear_project_alerts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications/preferences/projects/{project_id}\n  method: put\n  operationId: set_project_alerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations\n  method: get\n  operationId: list_organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations\n  method: post\n  operationId: create_organization\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}\n  method: get\n  operationId: get_organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/invitations\n  method: get\n  operationId: list_organization_invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/invitations\n  method: post\n  operationId: invite_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/invitations/{invitation_id}\n  method: delete\n  operationId: revoke_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/invitations/{invitation_id}\n  method: get\n  operationId: get_invitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/invitations/{invitation_id}/accept\n  method: post\n  operationId: accept_invitation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/members\n  method: get\n  operationId: list_organization_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/members/{member_id}/role\n  method: patch\n  operationId: change_member_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/project-roles\n  method: get\n  operationId: list_project_roles\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/project-roles\n  method: post\n  operationId: create_project_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/project-roles/{role_id}\n  method: delete\n  operationId: delete_project_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/project-roles/{role_id}\n\
  \  method: patch\n  operationId: update_project_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/projects/{project_id}/members\n  method: get\n  operationId: list_project_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/projects/{project_id}/members/{member_id}\n  method: delete\n  operationId: revoke_project_access\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/projects/{project_id}/members/{member_id}\n  method: put\n  operationId: grant_project_access\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/teams\n  method: get\n  operationId: list_teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/teams\n  method: post\n  operationId: create_team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/teams/{team_id}\n  method: delete\n  operationId: delete_team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/teams/{team_id}/members/{member_id}\n  method: delete\n  operationId: remove_team_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/teams/{team_id}/members/{member_id}\n  method: put\n  operationId: add_team_member\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects\n  method: get\n  operationId: list_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: post\n  operationId: create_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/archived\n  method: get\n  operationId: list_archived_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/repositories\n  method: get\n  operationId: list_repositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/repositories/components/discover\n  method: post\n  operationId: discover_components\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}\n  method: delete\n  operationId: archive_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}\n  method: patch\n  operationId: rename_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/alert-rules\n  method: get\n  operationId: list_alert_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/alert-rules\n  method: post\n  operationId: create_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/projects/{project_id}/alert-rules/{rule_id}\n  method: delete\n  operationId: delete_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/alert-rules/{rule_id}\n  method: get\n  operationId: get_alert_rule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/alert-rules/{rule_id}\n  method: patch\n  operationId: update_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/projects/{project_id}/components\n  method: get\n  operationId: get_project_components\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/doctor\n  method: get\n  operationId: check_project_setup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/inbound-filters\n  method: get\n  operationId: get_inbound_filters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/inbound-filters\n  method: put\n  operationId: update_inbound_filters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/ingest-keys\n  method: get\n  operationId: list_project_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/ingest-keys\n  method: post\n  operationId: create_project_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/ingest-keys/{key_id}\n  method: delete\n  operationId: revoke_project_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/projects/{project_id}/restore\n  method: post\n  operationId: restore_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/sample-data\n  method: delete\n  operationId: remove_sample_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/sample-data\n\
  \  method: get\n  operationId: get_sample_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/sample-data\n  method: post\n  operationId: load_sample_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/setup\n  method: get\n  operationId: get_project_setup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/setup/seen\n  method: post\n  operationId: record_setup_seen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ scope:\n    - browser\n    - cli\n    - sdk\n    - server\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/spike-protection\n  method: put\n  operationId: update_spike_protection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/test-event\n  method: post\n  operationId: send_test_event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/webhooks\n  method: get\n  operationId: list_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/webhooks\n  method: post\n  operationId: create_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/webhooks/{webhook_id}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/webhooks/{webhook_id}\n  method: patch\n  operationId: update_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{project_id}/webhooks/{webhook_id}/deliveries\n  method: get\n  operationId: list_webhook_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{project_id}/webhooks/{webhook_id}/test\n\
  \  method: post\n  operationId: test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/release-artifacts\n  method: get\n  operationId: list_release_artifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/release-artifacts/symbolicate\n  method: post\n  operationId: symbolicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/support/tickets\n\
  \  method: get\n  operationId: list_support_tickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/support/tickets\n  method: post\n  operationId: create_support_ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/support/tickets/{ticket_id}\n  method: get\n  operationId: get_support_ticket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/support/tickets/{ticket_id}\n  method: patch\n  operationId: update_support_ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/support/tickets/{ticket_id}/context\n  method: get\n  operationId: list_support_ticket_context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/support/tickets/{ticket_id}/context\n  method: post\n  operationId: add_support_ticket_context\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/telemetry/actions\n  method: get\n  operationId: list_actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n   \
  \ - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/telemetry/actions/{action_id}/investigation\n  method: get\n  operationId: investigate_action\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/telemetry/analytics/funnel\n  method: post\n  operationId: get_funnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/telemetry/analytics/lifecycle\n  method: post\n  operationId: get_lifecycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (42 KB total) ---\n# Full source: https://artifacts.apis.io/logbrew/agentic-access/logbrew-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/logbrew/agentic-access/logbrew-agentic-access.yml
summary_line: 141 operations · 65 acting · 6 human-in-the-loop
tags:
- Observability
- Logging
- Monitoring
- Analytics
- Error Tracking
---
