---
acting_count: 108
action_class_counts:
  acting: 108
  connected: 164
api_specs:
- filename: decisiv-account-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Account Management
  slug: decisiv-srm-gateway-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-account-management-openapi.yml
- filename: decisiv-asset-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Asset Management
  slug: decisiv-srm-gateway-asset-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-asset-management-openapi.yml
- filename: decisiv-service-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Service Management
  slug: decisiv-srm-gateway-service-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-management-openapi.yml
- filename: decisiv-telematics-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Telematics
  slug: decisiv-srm-gateway-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-telematics-openapi.yml
- filename: decisiv-global-assets-openapi.yml
  format: yaml
  label: Decisiv Global Assets API
  slug: decisiv-global-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-global-assets-openapi.yml
- filename: decisiv-service-provider-openapi.yml
  format: yaml
  label: Decisiv Service Provider API
  slug: decisiv-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-provider-openapi.yml
consequence_counts:
  physical: 19
  read: 164
  write: 89
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Decisiv Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account_management/v1/accounts/{account_id}/users/{account_user_id}/relationships/roles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /account_management/v1/accounts/{account_id}/users/{account_user_id}/relationships/roles/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /asset_management/{srm_account_id}/v1/cases/{case_id}/relationships/billing_contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /asset_management/{srm_account_id}/v1/cases/{case_id}/relationships/primary_contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /asset_management/{srm_account_id}/v1/cases/{case_id}/send_note_to_provider
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /asset_management/{srm_account_id}/v1/registered_components/{component_id}/relationships/registered_asset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/line_items/{line_item_id}/parts/{part_id}/relationships/salesperson
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/line_items/{line_item_id}/relationships/assignee
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/billing_contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/billing_customer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/driver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/primary_contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/program_type
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_id}/relationships/shipping_customer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service_management/{srm_account_id}/v1/cases/{case_uuid}/line_items/{line_item_uuid}/additional_charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_uuid}/line_items/{line_item_uuid}/additional_charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /service_management/{srm_account_id}/v1/cases/{case_uuid}/line_items/{line_item_uuid}/additional_charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /service_management/{srm_account_id}/v1/cases/{case_uuid}/line_items/{line_item_uuid}/additional_charges/{id}/relationships/category
operation_count: 272
overview: 'Decisiv exposes 272 API operations that an AI agent could call, of which 108 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 164 read, 89 write, and 19 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Decisiv
provider_slug: decisiv
slug: decisiv-agentic-access
source_filename: decisiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/decisiv-account-management-openapi.yml, openapi/decisiv-asset-management-openapi.yml,\n  openapi/decisiv-global-assets-openapi.yml, openapi/decisiv-service-management-openapi.yml,\n  openapi/decisiv-service-provider-openapi.yml, openapi/decisiv-telematics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 272\n  by_action_class:\n    connected: 164\n    acting: 108\n  by_consequence:\n    read: 164\n    write: 89\n    physical: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /account_management/v1/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}\n  method: get\n  operationId: getAccountsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/ecosystem_users\n  method: get\n  operationId: listEcosystemUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/ecosystem_users\n  method: post\n  operationId: createEcosystemUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/ecosystem_users/{id}\n\
  \  method: get\n  operationId: getEcosystemUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/users\n  method: get\n  operationId: listAccountUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/users\n  method: post\n  operationId: createAccountUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/users/{id}\n  method: get\n  operationId: getAccountUser\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/users/{id}\n  method: patch\n  operationId: updateAccountUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/users/{id}\n  method: delete\n  operationId: deleteAccountUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/users/{account_user_id}/relationships/roles\n  method: post\n  operationId:\
  \ addAccountUserRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/users/{account_user_id}/relationships/roles/{id}\n  method: delete\n  operationId: deleteAccountUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/roles\n  method: get\n  operationId: listAccountRoles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/roles/{id}\n  method: get\n  operationId: getAccountRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/webhooks\n  method: post\n  operationId: createWebhookByAccountId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /account_management/v1/accounts/{account_id}/webhooks/{id}\n  method: get\n  operationId: getWebhooksById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_management/v1/accounts/{account_id}/webhooks/{id}\n  method: patch\n  operationId: updateWebhookbyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/webhooks/{id}\n  method: delete\n  operationId: deleteWebhooksbyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/webhooks/{id}/refresh_signing_key\n  method: post\n  operationId: refreshSigningKeyWebhooksbyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_management/v1/accounts/{account_id}/webhook_events\n  method: get\n  operationId: getWebhooksEventsbyAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/case_summaries\n  method: get\n  operationId: listCaseSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{id}\n  method: get\n  operationId: getCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{id}\n  method: patch\n  operationId: updateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/attachments\n  method: get\n  operationId: listCaseAttachments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/attachments\n  method: post\n  operationId: createCaseAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/attachments/{id}\n  method: get\n  operationId: getCaseAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/attachments/{id}\n  method: delete\n  operationId: deleteCaseAttachment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/contacts/{id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/contacts/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/notes\n  method: get\n  operationId: listCaseNotes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/notes\n  method: post\n  operationId: createCaseNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/notes/{id}\n  method: get\n  operationId: getCaseNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/send_note_to_provider\n  method: post\n  operationId: sendNoteToProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/participants\n  method: get\n  operationId: listCaseParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/participants/{id}\n  method: get\n  operationId: getCaseParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/participants/{participant_id}/recipients\n  method: get\n  operationId: listCaseParticipantRecipients\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/participants/{participant_id}/recipients/{id}\n  method: get\n  operationId: getCaseParticipantRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/recipients\n  method: get\n  operationId: listCaseRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/recipients/{id}\n  method: get\n  operationId: getCaseRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/relationships/primary_contact\n\
  \  method: patch\n  operationId: updateCasePrimaryContact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/cases/{case_id}/relationships/billing_contact\n  method: patch\n  operationId: updateCaseBillingContact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/deactivated_assets\n  method: get\n  operationId: listDeactivatedAssets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/deactivated_assets/{id}\n  method: get\n  operationId: getDeactivatedAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/deactivated_depots\n  method: get\n  operationId: listDeactivatedDepots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/deactivated_depots/{id}\n  method: get\n  operationId: getDeactivatedDepot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/deactivated_depots/{id}/activate\n\
  \  method: post\n  operationId: activateDeactivatedDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/depots\n  method: get\n  operationId: listDepots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/depots\n  method: post\n  operationId: createDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/depots/{id}\n\
  \  method: get\n  operationId: getDepot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/depots/{id}\n  method: patch\n  operationId: updateDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/depots/{id}/deactivate\n  method: post\n  operationId: deactivateDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/estimates\n\
  \  method: get\n  operationId: listEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/estimates/{id}\n  method: get\n  operationId: getEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/estimates/{id}/respond\n  method: post\n  operationId: respondToEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/deactivated_assets/{id}/activate\n  method: post\n  operationId: activateDeactivatedAsset\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/extended_attributes\n  method: get\n  operationId: listExtendedAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/extended_attributes/{id}\n  method: get\n  operationId: getExtendedAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/extended_asset_attributes\n  method: get\n  operationId: listExtendedAssetAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/extended_asset_attributes\n  method: post\n  operationId: createExtendedAssetAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/extended_asset_attributes/{id}\n  method: get\n  operationId: getExtendedAssetAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/extended_asset_attributes/{id}\n  method: patch\n  operationId: updateExtendedAssetAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/extended_asset_attributes/{id}\n  method: delete\n  operationId: deleteExtendedAssetAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/internal_users\n  method: get\n  operationId: listInternalUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/internal_users/{id}\n  method: get\n  operationId: getInternalUser\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets\n  method: get\n  operationId: listRegisteredAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets\n  method: post\n  operationId: createRegisteredAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}\n  method: get\n  operationId: getRegisteredAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}\n  method: patch\n  operationId: updateRegisteredAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/deactivate\n  method: post\n  operationId: deactivateRegisteredAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/metadata\n  method: delete\n  operationId: deleteRegisteredAssetMetadata\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/metadata/{metadata_key}\n  method: delete\n  operationId: deleteRegisteredAssetMetadataKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/update_meter_data\n  method: post\n  operationId: asset_management_ra_update_meter_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/meter_data_history\n  method: get\n  operationId: asset_management_ra_meter_data_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/transfer\n  method: post\n  operationId: transferRegisteredAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{id}/build_information\n  method:\
  \ get\n  operationId: getBuildInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{registered_asset_id}/attachments\n  method: get\n  operationId: listRegisteredAssetAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{registered_asset_id}/attachments\n  method: post\n  operationId: createRegisteredAssetAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{registered_asset_id}/attachments/{id}\n\
  \  method: get\n  operationId: getRegisteredAssetAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_assets/{registered_asset_id}/attachments/{id}\n  method: delete\n  operationId: deleteRegisteredAssetAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_components\n  method: get\n  operationId: listRegisteredComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_components\n  method:\
  \ post\n  operationId: createRegisteredComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_components/{id}\n  method: get\n  operationId: getRegisteredComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/registered_components/{id}\n  method: patch\n  operationId: updateRegisteredComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /asset_management/{srm_account_id}/v1/registered_components/{id}\n  method: delete\n  operationId: deleteRegisteredComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/registered_components/{component_id}/relationships/registered_asset\n  method: patch\n  operationId: updateRegisteredComponentRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/service_providers\n\
  \  method: get\n  operationId: listServiceProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/service_providers/{id}\n  method: get\n  operationId: getServiceProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/service_requests\n  method: get\n  operationId: listServiceRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/service_requests\n  method: post\n  operationId: createServiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/service_requests/{id}\n  method: get\n  operationId: getServiceRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/service_requests/{id}\n  method: put\n  operationId: updateServiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/service_requests/{id}/cancel\n  method: post\n  operationId: cancelServiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_management/{srm_account_id}/v1/vmrs/asset_types\n  method: get\n  operationId: listVmrsAssetTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/vmrs/reasons_for_repair\n  method: get\n  operationId: listVmrsReasonsForRepair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_management/{srm_account_id}/v1/vmrs/repair_priorities\n  method: get\n  operationId: listVmrsRepairPriorities\n  x-agen\n\n# --- truncated at 32 KB (80 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/agentic-access/decisiv-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/agentic-access/decisiv-agentic-access.yml
summary_line: 272 operations · 108 acting
tags:
- Company
- commercial-vehicle
- fleet-management
- service-relationship-management
- telematics
- asset-management
- maintenance-and-repair
- heavy-duty-trucking
- transportation
- dealer-management
- json-api
- webhooks
---
