---
acting_count: 401
action_class_counts:
  acting: 401
  connected: 185
api_specs:
- filename: alphaus-admin-api-openapi.yml
  format: yaml
  label: Alphaus Admin API
  slug: alphaus-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-admin-api-openapi.yml
- filename: alphaus-billing-api-openapi.yml
  format: yaml
  label: Alphaus Billing API
  slug: alphaus-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-billing-api-openapi.yml
- filename: alphaus-cost-api-openapi.yml
  format: yaml
  label: Alphaus Cost API
  slug: alphaus-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-cost-api-openapi.yml
- filename: alphaus-cover-api-openapi.yml
  format: yaml
  label: Alphaus Cover API
  slug: alphaus-cover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-cover-api-openapi.yml
- filename: alphaus-flags-api-openapi.yml
  format: yaml
  label: Alphaus Flags API
  slug: alphaus-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-flags-api-openapi.yml
- filename: alphaus-flow-api-openapi.yml
  format: yaml
  label: Alphaus Flow API
  slug: alphaus-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-flow-api-openapi.yml
- filename: alphaus-guaranteedcommitments-api-openapi.yml
  format: yaml
  label: Alphaus GuaranteedCommitments API
  slug: alphaus-guaranteedcommitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-guaranteedcommitments-api-openapi.yml
- filename: alphaus-iam-api-openapi.yml
  format: yaml
  label: Alphaus Iam API
  slug: alphaus-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-iam-api-openapi.yml
- filename: alphaus-luster-api-openapi.yml
  format: yaml
  label: Alphaus Luster API
  slug: alphaus-luster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-luster-api-openapi.yml
- filename: alphaus-operations-api-openapi.yml
  format: yaml
  label: Alphaus Operations API
  slug: alphaus-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-operations-api-openapi.yml
- filename: alphaus-organization-api-openapi.yml
  format: yaml
  label: Alphaus Organization API
  slug: alphaus-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-organization-api-openapi.yml
- filename: alphaus-preferences-api-openapi.yml
  format: yaml
  label: Alphaus Preferences API
  slug: alphaus-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-preferences-api-openapi.yml
- filename: alphaus-pricing-api-openapi.yml
  format: yaml
  label: Alphaus Pricing API
  slug: alphaus-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-pricing-api-openapi.yml
- filename: alphaus-prism-api-openapi.yml
  format: yaml
  label: Alphaus Prism API
  slug: alphaus-prism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-prism-api-openapi.yml
- filename: alphaus-vortex-api-openapi.yml
  format: yaml
  label: Alphaus Vortex API
  slug: alphaus-vortex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-vortex-api-openapi.yml
consequence_counts:
  physical: 62
  read: 185
  safety-critical: 8
  write: 331
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
  path: /admin/v1/aws/xacct/dca
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /org/v1:sendVerification
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billinggroups/{id}/invoicetemplate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/commitments/plan/{planId}/apply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/commitments/purchaseplans/custom
operation_count: 586
overview: 'Alphaus exposes 586 API operations that an AI agent could call, of which 401 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 185 read, 331 write, 62 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alphaus
provider_slug: alphaus
slug: alphaus-agentic-access
source_filename: alphaus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/alphaus-admin-api-openapi.yml, openapi/alphaus-billing-api-openapi.yml, openapi/alphaus-cost-api-openapi.yml,\n  openapi/alphaus-cover-api-openapi.yml, openapi/alphaus-flags-api-openapi.yml, openapi/alphaus-flow-api-openapi.yml,\n  openapi/alphaus-guaranteedcommitments-api-openapi.yml, openapi/alphaus-iam-api-openapi.yml,\n  openapi/alphaus-luster-api-openapi.yml, openapi/alphaus-operations-api-openapi.yml, openapi/alphaus-organization-api-openapi.yml,\n  openapi/alphaus-preferences-api-openapi.yml, openapi/alphaus-pricing-api-openapi.yml, openapi/alphaus-prism-api-openapi.yml,\n  openapi/alphaus-vortex-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 586\n  by_action_class:\n\
  \    connected: 185\n    acting: 401\n  by_consequence:\n    read: 185\n    write: 331\n    physical: 62\n    safety-critical: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /admin/v1/acctgroups\n  method: get\n  operationId: Admin_ListAccountGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/acctgroups/{id}\n  method: get\n  operationId: Admin_GetAccountGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/auditlogs:export\n  method: post\n  operationId: Admin_ExportAuditLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/v1/aws/reports/proforma\n  method: post\n  operationId: Admin_CreateProformaCur\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/cwms\n  method: get\n  operationId: Admin_GetCloudWatchMetricsStreamTemplateUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/cwms\n  method: post\n  operationId: Admin_CreateCloudWatchMetricsStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/v1/aws/xacct/dca\n  method: get\n  operationId: Admin_GetDefaultCostAccessTemplateUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/dca\n  method: post\n  operationId: Admin_CreateDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/all:read\n  method: post\n  operationId: Admin_ListDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: get\n  operationId: Admin_GetDefaultCostAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: delete\n  operationId: Admin_DeleteDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/aws/xacct/dca/{target}\n  method: put\n  operationId: Admin_UpdateDefaultCostAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/defaultmeta\n  method: put\n  operationId: Admin_UpdateMSPDefaultMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/defaultmeta/{mspId}\n  method: get\n  operationId: Admin_GetMSPDefaultMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels\n  method: get\n  operationId: Admin_ListNotificationChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels\n  method: post\n  operationId: Admin_CreateNotificationChannel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/channels/{id}\n  method: get\n  operationId: Admin_GetNotificationChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/channels/{id}\n  method: delete\n  operationId: Admin_DeleteNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/channels/{id}\n  method: put\n  operationId: Admin_UpdateNotificationChannel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/default\n  method: post\n  operationId: Admin_CreateDefaultNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notification/settings\n  method: get\n  operationId: Admin_GetNotificationSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notification/settings\n  method: post\n  operationId: Admin_SaveNotificationSettings\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications\n  method: get\n  operationId: Admin_ListNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notifications\n  method: post\n  operationId: Admin_CreateNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications/{id}\n  method: get\n  operationId: Admin_GetNotification\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/notifications/{id}\n  method: delete\n  operationId: Admin_DeleteNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/notifications/{id}\n  method: put\n  operationId: Admin_UpdateNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/wavefeatures\n  method: get\n  operationId: Admin_GetWaveFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/wavefeatures\n  method: put\n  operationId: Admin_UpdateWaveFeatureSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing/v1/reseller/announcements/{announcementId}\n  method: get\n  operationId: Billing_GetAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups\n  method: get\n  operationId: Billing_ListAccessGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups\n\
  \  method: post\n  operationId: Billing_CreateAccessGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessgroups/{accessGroupId}\n  method: get\n  operationId: Billing_GetAccessGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessgroups/{id}\n  method: delete\n  operationId: Billing_DeleteAccessGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessgroups/{id}\n  method: put\n  operationId:\
  \ Billing_UpdateAccessGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: get\n  operationId: Billing_GetAdjustmentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/adjustmentconfig/{vendor}\n  method: delete\n  operationId: Billing_DeleteAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: post\n  operationId:\
  \ Billing_CreateAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/adjustmentconfig/{vendor}\n  method: put\n  operationId: Billing_UpdateAdjustmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aws/dailyrunhistory:read\n  method: post\n  operationId: Billing_ListAwsDailyRunHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/account\n  method: post\n  operationId: Billing_AddAccountToBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/customfield\n  method: post\n  operationId: Billing_AddBillingGroupCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/customfield/{groupId}/{customFieldId}\n  method: delete\n  operationId: Billing_DeleteBillingGroupCustomField\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/customfield:read\n  method: post\n  operationId: Billing_ListBillingGroupCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/reseller/announcements/{groupId}\n  method: get\n  operationId: Billing_GetBillingGroupAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroup/tags\n  method: post\n  operationId: Billing_AddTagsToBillingGroup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}\n  method: delete\n  operationId: Billing_DeleteBillinGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}/{vendor}/supportplan\n  method: get\n  operationId: Billing_GetBillingGroupAccountSupportPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroup/{id}/{vendor}/supportplan\n  method: put\n  operationId: Billing_UpdateBillingGroupAccountSupportPlan\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}/{vendor}/untaggedgroups\n  method: post\n  operationId: Billing_UpdateNonTagGroupToBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:additionalCharges\n  method: put\n  operationId: Billing_UpdateBillingGroupAdditionalCharges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:basicInfo\n  method: put\n  operationId: Billing_UpdateBillingGroupBasicInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:customFields\n  method: put\n  operationId: Billing_UpdateBillingGroupCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:freeFormat\n  method: put\n  operationId: Billing_UpdateBillingGroupFreeFormat\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:invoiceSettings\n  method: put\n  operationId: Billing_UpdateBillingGroupInvoiceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:resellerCharges\n  method: put\n  operationId: Billing_UpdateBillingGroupResellerCharges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroup/{id}:resources\n  method: put\n  operationId: Billing_UpdateBillingGroupLinkedResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups\n  method: get\n  operationId: Billing_ListBillingGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups\n  method: post\n  operationId: Billing_CreateBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/billingconductor/{id}\n  method: get\n  operationId: Billing_ListAbcBillingGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/billingconductor/{payerId}/accounts\n  method: get\n  operationId: Billing_ListAbcBillingGroupAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/children\n  method: post\n  operationId: Billing_CreateChildBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children/{internalId}\n  method: get\n  operationId: Billing_GetChildBillingGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/children/{internalId}\n  method: delete\n  operationId: Billing_DeleteChildBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children/{internalId}\n  method: put\n  operationId: Billing_UpdateChildBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children/{internalId}/invoiceSettings\n  method: put\n  operationId: Billing_UpdateChildBillingGroupInvoiceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children/{internalId}/serviceDiscounts\n  method: get\n  operationId: Billing_GetChildBillingGroupInvoiceServiceDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/children/{internalId}/serviceDiscounts\n  method: post\n  operationId: Billing_SetChildBillingGroupInvoiceServiceDiscounts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children/{internalId}/serviceDiscounts/accounts:read\n  method: get\n  operationId: Billing_ReadChildBillingGroupAccountInvoiceServiceDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/children/{internalId}/serviceDiscounts/accounts:set\n  method: post\n  operationId: Billing_SetChildBillingGroupAccountInvoiceServiceDiscounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/children:read\n  method: post\n  operationId: Billing_ReadChildBillingGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/exclude-service-settings\n  method: get\n  operationId: Billing_ListExcludeServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/exclude-service-settings\n  method: delete\n  operationId: Billing_DeleteExcludeServiceEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/exclude-service-settings\n  method: post\n  operationId: Billing_CreateExcludeServiceEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/exclude-service-settings\n  method: put\n  operationId: Billing_UpdateExcludeServiceEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/merged\n  method:\
  \ post\n  operationId: Billing_CreateBillingGroupMerged\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/{billingInternalId}\n  method: get\n  operationId: Billing_GetBillingGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/{id}/invoicelayoutconfig\n  method: get\n  operationId: Billing_GetBillingGroupInvoiceLayoutConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billinggroups/{id}/invoicelayoutconfig\n  method: delete\n  operationId: Billing_DeleteBillingGroupInvoiceLayoutConfig\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/{id}/invoicelayoutconfig\n  method: post\n  operationId: Billing_SetBillingGroupInvoiceLayoutConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups/{id}/invoicetemplate\n  method: post\n  operationId: Billing_UpdateBillingGroupInvoiceTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups:bulkCreate\n  method: post\n  operationId: Billing_BulkCreateBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups:bulkLinkAccount\n  method: post\n  operationId: Billing_BulkLinkAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups:bulkTag\n\
  \  method: post\n  operationId: Billing_BulkTagBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billinggroups:paginated\n  method: get\n  operationId: Billing_ListBillingGroupsPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits\n  method: get\n  operationId: Billing_GetCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/csvsettings\n  method: get\n  operationId: Billing_GetCsvSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/customfield\n  method: post\n  operationId: Billing_CreateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customfield/{id}\n  method: delete\n  operationId: Billing_DeleteCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customfield/{id}\n  method: put\n  operationId: Billing_UpdateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customfield:read\n  method: post\n  operationId: Billing_ListCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customizedbillingservices\n  method: post\n  operationId: Billing_CreateCustomizedBillingService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customizedbillingservices/billinggroup/{groupId}/{vendor}\n  method: get\n  operationId: Billing_GetCustomizedBillingServiceBillingGroup\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customizedbillingservices/billinggroup/{groupId}/{vendor}\n  method: delete\n  operationId: Billing_DeleteCustomizedBillingServiceBillingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (186 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/agentic-access/alphaus-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/agentic-access/alphaus-agentic-access.yml
summary_line: 586 operations · 401 acting · 8 human-in-the-loop
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
---
