---
acting_count: 64
action_class_counts:
  acting: 64
  connected: 47
api_specs:
- filename: notarize-cost-centers-api-openapi.yml
  format: yaml
  label: Notarize Cost Centers API
  slug: notarize-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-cost-centers-api-openapi.yml
- filename: notarize-documents-api-openapi.yml
  format: yaml
  label: Notarize Documents API
  slug: notarize-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-documents-api-openapi.yml
- filename: notarize-eligibilities-api-openapi.yml
  format: yaml
  label: Notarize Eligibilities API
  slug: notarize-eligibilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-eligibilities-api-openapi.yml
- filename: notarize-enote-api-openapi.yml
  format: yaml
  label: Notarize E Note API
  slug: notarize-enote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-enote-api-openapi.yml
- filename: notarize-integrations-api-openapi.yml
  format: yaml
  label: Notarize Integrations API
  slug: notarize-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-integrations-api-openapi.yml
- filename: notarize-notaries-api-openapi.yml
  format: yaml
  label: Notarize Notaries API
  slug: notarize-notaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notaries-api-openapi.yml
- filename: notarize-notarization-records-api-openapi.yml
  format: yaml
  label: Notarize Notarization Records API
  slug: notarize-notarization-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notarization-records-api-openapi.yml
- filename: notarize-oauth-2-0-api-openapi.yml
  format: yaml
  label: Notarize OAuth 2.0 API
  slug: notarize-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oauth-2-0-api-openapi.yml
- filename: notarize-oid4vp-api-openapi.yml
  format: yaml
  label: Notarize OID4VP API
  slug: notarize-oid4vp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oid4vp-api-openapi.yml
- filename: notarize-organizations-api-openapi.yml
  format: yaml
  label: Notarize Organizations API
  slug: notarize-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-organizations-api-openapi.yml
- filename: notarize-referrals-api-openapi.yml
  format: yaml
  label: Notarize Referrals API
  slug: notarize-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-referrals-api-openapi.yml
- filename: notarize-scim-api-openapi.yml
  format: yaml
  label: Notarize SCIM API
  slug: notarize-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-scim-api-openapi.yml
- filename: notarize-security-events-api-openapi.yml
  format: yaml
  label: Notarize Security Events API
  slug: notarize-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-security-events-api-openapi.yml
- filename: notarize-templates-api-openapi.yml
  format: yaml
  label: Notarize Templates API
  slug: notarize-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-templates-api-openapi.yml
- filename: notarize-title-agencies-api-openapi.yml
  format: yaml
  label: Notarize Title Agencies API
  slug: notarize-title-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-title-agencies-api-openapi.yml
- filename: notarize-transactions-api-openapi.yml
  format: yaml
  label: Notarize Transactions API
  slug: notarize-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-transactions-api-openapi.yml
- filename: notarize-webhooks-api-openapi.yml
  format: yaml
  label: Notarize Webhooks API
  slug: notarize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 47
  safety-critical: 1
  write: 57
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Notarize Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/v2/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mortgage/v2/transactions/{id}/place_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mortgage/v2/transactions/{id}/send_contacts_email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mortgage/v2/transactions/{id}/send_email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mortgage/v2/transactions/{id}/send_sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/{id}/send_email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/{id}/send_sms
operation_count: 111
overview: 'Notarize exposes 111 API operations that an AI agent could call, of which 64 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read, 57 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Notarize
provider_slug: notarize
slug: notarize-agentic-access
source_filename: notarize-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/notarize-logs-api-specification-openapi.yml, openapi/notarize-oauth-2-0-api-specification-openapi.yml,\n  openapi/notarize-proof-business-api-specification-openapi.yml, openapi/notarize-proof-real-estate-api-specification-openapi.yml,\n  openapi/notarize-proof-verifiable-credentials-api-specification-openapi.yml, openapi/notarize-scim-api-specification-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 111\n  by_action_class:\n    connected: 47\n    acting: 64\n  by_consequence:\n    read: 47\n    write: 57\n    safety-critical: 1\n    physical: 6\n  human_in_the_loop_required: 1\noperations:\n- path: /logs/v1/security-events\n  method: get\n  operationId: listSecurityEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuthAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/v2/authorize\n  method: get\n  operationId: authorizeOAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/v2/introspect\n  method: post\n  operationId: introspectOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/v2/register\n\
  \  method: post\n  operationId: registerOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/v2/revoke\n  method: post\n  operationId: revokeOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/v2/token\n  method: post\n  operationId: createOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/v2/token/info\n  method: get\n  operationId: getOAuthTokenInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cost_centers\n  method: get\n  operationId: getAllCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}\n  method: put\n  operationId: updateDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}\n  method: patch\n  operationId: patchDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations\n  method: post\n  operationId: createIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notaries/\n  method: post\n  operationId: createNotary\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notaries/\n  method: get\n  operationId: getAllNotaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notaries/{id}\n  method: get\n  operationId: getNotary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notaries/{id}\n  method: delete\n  operationId: deleteNotary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/notarization_records\n  method: get\n  operationId: getNotarizationRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notarization_records/{id}\n  method: get\n  operationId: getNotarizationRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization\n  method: get\n  operationId: getOrganizationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{organization_id}/transactions/identity\n  method: post\n  operationId: createOpenIdConnectTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partners\n  method: post\n  operationId: createPartnerOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partners/{id}\n  method: patch\n  operationId: updatePartnerOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/referrals\n  method: post\n  operationId: createReferral\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/referrals/{referral_campaign_id}/generate_link\n  method: post\n  operationId: generateReferralCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: getAllTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: get\n  operationId: getAllTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}\n  method: put\n  operationId: updateDraftTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}\n\
  \  method: patch\n  operationId: patchDraftTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}\n  method: delete\n  operationId: deleteTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/assets/audit_trail\n  method: get\n  operationId: getAuditTrail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}/cancel\n  method: post\n  operationId:\
  \ cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/documents\n  method: post\n  operationId: addDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/documents/{document_id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}/force_complete\n  method: post\n  operationId: forceCompleteTransaction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/notaries\n  method: get\n  operationId: getAllEligibleNotaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}/notarization_ready\n  method: post\n  operationId: activateDraftTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/recall\n  method: post\n  operationId: recallTransaction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/send_email\n  method: post\n  operationId: resendTransactionEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}/send_sms\n  method: post\n  operationId: resendTransactionSMS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_tests\n  method: post\n  operationId: createTestWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: getWebhookURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhookURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/webhooks\n  method: delete\n  operationId: deleteWebhookURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks\n  method: get\n  operationId: getAllWebhooksV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: createWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/subscriptions\n  method: get\n  operationId:\
  \ getWebhookSubscriptionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: get\n  operationId: getWebhookV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: put\n  operationId: updateWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}\n  method: delete\n  operationId: deleteWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}/events\n  method: get\n  operationId: getWebhookEventsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v1/cost_centers\n  method: get\n  operationId: getAllRealEstateCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v1/notaries/\n  method: post\n  operationId: createMortgageNotary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v1/notaries/\n  method: get\n  operationId: getAllMortgageNotaries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v1/notaries/{id}\n  method: get\n  operationId: getMortgageNotary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v1/notaries/{id}\n  method: delete\n  operationId: deleteMortgageNotary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v1/webhook_tests\n  method: post\n  operationId: createTestWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v1/webhooks\n  method: get\n  operationId: getMortgageWebhookURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v1/webhooks\n  method: post\n  operationId: createMortgageWebhookURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v1/webhooks\n  method: delete\n  operationId: deleteMortgageWebhookURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/documents/{id}\n  method: put\n  operationId: updateMortgageDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/documents/{id}\n  method: patch\n  operationId: patchMortgageDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/documents/{id}\n  method: delete\n  operationId: deleteMortgageDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/notarization_records/{id}\n  method: get\n  operationId: getMortgageNotarizationRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/partners\n  method: post\n  operationId: createMortgagePartnerOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/partners/{id}\n  method: patch\n  operationId: updateMortgagePartnerOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/recording_locations\n  method: get\n  operationId: getRecordingLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/templates\n  method: get\n  operationId: getAllRealEstateTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/title_agencies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions\n  method: get\n  operationId: getAllMortgageTransactions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions\n  method: post\n  operationId: createMortgageTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/title_underwriters\n  method: get\n  operationId: getValidUnderwriters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions/verify_address\n  method: get\n  operationId: verifyPropertyAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions/{id}\n\
  \  method: get\n  operationId: getMortgageTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions/{id}\n  method: put\n  operationId: updateMortgageTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}\n  method: delete\n  operationId: deleteMortgageTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/cancel\n\
  \  method: post\n  operationId: cancelMortgageTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/documents\n  method: post\n  operationId: addMortgageDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/documents/{document_id}\n  method: get\n  operationId: getMortgageDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions/{id}/enote\n\
  \  method: post\n  operationId: addEnote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/enote\n  method: delete\n  operationId: deleteEnote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/force_complete\n  method: post\n  operationId: forceCompleteTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/notaries\n  method: get\n  operationId: getAllEligibleNotaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/transactions/{id}/place_order\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/recall\n  method: post\n  operationId: recallTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/send_contacts_email\n  method: post\n  operationId: resendMortgageContactsEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{id}/send_email\n  method: post\n  operationId: resendMortgageTransactionEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /mortgage/v2/transactions/{id}/send_sms\n  method: post\n  operationId: resendMortgageTransactionSMS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/transactions/{transaction_id}/documents/external\n  method: post\n  operationId: addMortgageExternalDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/webhooks\n  method: get\n  operationId: getAllMortgageWebhooksV2\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/webhooks\n  method: post\n  operationId: createMortgageWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/webhooks/subscriptions\n  method: get\n  operationId: getMortgageWebhookSubscriptionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/webhooks/{id}\n  method: get\n  operationId: getMortgageWebhookV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mortgage/v2/webhooks/{id}\n  method: put\n\
  \  operationId: updateMortgageWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/webhooks/{id}\n  method: delete\n  operationId: deleteMortgageWebhookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mortgage/v2/webhooks/{id}/events\n  method: get\n  operationId: getMortgageWebhookEventsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifiable-credentials/v1/presentation/authorize\n  method:\
  \ get\n  operationId: authorizeVerifiableCredentialPresentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifiable-credentials/v1/x401-handoff\n  method: post\n  operationId: createPresentationX401Handoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifiable-credentials/v1/x401-result/{id}\n  method: get\n  operationId: getX401Result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifiable-credentials/v1/x401-signatures\n  method: post\n  operationId: getX401Signatures\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v1/organizations/{organization_id}/ResourceTypes\n  method: get\n  operationId: resourceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v1/organizations/{organization_id}/Schemas/Users\n  method: get\n  operationId: userSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v1/organizations/{organization_id}/ServiceProviderConfig\n  method: get\n  operationId: serviceProviderConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/agentic-access/notarize-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/agentic-access/notarize-agentic-access.yml
summary_line: 111 operations · 64 acting · 1 human-in-the-loop
tags:
- Company
- PropTech
- Notarization
- Remote Online Notarization
- Identity Verification
- E-Signature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
---
