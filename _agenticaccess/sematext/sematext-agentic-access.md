---
acting_count: 60
action_class_counts:
  acting: 60
  connected: 34
api_specs:
- filename: sematext-alert-notifications-api-openapi.yml
  format: yaml
  label: Sematext Alert Notifications API
  slug: sematext-alert-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alert-notifications-api-openapi.yml
- filename: sematext-alerts-api-openapi.yml
  format: yaml
  label: Sematext Alerts API
  slug: sematext-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alerts-api-openapi.yml
- filename: sematext-app-guests-api-openapi.yml
  format: yaml
  label: Sematext App guests API
  slug: sematext-app-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-guests-api-openapi.yml
- filename: sematext-app-ips-api-openapi.yml
  format: yaml
  label: Sematext App IPs API
  slug: sematext-app-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-ips-api-openapi.yml
- filename: sematext-app-tokens-api-openapi.yml
  format: yaml
  label: Sematext App tokens API
  slug: sematext-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-tokens-api-openapi.yml
- filename: sematext-apps-api-openapi.yml
  format: yaml
  label: Sematext Apps API
  slug: sematext-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-apps-api-openapi.yml
- filename: sematext-billing-api-openapi.yml
  format: yaml
  label: Sematext Billing API
  slug: sematext-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-billing-api-openapi.yml
- filename: sematext-experience-app-api-openapi.yml
  format: yaml
  label: Sematext Experience App API
  slug: sematext-experience-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-experience-app-api-openapi.yml
- filename: sematext-logs-app-api-openapi.yml
  format: yaml
  label: Sematext Logs App API
  slug: sematext-logs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-api-openapi.yml
- filename: sematext-logs-app-usage-api-openapi.yml
  format: yaml
  label: Sematext Logs App usage API
  slug: sematext-logs-app-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-usage-api-openapi.yml
- filename: sematext-monitoring-app-api-openapi.yml
  format: yaml
  label: Sematext Monitoring App API
  slug: sematext-monitoring-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-monitoring-app-api-openapi.yml
- filename: sematext-notifications-api-openapi.yml
  format: yaml
  label: Sematext Notifications API
  slug: sematext-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-notifications-api-openapi.yml
- filename: sematext-reset-password-api-openapi.yml
  format: yaml
  label: Sematext Reset Password API
  slug: sematext-reset-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-reset-password-api-openapi.yml
- filename: sematext-subscriptions-api-openapi.yml
  format: yaml
  label: Sematext Subscriptions API
  slug: sematext-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-subscriptions-api-openapi.yml
- filename: sematext-tags-api-openapi.yml
  format: yaml
  label: Sematext Tags API
  slug: sematext-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-tags-api-openapi.yml
consequence_counts:
  physical: 4
  read: 34
  safety-critical: 10
  write: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Sematext Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users-web/api/v3/account/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users-web/api/v3/account/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/alerts/{updateableAlertId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/alerts/{updateableAlertId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users-web/api/v3/apps/{token}/ips/{ipId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users-web/api/v3/apps/{token}/ips/{ipId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /users-web/api/v3/apps/{appId}/report/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /users-web/api/v3/apps/{appId}/report/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /users-web/api/v3/dashboards/{dashId}/report/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /users-web/api/v3/dashboards/{dashId}/report/send
operation_count: 94
overview: 'Sematext exposes 94 API operations that an AI agent could call, of which 60 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 46 write, 4 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sematext
provider_slug: sematext
slug: sematext-agentic-access
source_filename: sematext-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/sematext-cloud-openapi-original.json, openapi/sematext-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 94\n  by_action_class:\n    acting: 60\n    connected: 34\n  by_consequence:\n    safety-critical: 10\n    write: 46\n    read: 34\n    physical: 4\n  human_in_the_loop_required: 10\noperations:\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}\n  method: put\n  operationId: updateAppToken_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}\n  method: delete\n  operationId: deleteAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens\n  method: get\n  operationId: getAppTokens_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{appId}/tokens\n  method: post\n  operationId: createAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips/{ipId}\n  method: put\n  operationId: updateAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips/{ipId}\n  method: delete\n  operationId: deleteAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/disable\n\
  \  method: put\n  operationId: disableUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}\n  method: delete\n  operationId: deleteAlertRuleUsingDELETE_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}/regenerate\n  method: post\n  operationId: regenerateAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts\n  method: post\n  operationId: createAlertUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions/{updateableSubscriptionId}\n  method: put\n  operationId: toggleEnabledUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions/{updateableSubscriptionId}\n  method: delete\n  operationId: deleteUsingDELETE_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}/enable\n  method: put\n  operationId: enableAlertRuleUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/types\n  method: get\n  operationId: getAppTypesUsingGET\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/availablePlans\n  method: get\n  operationId: listAvailablePlansUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/invoice/{service}/{year}/{month}\n  method: get\n  operationId: getDetailedInvoiceUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/notifications/alerts\n  method: post\n  operationId: getAlertNotificationsForUserUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /users-web/api/v3/dashboards/{dashId}/report/send\n  method: post\n  operationId: sendDashReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips\n  method: get\n  operationId: getAppIps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{token}/ips\n  method: post\n  operationId: createAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/alerts\n  method: get\n  operationId: getAlertRulesForAppUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/enable\n  method: put\n  operationId: enableUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscriptions\n  method: get\n  operationId: listUsingGET_2\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/info/{appId}\n  method: put\n  operationId: updatePlanUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{anyStateAppId}\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{anyStateAppId}\n  method: put\n  operationId: updateUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{anyStateAppId}\n  method: delete\n  operationId: deleteUsingDELETE_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}/disable\n  method: put\n  operationId: disableAlertRuleUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/account/password/reset\n  method: post\n  operationId: resetPasswordUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/apps/guests\n  method: post\n  operationId: inviteAppGuestsUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/dashboards/{dashId}/subscription\n  method: post\n  operationId: createForDashUsingPOST_1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/dashboards/{dashId}/subscription\n  method: put\n  operationId: updateForDashUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscription\n  method: post\n  operationId: createForAppUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscription\n  method: put\n  operationId: updateForAppUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps\n  method: get\n  operationId: listUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps\n  method: post\n  operationId: createExperienceApp_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/notifications/alerts\n  method: post\n  operationId: getAlertNotificationsForAppUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/users\n  method: get\n  operationId: listAppsUsersUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{appId}/report/send\n  method: post\n  operationId: sendAppReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions\n  method: get\n  operationId: listUsingGET_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{anyStateAppId}/description\n  method: put\n  operationId: updateDescriptionUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logsene-reports/api/v3/apps\n  method: post\n  operationId: createLogseneApplication\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logsene-reports/api/v3/apps/{appId}/usage/{from}/{to}\n  method: get\n  operationId: getForRangeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spm-reports/api/v3/apps/{appIds}/metrics/filters\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spm-reports/api/v3/apps\n  method: post\n  operationId: createSpmApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spm-reports/api/v3/apps/{appIds}/tags\n  method: get\n  operationId: getUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spm-reports/api/v3/apps/{appIds}/tagNames\n  method: get\n  operationId: getTagNamesUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}\n  method: put\n  operationId: updateAppToken_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n   \
  \ - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}\n  method: delete\n  operationId: deleteAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens\n  method: get\n  operationId: getAppTokens_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{appId}/tokens\n  method: post\n  operationId: createAppToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips/{ipId}\n  method: put\n  operationId: updateAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips/{ipId}\n  method: delete\n  operationId: deleteAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/disable\n  method: put\n  operationId: disableUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}\n  method: delete\n  operationId: deleteAlertRuleUsingDELETE_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /users-web/api/v3/apps/{appId}/tokens/{tokenId}/regenerate\n  method: post\n  operationId: regenerateAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts\n  method: post\n  operationId: createAlertUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions/{updateableSubscriptionId}\n  method: put\n  operationId: toggleEnabledUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions/{updateableSubscriptionId}\n  method: delete\n  operationId: deleteUsingDELETE_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}/enable\n  method: put\n  operationId: enableAlertRuleUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/types\n  method: get\n  operationId: getAppTypesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/availablePlans\n  method: get\n  operationId: listAvailablePlansUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/invoice/{service}/{year}/{month}\n  method: get\n  operationId: getDetailedInvoiceUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/notifications/alerts\n  method: post\n  operationId:\
  \ getAlertNotificationsForUserUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/dashboards/{dashId}/report/send\n  method: post\n  operationId: sendDashReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{token}/ips\n  method: get\n  operationId: getAppIps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{token}/ips\n  method: post\n\
  \  operationId: createAppIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/alerts\n  method: get\n  operationId: getAlertRulesForAppUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/notifications/integrations/{updateableNotificationIntegrationId}/enable\n  method: put\n  operationId: enableUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscriptions\n  method: get\n  operationId: listUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/billing/info/{appId}\n  method: put\n  operationId: updatePlanUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{anyStateAppId}\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /users-web/api/v3/apps/{anyStateAppId}\n  method: put\n  operationId: updateUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{anyStateAppId}\n  method: delete\n  operationId: deleteUsingDELETE_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/alerts/{updateableAlertId}/disable\n  method: put\n  operationId: disableAlertRuleUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/account/password/reset\n  method: post\n  operationId: resetPasswordUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users-web/api/v3/apps/guests\n  method: post\n  operationId: inviteAppGuestsUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/dashboards/{dashId}/subscription\n  method: post\n  operationId: createForDashUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/dashboards/{dashId}/subscription\n  method: put\n  operationId: updateForDashUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscription\n\
  \  method: post\n  operationId: createForAppUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/subscription\n  method: put\n  operationId: updateForAppUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps\n  method: get\n  operationId: listUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /users-web/api/v3/apps\n  method: post\n  operationId: createExperienceApp_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/apps/{appId}/notifications/alerts\n  method: post\n  operationId: getAlertNotificationsForAppUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/users\n  method: get\n  operationId: listAppsUsersUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{appId}/report/send\n\
  \  method: post\n  operationId: sendAppReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-web/api/v3/subscriptions\n  method: get\n  operationId: listUsingGET_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users-web/api/v3/apps/{anyStateAppId}/description\n  method: put\n  operationId: updateDescriptionUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logsene-reports/api/v3/apps\n  method: post\n  operationId: createLogseneApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logsene-reports/api/v3/apps/{appId}/usage/{from}/{to}\n  method: get\n  operationId: getForRangeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spm-reports/api/v3/apps/{appIds}/metrics/filters\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (32 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/agentic-access/sematext-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/agentic-access/sematext-agentic-access.yml
summary_line: 94 operations · 60 acting · 10 human-in-the-loop
tags:
- Company
- Observability
- Monitoring
- Logging
- Log Management
- Elasticsearch
- Tracing
- Synthetic Monitoring
- OpenTelemetry
---
