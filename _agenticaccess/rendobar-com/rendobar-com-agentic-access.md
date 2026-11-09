---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 50
api_specs:
- filename: rendobar-com-account-api-openapi.yml
  format: yaml
  label: rendobar-com Account API
  slug: rendobar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-account-api-openapi.yml
- filename: rendobar-com-api-keys-api-openapi.yml
  format: yaml
  label: rendobar-com API Keys API
  slug: rendobar-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-api-keys-api-openapi.yml
- filename: rendobar-com-assets-api-openapi.yml
  format: yaml
  label: rendobar-com Assets API
  slug: rendobar-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-assets-api-openapi.yml
- filename: rendobar-com-billing-api-openapi.yml
  format: yaml
  label: rendobar-com Billing API
  slug: rendobar-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-billing-api-openapi.yml
- filename: rendobar-com-compose-api-openapi.yml
  format: yaml
  label: rendobar-com Compose API
  slug: rendobar-com-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-compose-api-openapi.yml
- filename: rendobar-com-jobs-api-openapi.yml
  format: yaml
  label: rendobar-com Jobs API
  slug: rendobar-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-jobs-api-openapi.yml
- filename: rendobar-com-models-api-openapi.yml
  format: yaml
  label: rendobar-com Models API
  slug: rendobar-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-models-api-openapi.yml
- filename: rendobar-com-notifications-api-openapi.yml
  format: yaml
  label: rendobar-com Notifications API
  slug: rendobar-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-notifications-api-openapi.yml
- filename: rendobar-com-organizations-api-openapi.yml
  format: yaml
  label: rendobar-com Organizations API
  slug: rendobar-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-organizations-api-openapi.yml
- filename: rendobar-com-sharing-api-openapi.yml
  format: yaml
  label: rendobar-com Sharing API
  slug: rendobar-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-sharing-api-openapi.yml
- filename: rendobar-com-storage-api-openapi.yml
  format: yaml
  label: rendobar-com Storage API
  slug: rendobar-com-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-storage-api-openapi.yml
- filename: rendobar-com-team-api-openapi.yml
  format: yaml
  label: rendobar-com Team API
  slug: rendobar-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-team-api-openapi.yml
- filename: rendobar-com-upload-sessions-api-openapi.yml
  format: yaml
  label: rendobar-com Upload Sessions API
  slug: rendobar-com-upload-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-upload-sessions-api-openapi.yml
- filename: rendobar-com-webhooks-api-openapi.yml
  format: yaml
  label: rendobar-com Webhooks API
  slug: rendobar-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 8
  read: 50
  safety-critical: 3
  write: 40
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Rendobar Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /orgs/current/invitations/{invitationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /team/revoke-invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout/credits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout/plan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout/pro
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /billing/payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /billing/payment-methods/{id}/default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /jobs/{id}/dispute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/current/exit-feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/endpoints/{id}/test
operation_count: 101
overview: 'rendobar-com exposes 101 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 40 write, 8 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rendobar-com
provider_slug: rendobar-com
slug: rendobar-com-agentic-access
source_filename: rendobar-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rendobar-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 101\n  by_action_class:\n    connected: 50\n    acting: 51\n  by_consequence:\n    read: 50\n    write: 40\n    physical: 8\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /jobs/types\n  method: get\n  operationId: listJobTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/types/{type}/schema\n  method: get\n  operationId: getJobTypeSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /jobs\n  method: post\n  operationId: submitJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/stats\n  method: get\n  operationId: getJobStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/deliveries/retry\n  method: post\n  operationId: retryDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/download\n  method: get\n  operationId: downloadJobOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/logs\n  method: get\n  operationId: getJobLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/resources\n  method: get\n  operationId: getJobResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/metrics\n  method: get\n  operationId: getJobMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/throughput\n  method: get\n  operationId: getJobThroughput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/timings\n  method: get\n  operationId: getJobTimings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/share\n  method: post\n  operationId: createJobShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/share\n  method: delete\n  operationId: deleteJobShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/share\n  method: get\n  operationId: getJobShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/dispute\n  method: post\n  operationId: disputeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /compose/validate\n  method: post\n  operationId: validateCompose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compose/effects\n  method: get\n  operationId: listComposeEffects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compose/effects/engine\n  method: get\n  operationId: listComposeEngineEffects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/state\n  method: get\n  operationId: getBillingState\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage-by-client\n  method: get\n  operationId: getUsageByClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credit-schedule\n  method: delete\n  operationId: cancelCreditSchedule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/checkout/credits\n  method: post\n  operationId: createCreditsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/checkout/plan\n  method: post\n  operationId: createPlanCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/checkout/pro\n  method: post\n  operationId: createProCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/subscription\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /billing/history\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/history/{id}/pdf\n  method: get\n  operationId: getInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/history/{id}/receipt\n  method: get\n  operationId: getReceiptPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/payment-methods\n  method: get\n  operationId: listPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/payment-methods/portal-url\n  method: get\n  operationId: getBillingPortalUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/payment-methods/{id}\n  method: delete\n  operationId: deletePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/payment-methods/{id}/default\n  method: patch\n  operationId: setDefaultPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orgs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/read\n  method: post\n  operationId: markNotificationsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs\n  method: get\n  operationId: listOrgs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs\n  method: post\n  operationId: createOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current\n  method: get\n  operationId: getCurrentOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/current\n  method: patch\n  operationId: updateOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current\n  method: delete\n  operationId: deleteOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/exit-feedback\n  method: post\n  operationId: sendExitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/settings\n  method: get\n  operationId: getOrgSettings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orgs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/current/settings\n  method: patch\n  operationId: updateOrgSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/callback-secret\n  method: get\n  operationId: getCallbackSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/current/callback-secret/rotate\n  method: post\n  operationId: rotateCallbackSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/audit-log\n  method: get\n  operationId: listOrgAuditLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orgs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/current/members\n  method: post\n  operationId: inviteOrgMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/members/{memberId}\n  method: patch\n  operationId: updateOrgMemberRole\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/members/{memberId}\n  method: delete\n  operationId: removeOrgMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/current/invitations/{invitationId}\n  method: delete\n  operationId: revokeOrgInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/capabilities\n  method: get\n  operationId: getAccountCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - keys:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - keys:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys/{id}\n  method: delete\n  operationId:\
  \ revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - keys:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api-keys/{id}\n  method: patch\n  operationId: updateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - keys:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/templates\n  method: get\n  operationId: listAssetTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{id}/complete\n  method: post\n  operationId: completeAssetUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{id}/download\n  method: get\n  operationId: downloadAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/content\n  method: get\n  operationId: getAssetContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/preview\n  method: get\n  operationId: getAssetPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/invite\n  method: post\n  operationId: inviteTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/role\n  method: patch\n  operationId: updateTeamMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/remove\n  method: post\n  operationId: removeTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/revoke-invitation\n  method: post\n  operationId: revokeTeamInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - orgs:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /webhooks/endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints/{id}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints/{id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{id}/secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /webhooks/endpoints/{id}/test\n  method: post\n  operationId: testWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/deliveries/{id}/retry\n  method: post\n  operationId: retryWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage\n  method: post\n  operationId: createStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage\n  method: get\n  operationId: listStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/s3/bucket\n  method: get\n  operationId: lookUpS3Bucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:write\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /storage/buckets\n  method: get\n  operationId: listAccountBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/aws/prepare\n  method: post\n  operationId: prepareAwsStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/supabase/start\n  method: post\n  operationId: startSupabaseStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /storage/supabase/sessions/{state}\n  method: get\n  operationId: getSupabaseSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/supabase/sessions/{state}/projects/{projectRef}/buckets\n  method: get\n  operationId: listSupabaseBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/supabase/finish\n  method: post\n  operationId: finishSupabaseStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /storage/{id}\n  method: get\n  operationId: getStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/{id}\n  method: patch\n  operationId: updateStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/{id}\n  method: delete\n  operationId: deleteStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /storage/{id}/test\n  method: post\n  operationId: testStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/{id}/stats\n  method: get\n  operationId: getStorageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/{id}/objects\n  method: get\n  operationId: listStorageObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload-sessions/{token}\n  method: get\n  operationId:\
  \ getUploadSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload-sessions/{token}/files\n  method: post\n  operationId: addUploadSessionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload-sessions/{token}/files/{assetId}/complete\n  method: post\n  operationId: completeUploadSessionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload-sessions/{token}/done\n  method: post\n  operationId:\
  \ completeUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/rendobar-com/agentic-access/rendobar-com-agentic-access.yml
summary_line: 101 operations · 51 acting · 3 human-in-the-loop
tags:
- Company
- Video Processing
- FFmpeg
- Artificial Intelligence
- Serverless
- Media API
---
