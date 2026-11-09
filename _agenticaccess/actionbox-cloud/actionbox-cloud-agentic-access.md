---
acting_count: 95
action_class_counts:
  acting: 95
  connected: 50
api_specs:
- filename: actionbox-cloud-account-api-openapi.yml
  format: yaml
  label: actionbox-cloud Account API
  slug: actionbox-cloud-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-account-api-openapi.yml
- filename: actionbox-cloud-actions-api-openapi.yml
  format: yaml
  label: actionbox-cloud Actions API
  slug: actionbox-cloud-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-actions-api-openapi.yml
- filename: actionbox-cloud-analytics-api-openapi.yml
  format: yaml
  label: actionbox-cloud Analytics API
  slug: actionbox-cloud-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-analytics-api-openapi.yml
- filename: actionbox-cloud-auth-api-openapi.yml
  format: yaml
  label: actionbox-cloud Auth API
  slug: actionbox-cloud-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-auth-api-openapi.yml
- filename: actionbox-cloud-billing-api-openapi.yml
  format: yaml
  label: actionbox-cloud Billing API
  slug: actionbox-cloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-billing-api-openapi.yml
- filename: actionbox-cloud-dashboard-api-openapi.yml
  format: yaml
  label: actionbox-cloud Dashboard API
  slug: actionbox-cloud-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-dashboard-api-openapi.yml
- filename: actionbox-cloud-devices-api-openapi.yml
  format: yaml
  label: actionbox-cloud Devices API
  slug: actionbox-cloud-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-devices-api-openapi.yml
- filename: actionbox-cloud-documentation-api-openapi.yml
  format: yaml
  label: actionbox-cloud Documentation API
  slug: actionbox-cloud-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-documentation-api-openapi.yml
- filename: actionbox-cloud-feedback-api-openapi.yml
  format: yaml
  label: actionbox-cloud Feedback API
  slug: actionbox-cloud-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-feedback-api-openapi.yml
- filename: actionbox-cloud-notifications-api-openapi.yml
  format: yaml
  label: actionbox-cloud Notifications API
  slug: actionbox-cloud-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-notifications-api-openapi.yml
- filename: actionbox-cloud-runs-api-openapi.yml
  format: yaml
  label: actionbox-cloud Runs API
  slug: actionbox-cloud-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-runs-api-openapi.yml
- filename: actionbox-cloud-slack-api-openapi.yml
  format: yaml
  label: actionbox-cloud Slack API
  slug: actionbox-cloud-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-slack-api-openapi.yml
- filename: actionbox-cloud-sources-api-openapi.yml
  format: yaml
  label: actionbox-cloud Sources API
  slug: actionbox-cloud-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-sources-api-openapi.yml
- filename: actionbox-cloud-system-api-openapi.yml
  format: yaml
  label: actionbox-cloud System API
  slug: actionbox-cloud-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-system-api-openapi.yml
- filename: actionbox-cloud-watches-api-openapi.yml
  format: yaml
  label: actionbox-cloud Watches API
  slug: actionbox-cloud-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-watches-api-openapi.yml
- filename: actionbox-cloud-webhooks-api-openapi.yml
  format: yaml
  label: actionbox-cloud Webhooks API
  slug: actionbox-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-webhooks-api-openapi.yml
- filename: actionbox-cloud-workspaces-api-openapi.yml
  format: yaml
  label: actionbox-cloud Workspaces API
  slug: actionbox-cloud-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-workspaces-api-openapi.yml
consequence_counts:
  physical: 1
  read: 50
  safety-critical: 6
  write: 88
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Actionbox Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/actions/{action_id}/controls/{control_key}/invoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/mfa/recovery/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/auth/mfa/totp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/devices/{device_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/source/control-requests/{control_request_id}/result
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/invitations/{invitation_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 145
overview: 'actionbox-cloud exposes 145 API operations that an AI agent could call, of which 95 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 88 write, 1 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: actionbox-cloud
provider_slug: actionbox-cloud
slug: actionbox-cloud-agentic-access
source_filename: actionbox-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/actionbox-cloud-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 145\n  by_action_class:\n    connected: 50\n    acting: 95\n  by_consequence:\n    read: 50\n    write: 88\n    safety-critical: 6\n    physical: 1\n  human_in_the_loop_required: 6\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/keys\n  method: get\n  operationId: receipt_keys_v1_receipts_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/docs\n  method: get\n  operationId: user_documentation_v1_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ready\n  method: get\n  operationId: readiness_ready_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/providers\n  method: get\n  operationId: auth_providers_v1_auth_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/google/native\n  method: post\n  operationId: native_google_login_v1_auth_google_native_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/google/native/challenge\n  method: post\n  operationId: native_google_challenge_v1_auth_google_native_challenge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/apple/native/challenge\n  method: post\n  operationId: native_apple_challenge_v1_auth_apple_native_challenge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/apple/native\n  method: post\n  operationId: native_apple_login_v1_auth_apple_native_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/apple/android\n  method: post\n  operationId: apple_android_login_v1_auth_apple_android_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/session\n  method: get\n  operationId: auth_session_v1_auth_session_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces\n  method: get\n  operationId: workspaces_endpoint_v1_workspaces_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/select\n  method: post\n  operationId: select_workspace_endpoint_v1_workspaces_select_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/members\n  method: get\n  operationId: workspace_members_endpoint_v1_workspaces_members_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/invitations\n\
  \  method: get\n  operationId: workspace_invitations_endpoint_v1_workspaces_invitations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/invitations\n  method: post\n  operationId: create_workspace_invitation_endpoint_v1_workspaces_invitations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/groups\n  method: get\n  operationId: workspace_groups_endpoint_v1_workspaces_groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/groups\n  method: post\n  operationId: create_workspace_group_endpoint_v1_workspaces_groups_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/groups/{group_id}\n  method: patch\n  operationId: rename_workspace_group_endpoint_v1_workspaces_groups__group_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/groups/{group_id}\n  method: delete\n  operationId: delete_workspace_group_endpoint_v1_workspaces_groups__group_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/groups/{group_id}/members\n  method: put\n  operationId: replace_workspace_group_members_endpoint_v1_workspaces_groups__group_id__members_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/approval-policies\n  method: get\n  operationId: list_workspace_managed_policies_endpoint_v1_workspaces_approval_policies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/approval-policies\n  method: post\n  operationId: create_workspace_managed_policy_endpoint_v1_workspaces_approval_policies_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/approval-policies/{policy_id}\n  method: patch\n  operationId: update_workspace_managed_policy_endpoint_v1_workspaces_approval_policies__policy_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{source_id}/approval-policy\n  method: get\n  operationId: source_approval_policy_endpoint_v1_sources__source_id__approval_policy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/sources/{source_id}/approval-policy\n  method: put\n  operationId: set_source_approval_policy_endpoint_v1_sources__source_id__approval_policy_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/audit-events\n  method: get\n  operationId: workspace_audit_events_endpoint_v1_workspaces_audit_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/audit-events/export\n  method: get\n  operationId: workspace_audit_export_endpoint_v1_workspaces_audit_events_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/audit-events/integrity\n  method: get\n  operationId: workspace_audit_integrity_endpoint_v1_workspaces_audit_events_integrity_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/audit-events/integrity/verify\n  method: post\n  operationId: workspace_audit_verify_checkpoint_endpoint_v1_workspaces_audit_events_integrity_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/invitations/{invitation_id}\n  method: delete\n  operationId: revoke_workspace_invitation_endpoint_v1_workspaces_invitations__invitation_id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workspace-invitations/accept\n  method: post\n  operationId: accept_workspace_invitation_endpoint_v1_workspace_invitations_accept_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/members/{user_id}\n  method: patch\n  operationId: update_workspace_member_endpoint_v1_workspaces_members__user_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/members/{user_id}\n  method: delete\n  operationId: remove_workspace_member_endpoint_v1_workspaces_members__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/leave\n  method: post\n  operationId: leave_workspace_endpoint_v1_workspaces_leave_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications\n  method: get\n  operationId: notifications_endpoint_v1_notifications_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/summary\n  method: get\n  operationId: notification_summary_endpoint_v1_notifications_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/read-all\n  method: post\n  operationId: read_all_notifications_endpoint_v1_notifications_read_all_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/{notification_id}/read\n  method: post\n  operationId: read_notification_endpoint_v1_notifications__notification_id__read_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification-preferences\n  method: get\n  operationId: notification_preferences_endpoint_v1_notification_preferences_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification-preferences\n  method: patch\n  operationId: update_notification_preferences_endpoint_v1_notification_preferences_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/notification-policy\n\
  \  method: get\n  operationId: workspace_notification_policy_endpoint_v1_workspaces_notification_policy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/notification-policy\n  method: patch\n  operationId: update_workspace_notification_policy_endpoint_v1_workspaces_notification_policy_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing\n  method: get\n  operationId: billing_endpoint_v1_billing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/purchase-eligibility\n  method: get\n  operationId: billing_purchase_eligibility_endpoint_v1_billing_purchase_eligibility_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/portal\n  method: post\n  operationId: billing_portal_endpoint_v1_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: post\n  operationId: billing_checkout_endpoint_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/logout\n\
  \  method: post\n  operationId: logout_v1_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/export\n  method: get\n  operationId: account_export_v1_account_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: delete\n  operationId: account_delete_v1_account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bootstrap\n  method: get\n  operationId: bootstrap_v1_bootstrap_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/summary\n  method: get\n  operationId: analytics_summary_endpoint_v1_analytics_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: product_feedback_endpoint_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/events\n  method: post\n  operationId: analytics_event_endpoint_v1_analytics_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/actions\n  method: get\n  operationId: list_my_actions_v1_me_actions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs\n  method: post\n  operationId: create_run_endpoint_v1_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/runs\n  method: get\n  operationId: list_runs_endpoint_v1_runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/runs/{run_id}\n  method: get\n  operationId: get_run_endpoint_v1_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/source/runs/{run_id}\n  method: get\n  operationId: get_source_run_endpoint_v1_source_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/source/runs/{run_id}/progress\n  method: patch\n  operationId: update_run_progress_endpoint_v1_source_runs__run_id__progress_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/source/runs/{run_id}/complete\n  method: post\n  operationId: complete_run_endpoint_v1_source_runs__run_id__complete_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/context/{block_index}/diagram\n  method: get\n  operationId: get_action_diagram_v1_actions__action_id__context__block_index__diagram_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/actions/{action_id}\n  method: get\n  operationId: get_action_v1_actions__action_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/actions/{action_id}\n  method: patch\n  operationId: patch_action_endpoint_v1_actions__action_id__patch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/comments\n  method: get\n  operationId: action_comments_endpoint_v1_actions__action_id__comments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/actions/{action_id}/comments\n  method: post\n  operationId: create_action_comment_endpoint_v1_actions__action_id__comments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/context-request\n  method: post\n  operationId:\
  \ request_action_context_endpoint_v1_actions__action_id__context_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/source/actions/{action_id}/context-request/unavailable\n  method: post\n  operationId: decline_action_context_endpoint_v1_source_actions__action_id__context_request_unavailable_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/source/actions/{action_id}\n  method: get\n  operationId: get_source_action_v1_source_actions__action_id__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/actions\n  method: post\n  operationId: create_action_endpoint_v1_actions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/controls/{control_key}/invoke\n  method: post\n  operationId: invoke_control_endpoint_v1_actions__action_id__controls__control_key__invoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/actions/{action_id}/control-requests\n\
  \  method: get\n  operationId: list_control_requests_endpoint_v1_actions__action_id__control_requests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/source/control-requests/{control_request_id}/result\n  method: post\n  operationId: report_control_result_endpoint_v1_source_control_requests__control_request_id__result_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/actions/{action_id}/decision\n  method: post\n  operationId: decision_endpoint_v1_actions__action_id__decision_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/votes\n  method: post\n  operationId: approval_vote_endpoint_v1_actions__action_id__votes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/claim\n  method: post\n  operationId: claim_action_endpoint_v1_actions__action_id__claim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/assignment\n\
  \  method: patch\n  operationId: assign_action_endpoint_v1_actions__action_id__assignment_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/reviewers\n  method: patch\n  operationId: update_action_reviewers_endpoint_v1_actions__action_id__reviewers_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/resolve\n  method: post\n  operationId: resolve_endpoint_v1_actions__action_id__resolve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/outcome\n  method: post\n  operationId: report_action_outcome_endpoint_v1_actions__action_id__outcome_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actions/{action_id}/cancel\n  method: post\n  operationId: cancel_endpoint_v1_actions__action_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/actions/{action_id}/snooze\n  method: post\n  operationId: snooze_endpoint_v1_actions__action_id__snooze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources\n  method: get\n  operationId: sources_endpoint_v1_sources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources\n  method: post\n  operationId: create_source_endpoint_v1_sources_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/sources/{source_id}\n  method: get\n  operationId: source_detail_endpoint_v1_sources__source_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources/{source_id}\n  method: patch\n  operationId: update_source_endpoint_v1_sources__source_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{source_id}\n  method: delete\n  operationId: delete_source_endpoint_v1_sources__source_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{source_id}/keys/rotate\n  method: post\n  operationId: rotate_source_key_endpoint_v1_sources__source_id__keys_rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{source_id}/webhook-secret/rotate\n  method: post\n  operationId: rotate_webhook_secret_endpoint_v1_sources__source_id__webhook_secret_rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/source/watches\n  method: get\n  operationId:\
  \ source_watches_endpoint_v1_source_watches_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/source/watches\n  method: post\n  operationId: source_create_watch_endpoint_v1_source_watches_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/source/watches/{watch_id}/pause\n  method: post\n  operationId: source_pause_watch_endpoint_v1_source_watches__watch_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/source/watches/{watch_id}/resume\n  method: post\n  operationId: source_resume_watch_endpoint_v1_source_watches__watch_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (49 KB total) ---\n# Full source: https://artifacts.apis.io/actionbox-cloud/agentic-access/actionbox-cloud-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/actionbox-cloud/agentic-access/actionbox-cloud-agentic-access.yml
summary_line: 145 operations · 95 acting · 6 human-in-the-loop
tags:
- Artificial Intelligence
- Human-in-the-Loop
- Automation
- Approval
- Cloud
---
