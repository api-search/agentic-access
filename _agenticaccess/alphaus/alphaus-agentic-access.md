---
acting_count: 404
action_class_counts:
  acting: 404
  connected: 182
api_specs:
- filename: alphaus-blueapi-openapi-original.json
  format: json
  label: Blue API
  slug: blue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-blueapi-openapi-original.json
consequence_counts:
  physical: 66
  read: 182
  safety-critical: 8
  write: 330
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Alphaus Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /admin/v1/wavefeatures
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam/v1/password:reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam/v1/ripple/password:requestresetcode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam/v1/ripple/password:reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam/v1/{user}/password:verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/demo/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/me/password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/members/resetpassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/v1/aws/xacct/cwms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/v1/aws/xacct/dca
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/v1/aws/xacct/dca/{target}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /org/v1:sendVerification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/acctaccess/{target}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/aws/acctaccess
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/aws/acctaccess/cur
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/aws/acctaccess/stackset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/aws/xacct/spa
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/billinggroup/{id}:additionalCharges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/billinggroup/{id}:invoiceSettings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/billinggroup/{id}:resellerCharges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/billinggroups/children/{internalId}/invoiceSettings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billinggroups/children/{internalId}/serviceDiscounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billinggroups/children/{internalId}/serviceDiscounts/accounts:set
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/billinggroups/{id}/invoicelayoutconfig
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billinggroups/{id}/invoicelayoutconfig
operation_count: 586
overview: 'Alphaus exposes 586 API operations that an AI agent could call, of which 404 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 182 read, 330 write, 66 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alphaus
provider_slug: alphaus
slug: alphaus-agentic-access
source_filename: alphaus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/alphaus-blueapi-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 586\n  by_action_class:\n    connected: 182\n    acting: 404\n  by_consequence:\n    read: 182\n    write: 330\n    physical: 66\n    safety-critical: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /admin/v1/acctgroups\n  method: get\n  operationId: Admin_ListAccountGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/acctgroups/{id}\n  method: get\n  operationId: Admin_GetAccountGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/auditlogs:export\n  method: post\n  operationId: Admin_ExportAuditLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/reports/proforma\n  method: post\n  operationId: Admin_CreateProformaCur\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/cwms\n  method: get\n  operationId: Admin_GetCloudWatchMetricsStreamTemplateUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/cwms\n  method: post\n  operationId: Admin_CreateCloudWatchMetricsStream\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca\n  method: get\n  operationId: Admin_GetDefaultCostAccessTemplateUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/dca\n  method: post\n  operationId: Admin_CreateDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/all:read\n  method: post\n  operationId: Admin_ListDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: get\n  operationId: Admin_GetDefaultCostAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: delete\n  operationId: Admin_DeleteDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: put\n  operationId: Admin_UpdateDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/defaultmeta\n  method: put\n  operationId: Admin_UpdateMSPDefaultMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/defaultmeta/{mspId}\n\
  \  method: get\n  operationId: Admin_GetMSPDefaultMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels\n  method: get\n  operationId: Admin_ListNotificationChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels\n  method: post\n  operationId: Admin_CreateNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/channels/{id}\n  method: get\n  operationId: Admin_GetNotificationChannel\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels/{id}\n  method: delete\n  operationId: Admin_DeleteNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/channels/{id}\n  method: put\n  operationId: Admin_UpdateNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/default\n  method: post\n  operationId: Admin_CreateDefaultNotificationChannel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/settings\n  method: get\n  operationId: Admin_GetNotificationSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/settings\n  method: post\n  operationId: Admin_SaveNotificationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications\n  method: get\n  operationId: Admin_ListNotifications\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notifications\n  method: post\n  operationId: Admin_CreateNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications/{id}\n  method: get\n  operationId: Admin_GetNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notifications/{id}\n  method: delete\n  operationId: Admin_DeleteNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications/{id}\n  method: put\n  operationId: Admin_UpdateNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/wavefeatures\n  method: get\n  operationId: Admin_GetWaveFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/wavefeatures\n  method: put\n  operationId: Admin_UpdateWaveFeatureSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing/v1/reseller/announcements/{announcementId}\n  method: get\n  operationId: Billing_GetAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flags/v1/namespace/{namespaceId}/boolean/{id}:eval\n  method: post\n  operationId: Flags_EvaluateBooleanFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flags/v1/namespace/{namespaceId}/variant/{id}:eval\n  method: post\n  operationId: Flags_EvaluateVariantFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/apiclients\n  method: get\n  operationId: Iam_ListApiClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/apiclients\n  method: post\n  operationId: Iam_CreateApiClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/apiclients/{id}\n  method: delete\n  operationId: Iam_DeleteApiClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/experimentalui/preferences\n  method: get\n  operationId: Iam_GetExperimentalUIPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/experimentalui/preferences/{componentId}\n  method: put\n  operationId: Iam_UpsertExperimentalUIPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/grouprootusers\n  method: get\n  operationId: Iam_ListGroupRootUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/grouprootusers\n  method:\
  \ post\n  operationId: Iam_CreateGroupRootUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/grouprootusers/{id}\n  method: get\n  operationId: Iam_GetGroupRootUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/grouprootusers/{id}\n  method: delete\n  operationId: Iam_DeleteGroupRootUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/grouprootusers/{id}/features\n  method: get\n  operationId:\
  \ Iam_GetFeatureFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/grouprootusers/{id}/features\n  method: put\n  operationId: Iam_UpdateFeatureFlags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/idps\n  method: get\n  operationId: Iam_ListIdentityProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/idps\n  method: post\n  operationId: Iam_CreateIdentityProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/idps/{id}\n  method: delete\n  operationId: Iam_DeleteIdentityProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/ipfilters\n  method: get\n  operationId: Iam_ListIpFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/ipfilters\n  method: post\n  operationId: Iam_CreateIpFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/ipfilters/{id}\n  method: delete\n  operationId: Iam_DeleteIpFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/metadata/{id}\n  method: get\n  operationId: Iam_GetSubUserMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/mfausers\n  method: get\n  operationId: Iam_GetMFAUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/partners/{id}/token\n  method: post\n  operationId: Iam_CreatePartnerToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/partners/{id}/token:refresh\n  method: post\n  operationId: Iam_RefreshPartnerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/password:reset\n  method: post\n  operationId: Iam_ValidateResetPasswordLinkAndChangePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /iam/v1/permissions\n  method: get\n  operationId: Iam_ListPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/ripple/password:requestresetcode\n  method: post\n  operationId: Iam_SendRipplePasswordResetCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /iam/v1/ripple/password:reset\n  method: post\n  operationId: Iam_ResetRipplePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /iam/v1/roles\n  method: get\n  operationId: Iam_ListRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/roles\n  method: post\n  operationId: Iam_CreateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/roles/{namespace}/{name}\n  method: delete\n  operationId: Iam_DeleteRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /iam/v1/roles/{namespace}/{name}\n  method: put\n  operationId: Iam_UpdateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/userroles\n  method: get\n  operationId: Iam_ListUserRoleMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/userroles\n  method: post\n  operationId: Iam_CreateUserRoleMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /iam/v1/userroles\n  method: put\n  operationId: Iam_UpdateUserRoleMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/users\n  method: get\n  operationId: Iam_ListUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/users\n  method: post\n  operationId: Iam_CreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/users/{id}\n  method: get\n  operationId: Iam_GetUser\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/users/{id}\n  method: delete\n  operationId: Iam_DeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/whoami\n  method: get\n  operationId: Iam_WhoAmI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1/{domain}/account:unlock\n  method: post\n  operationId: Iam_UnlockUserAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1/{user}/password:verify\n  method: post\n  operationId: Iam_VerifyUserForResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ops/v1\n  method: get\n  operationId: Operations_ListOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ops/v1/{name}\n  method: get\n  operationId: Operations_GetOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ops/v1/{name}\n  method: delete\n  operationId: Operations_DeleteOperation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ops/v1/{name}:cancel\n  method: post\n  operationId: Operations_CancelOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1\n  method: get\n  operationId: Organization_GetOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/v1\n  method: delete\n  operationId: Organization_DeleteOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1\n  method: post\n  operationId: Organization_CreateOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1/metadata\n  method: put\n  operationId: Organization_UpdateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1/passwd\n  method: put\n  operationId: Organization_UpdatePassword\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1:sendVerification\n  method: post\n  operationId: Organization_SendVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/v1:verify\n  method: post\n  operationId: Organization_VerifyOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /prefs/v1\n  method: get\n  operationId: Preferences_GetPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/info\n  method: get\n  operationId: Pricing_GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/{vendor}/pricing\n  method: post\n  operationId: Pricing_GetPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/{vendor}/services\n  method: get\n  operationId: Pricing_GetSupportedServices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups\n  method: get\n  operationId: Billing_ListAccessGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups\n  method: post\n  operationId: Billing_CreateAccessGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessgroups/{accessGroupId}\n  method: get\n  operationId: Billing_GetAccessGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups/{id}\n  method: delete\n  operationId: Billing_DeleteAccessGroup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessgroups/{id}\n  method: put\n  operationId: Billing_UpdateAccessGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account\n  method: post\n  operationId: Cover_RegisterDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/account/all:read\n  method: post\n  operationId: Cover_ListDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/unregistered:read\n  method: post\n  operationId: Cover_ListUnregisteredAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{target}\n  method: get\n  operationId: Cover_GetDataAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{target}\n  method:\
  \ delete\n  operationId: Cover_DeleteDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{target}\n  method: put\n  operationId: Cover_UpdateDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/acctaccess/{target}\n  method: delete\n  operationId: Cover_DeleteAccountAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/activity/all:read\n  method: post\n  operationId: Prism_ListActivities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: get\n  operationId: Billing_GetAdjustmentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/adjustmentconfig/{vendor}\n  method: delete\n  operationId: Billing_DeleteAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: post\n  operationId: Billing_CreateAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: put\n  operationId: Billing_UpdateAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/costusage\n  method: post\n  operationId: Cover_GetAICostAndUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers\n\n# --- truncated at 32 KB (186 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/agentic-access/alphaus-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/agentic-access/alphaus-agentic-access.yml
summary_line: 586 operations · 404 acting · 8 human-in-the-loop
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud
- Billing
- Multi-Cloud
- Azure
- GCP
- gRPC
- Cost Optimization
- Reseller Billing
- API
---
