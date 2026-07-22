---
acting_count: 287
action_class_counts:
  acting: 287
  connected: 151
api_specs:
- filename: solvimon-configuration-api-openapi.yml
  format: yaml
  label: Solvimon Configuration API
  slug: solvimon-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-configuration-api-openapi.yml
- filename: solvimon-transaction-api-openapi.yml
  format: yaml
  label: Solvimon Transaction API
  slug: solvimon-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-transaction-api-openapi.yml
- filename: solvimon-identity-api-openapi.yml
  format: yaml
  label: Solvimon Identity API
  slug: solvimon-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-identity-api-openapi.yml
- filename: solvimon-event-api-openapi.yml
  format: yaml
  label: Solvimon Event API
  slug: solvimon-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-event-api-openapi.yml
consequence_counts:
  physical: 52
  read: 151
  safety-critical: 4
  write: 231
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Solvimon Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v{version}/oauth/request-password-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v{version}/oauth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v{version}/portal-urls/{resourceId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v{version}/users/revoke-invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/charge-on-demand-pricing-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v{version}/invoices/{resourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/add-line
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/archive
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/cancel-dunning-actions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/credit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/credit_and_copy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/delete-line
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/export_to_erp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/lines
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v{version}/invoices/{resourceId}/lines/{invoiceLineResourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v{version}/invoices/{resourceId}/lines/{invoiceLineResourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/refresh
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/refresh-e-invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/resubmit-e-invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v{version}/invoices/{resourceId}/send_by_email
operation_count: 438
overview: 'Solvimon exposes 438 API operations that an AI agent could call, of which 287 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 151 read, 231 write, 52 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Solvimon
provider_slug: solvimon
slug: solvimon-agentic-access
source_filename: solvimon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/solvimon-configuration-api-openapi.yml, openapi/solvimon-event-api-openapi.yml,\n  openapi/solvimon-identity-api-openapi.yml, openapi/solvimon-transaction-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 438\n  by_action_class:\n    connected: 151\n    acting: 287\n  by_consequence:\n    read: 151\n    write: 231\n    physical: 52\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v{version}/attachments\n  method: get\n  operationId: getAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/attachments\n  method: post\n\
  \  operationId: postAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/attachments/{resourceId}\n  method: get\n  operationId: getAttachmentsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/attachments/{resourceId}\n  method: delete\n  operationId: deleteAttachmentsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/documents\n  method: post\n  operationId:\
  \ postDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/documents/{resourceId}\n  method: get\n  operationId: getDocumentsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/documents/{resourceId}\n  method: delete\n  operationId: deleteDocumentsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/documents/{resourceId}/download\n  method: post\n  operationId:\
  \ postDocumentsByResourceIdDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/customers\n  method: post\n  operationId: postCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers\n  method: put\n  operationId: putCustomers\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}\n  method: get\n  operationId: getCustomersByResourceIdOrReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/customers/{resourceIdOrReference}\n  method: delete\n  operationId: deleteCustomersByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}\n  method: patch\n  operationId:\
  \ patchCustomersByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}/entitlements\n  method: get\n  operationId: getCustomersByResourceIdOrReferenceEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/customers/{resourceIdOrReference}/activate\n  method: post\n  operationId: postCustomersByResourceIdOrReferenceActivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}/deprecate\n  method: post\n  operationId: postCustomersByResourceIdOrReferenceDeprecate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}/archive\n  method: post\n  operationId: postCustomersByResourceIdOrReferenceArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}/forget\n  method: post\n  operationId: postCustomersByResourceIdOrReferenceForget\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/{resourceIdOrReference}/wallets/balance\n  method: post\n  operationId: postCustomersByResourceIdOrReferenceWalletsBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/search\n  method: post\n  operationId: postCustomersSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/customers/validate-tax-id\n  method: post\n  operationId: postCustomersValidateTaxId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/custom-fields\n  method: get\n  operationId: getCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/custom-fields\n  method: post\n  operationId: postCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v{version}/custom-fields/{resourceId}\n  method: get\n  operationId: getCustomFieldsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/custom-fields/{resourceId}\n  method: delete\n  operationId: deleteCustomFieldsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/custom-fields/{resourceId}\n  method: patch\n  operationId: patchCustomFieldsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/contacts\n  method: post\n  operationId: postContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/contacts\n  method: put\n  operationId: putContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/contacts/{resourceId}\n\
  \  method: get\n  operationId: getContactsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/contacts/{resourceId}\n  method: delete\n  operationId: deleteContactsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/contacts/{resourceId}\n  method: patch\n  operationId: patchContactsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/alert-rules\n  method:\
  \ get\n  operationId: getAlertRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/alert-rules\n  method: post\n  operationId: postAlertRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/alert-rules/{resourceId}\n  method: get\n  operationId: getAlertRulesByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/alert-rules/{resourceId}\n  method: delete\n  operationId: deleteAlertRulesByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/alert-rules/{resourceId}\n  method: patch\n  operationId: patchAlertRulesByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/platforms/{resourceId}\n  method: get\n  operationId: getPlatformsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/platforms/{resourceId}\n  method: patch\n  operationId: patchPlatformsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/platforms/{resourceId}/entitlements\n  method: get\n  operationId: getPlatformsByResourceIdEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/platforms/{resourceId}/currencies\n  method: get\n  operationId: getPlatformsByResourceIdCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/platforms/{resourceId}/up-to-date\n  method: get\n  operationId: getPlatformsByResourceIdUpToDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meters\n\
  \  method: get\n  operationId: getMeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meters\n  method: post\n  operationId: postMeters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meters/{resourceIdOrReference}\n  method: get\n  operationId: getMetersByResourceIdOrReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meters/{resourceIdOrReference}\n  method: delete\n  operationId: deleteMetersByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meters/{resourceIdOrReference}\n  method: patch\n  operationId: patchMetersByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meters/{resourceIdOrReference}/meter-data-file\n  method: get\n  operationId: getMetersByResourceIdOrReferenceMeterDataFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-values\n  method: get\n  operationId: getMeterValues\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-values\n  method: post\n  operationId: postMeterValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-values/{resourceIdOrReference}\n  method: get\n  operationId: getMeterValuesByResourceIdOrReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-values/{resourceIdOrReference}\n  method: delete\n  operationId: deleteMeterValuesByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-values/{resourceIdOrReference}\n  method: patch\n  operationId: patchMeterValuesByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-properties\n  method: get\n  operationId: getMeterProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-properties\n  method: post\n  operationId: postMeterProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-properties/{resourceIdOrReference}\n  method: get\n  operationId: getMeterPropertiesByResourceIdOrReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-properties/{resourceIdOrReference}\n  method: delete\n  operationId: deleteMeterPropertiesByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-properties/{resourceIdOrReference}\n  method: patch\n  operationId: patchMeterPropertiesByResourceIdOrReference\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-value-calculations\n  method: get\n  operationId: getMeterValueCalculations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-value-calculations\n  method: post\n  operationId: postMeterValueCalculations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-value-calculations/{resourceId}\n  method: get\n  operationId: getMeterValueCalculationsByResourceId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/meter-value-calculations/{resourceId}\n  method: delete\n  operationId: deleteMeterValueCalculationsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/meter-value-calculations/{resourceId}\n  method: patch\n  operationId: patchMeterValueCalculationsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plans\n\
  \  method: get\n  operationId: getPricingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-plans\n  method: post\n  operationId: postPricingPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plans\n  method: put\n  operationId: putPricingPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plans/search\n  method: post\n  operationId: postPricingPlansSearch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plans/{resourceIdOrReference}\n  method: get\n  operationId: getPricingPlansByResourceIdOrReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-plans/{resourceIdOrReference}\n  method: delete\n  operationId: deletePricingPlansByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plans/{resourceIdOrReference}\n\
  \  method: patch\n  operationId: patchPricingPlansByResourceIdOrReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-versions/{resourceId}\n  method: get\n  operationId: getPricingPlanVersionsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-plan-versions/{resourceId}\n  method: delete\n  operationId: deletePricingPlanVersionsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v{version}/pricing-plan-versions/{resourceId}\n  method: patch\n  operationId: patchPricingPlanVersionsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-versions\n  method: post\n  operationId: postPricingPlanVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-versions\n  method: put\n  operationId: putPricingPlanVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricings\n  method: post\n  operationId: postPricings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricings/{resourceId}\n  method: delete\n  operationId: deletePricingsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricings/{resourceId}\n  method: patch\n  operationId: patchPricingsByResourceId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-groups\n  method: post\n  operationId: postPricingGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-groups/{resourceId}\n  method: get\n  operationId: getPricingGroupsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-groups/{resourceId}\n  method: delete\n  operationId: deletePricingGroupsByResourceId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-groups/{resourceId}\n  method: patch\n  operationId: patchPricingGroupsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions\n  method: get\n  operationId: getPricingPlanSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-plan-subscriptions\n  method: post\n  operationId:\
  \ postPricingPlanSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions\n  method: put\n  operationId: putPricingPlanSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/init\n  method: post\n  operationId: postPricingPlanSubscriptionsInit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/search\n  method: post\n  operationId: postPricingPlanSubscriptionsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}\n  method: get\n  operationId: getPricingPlanSubscriptionsByResourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}\n  method: delete\n  operationId: deletePricingPlanSubscriptionsByResourceId\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}\n  method: patch\n  operationId: patchPricingPlanSubscriptionsByResourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}/void\n  method: post\n  operationId: postPricingPlanSubscriptionsByResourceIdVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}/archive\n  method: post\n  operationId: postPricingPlanSubscriptionsByResourceIdArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}/cancel\n  method: post\n  operationId: postPricingPlanSubscriptionsByResourceIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}/copy\n  method: post\n  operationId:\
  \ postPricingPlanSubscriptionsByResourceIdCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscriptions/{resourceId}/update-payment-method\n  method: post\n  operationId: postPricingPlanSubscriptionsByResourceIdUpdatePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v{version}/pricing-plan-subscription-groups\n  method: get\n  operationId: getPricingPlanSubscriptionGroups\n  x-agentic-access:\n    acti\n\n# --- truncated at\
  \ 32 KB (143 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/agentic-access/solvimon-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/agentic-access/solvimon-agentic-access.yml
summary_line: 438 operations · 287 acting · 4 human-in-the-loop
tags:
- Company
- Fintech
- Billing
- Payments
- Monetization
- Usage-Based Pricing
- Subscriptions
- Invoicing
- Metering
- Revenue Recognition
---
