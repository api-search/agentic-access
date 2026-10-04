---
acting_count: 88
action_class_counts:
  acting: 88
  connected: 59
api_specs:
- filename: portone-banks-api-openapi.yml
  format: yaml
  label: PortOne Banks API
  slug: portone-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-banks-api-openapi.yml
- filename: portone-billing-keys-api-openapi.yml
  format: yaml
  label: PortOne Billing Keys API
  slug: portone-billing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-billing-keys-api-openapi.yml
- filename: portone-cash-receipts-api-openapi.yml
  format: yaml
  label: PortOne Cash Receipts API
  slug: portone-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-cash-receipts-api-openapi.yml
- filename: portone-checkout-profiles-api-openapi.yml
  format: yaml
  label: PortOne Checkout Profiles API
  slug: portone-checkout-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-checkout-profiles-api-openapi.yml
- filename: portone-identity-verifications-api-openapi.yml
  format: yaml
  label: PortOne Identity Verifications API
  slug: portone-identity-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-identity-verifications-api-openapi.yml
- filename: portone-kakaopay-api-openapi.yml
  format: yaml
  label: PortOne Kakaopay API
  slug: portone-kakaopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-kakaopay-api-openapi.yml
- filename: portone-login-api-openapi.yml
  format: yaml
  label: PortOne Login API
  slug: portone-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-login-api-openapi.yml
- filename: portone-payment-events-by-cursor-api-openapi.yml
  format: yaml
  label: PortOne Payment Events By Cursor API
  slug: portone-payment-events-by-cursor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-events-by-cursor-api-openapi.yml
- filename: portone-payment-gateways-api-openapi.yml
  format: yaml
  label: PortOne Payment Gateways API
  slug: portone-payment-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-gateways-api-openapi.yml
- filename: portone-payment-reconciliations-api-openapi.yml
  format: yaml
  label: PortOne Payment Reconciliations API
  slug: portone-payment-reconciliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-reconciliations-api-openapi.yml
- filename: portone-payment-schedules-api-openapi.yml
  format: yaml
  label: PortOne Payment Schedules API
  slug: portone-payment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-schedules-api-openapi.yml
- filename: portone-payment-sessions-api-openapi.yml
  format: yaml
  label: PortOne Payment Sessions API
  slug: portone-payment-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payment-sessions-api-openapi.yml
- filename: portone-payments-api-openapi.yml
  format: yaml
  label: PortOne Payments API
  slug: portone-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payments-api-openapi.yml
- filename: portone-payments-by-cursor-api-openapi.yml
  format: yaml
  label: PortOne Payments By Cursor API
  slug: portone-payments-by-cursor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-payments-by-cursor-api-openapi.yml
- filename: portone-paymentwall-api-openapi.yml
  format: yaml
  label: PortOne Paymentwall API
  slug: portone-paymentwall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-paymentwall-api-openapi.yml
- filename: portone-platform-api-openapi.yml
  format: yaml
  label: PortOne Platform API
  slug: portone-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-platform-api-openapi.yml
- filename: portone-promotions-api-openapi.yml
  format: yaml
  label: PortOne Promotions API
  slug: portone-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-promotions-api-openapi.yml
- filename: portone-token-api-openapi.yml
  format: yaml
  label: PortOne Token API
  slug: portone-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-token-api-openapi.yml
- filename: portone-b2-b-api-openapi.yml
  format: yaml
  label: PortOne B2 B API
  slug: portone-b2-b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-b2-b-api-openapi.yml
consequence_counts:
  physical: 37
  read: 59
  safety-critical: 2
  write: 49
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Portone Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /payment-schedules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /payments/{paymentId}/cancellations/{cancellationId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /b2b/tax-invoices/draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/issue-immediately
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/request-reverse-issuance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /b2b/tax-invoices/{taxInvoiceKey}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/attach-file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /b2b/tax-invoices/{taxInvoiceKey}/attachments/{attachmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/cancel-issuance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/cancel-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/issue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/refuse-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /b2b/tax-invoices/{taxInvoiceKey}/send-to-nts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /identity-verifications/{identityVerificationId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /identity-verifications/{identityVerificationId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-sessions/{sessionId}/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/billing-key
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/cash-receipt/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/escrow/complete
operation_count: 147
overview: 'PortOne exposes 147 API operations that an AI agent could call, of which 88 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 59 read, 49 write, 37 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PortOne
provider_slug: portone
slug: portone-agentic-access
source_filename: portone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/portone-b2-b-api-openapi.yml, openapi/portone-banks-api-openapi.yml, openapi/portone-billing-keys-api-openapi.yml,\n  openapi/portone-cash-receipts-api-openapi.yml, openapi/portone-checkout-profiles-api-openapi.yml,\n  openapi/portone-identity-verifications-api-openapi.yml, openapi/portone-kakaopay-api-openapi.yml,\n  openapi/portone-login-api-openapi.yml, openapi/portone-payment-events-by-cursor-api-openapi.yml,\n  openapi/portone-payment-gateways-api-openapi.yml, openapi/portone-payment-reconciliations-api-openapi.yml,\n  openapi/portone-payment-schedules-api-openapi.yml, openapi/portone-payment-sessions-api-openapi.yml,\n  openapi/portone-payments-api-openapi.yml, openapi/portone-payments-by-cursor-api-openapi.yml,\n  openapi/portone-paymentwall-api-openapi.yml, openapi/portone-platform-api-openapi.yml, openapi/portone-promotions-api-openapi.yml,\n  openapi/portone-token-api-openapi.yml\ndescription: Recommended\
  \ x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 147\n  by_action_class:\n    connected: 59\n    acting: 88\n  by_consequence:\n    read: 59\n    write: 49\n    physical: 37\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /b2b/bulk-tax-invoices/{bulkTaxInvoiceId}\n  method: get\n  operationId: getB2bBulkTaxInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/companies/business-info\n  method: post\n  operationId: getB2bBusinessInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/counterparties/{brn}/certificate/registration-url\n\
  \  method: get\n  operationId: getB2bCounterpartyCertificateRegistrationUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/counterparties/{brn}/certificate/validate\n  method: post\n  operationId: validateB2bCounterpartyCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/counterparties/{brn}/certificate\n  method: get\n  operationId: getB2bCounterpartyCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/counterparties/{counterpartyId}\n  method: get\n  operationId: getB2bCounterparty\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/counterparties/{counterpartyId}\n  method: delete\n  operationId: deleteB2bCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/counterparties/{counterpartyId}\n  method: patch\n  operationId: updateB2bCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/counterparties\n  method: get\n  operationId: getB2bCounterparties\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/counterparties\n  method: post\n  operationId: createB2bCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/file-upload-url\n  method: post\n  operationId: createB2bFileUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices-sheet\n  method: get\n  operationId: downloadB2bTaxInvoicesSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/draft\n  method: put\n  operationId: updateB2bTaxInvoiceDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/draft\n  method: post\n  operationId: draftB2bTaxInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/issue-immediately\n  method: post\n  operationId: issueB2bTaxInvoiceImmediately\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/request-reverse-issuance\n  method: post\n  operationId: requestB2bTaxInvoiceReverseIssuance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/attach-file\n  method: post\n  operationId: attachB2bTaxInvoiceFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/attachments/{attachmentId}\n  method: delete\n  operationId: deleteB2bTaxInvoiceAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/attachments\n  method: get\n  operationId: getB2bTaxInvoiceAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/{taxInvoiceKey}/cancel-issuance\n  method: post\n\
  \  operationId: cancelB2bTaxInvoiceIssuance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/cancel-request\n  method: post\n  operationId: cancelB2bTaxInvoiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/issue\n  method: post\n  operationId: issueB2bTaxInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/pdf-download-url\n  method: get\n  operationId: getB2bTaxInvoicePdfDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/{taxInvoiceKey}/popup-url\n  method: get\n  operationId: getB2bTaxInvoicePopupUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/{taxInvoiceKey}/print-url\n  method: get\n  operationId: getB2bTaxInvoicePrintUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/{taxInvoiceKey}/refuse-request\n  method: post\n  operationId: refuseB2bTaxInvoiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/request\n  method: post\n  operationId: requestB2bTaxInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}/send-to-nts\n  method: post\n  operationId:\
  \ sendToNtsB2bTaxInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b2b/tax-invoices/{taxInvoiceKey}\n  method: get\n  operationId: getB2bTaxInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b2b/tax-invoices/{taxInvoiceKey}\n  method: delete\n  operationId: deleteB2bTaxInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /b2b/tax-invoices\n  method: get\n  operationId: getB2bTaxInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks\n  method: get\n  operationId: getBankInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-keys\n  method: get\n  operationId: getBillingKeyInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-keys\n  method: post\n  operationId: issueBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /billing-keys/confirm\n  method: post\n  operationId: confirmBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-keys/confirm-issue-and-pay\n  method: post\n  operationId: confirmBillingKeyIssueAndPay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-keys/{billingKey}\n  method: get\n  operationId: getBillingKeyInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-keys/{billingKey}\n\
  \  method: delete\n  operationId: deleteBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cash-receipts\n  method: get\n  operationId: getCashReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cash-receipts\n  method: post\n  operationId: issueCashReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout-profiles/evaluate\n  method: get\n  operationId: evaluateCheckoutProfile\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity-verifications/{identityVerificationId}/confirm\n  method: post\n  operationId: confirmIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity-verifications/{identityVerificationId}/resend\n  method: post\n  operationId: resendIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity-verifications/{identityVerificationId}/send\n\
  \  method: post\n  operationId: sendIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity-verifications/{identityVerificationId}\n  method: get\n  operationId: getIdentityVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity-verifications\n  method: get\n  operationId: getIdentityVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kakaopay/payment/order\n  method: get\n  operationId: getKakaopayPaymentOrder\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login/api-secret\n  method: post\n  operationId: loginViaApiSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-events-by-cursor\n  method: get\n  operationId: getAllPaymentEventsByCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-gateways/card-promotion\n  method: get\n  operationId: getPgCardPromotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-reconciliations/settlements/vat-report\n\
  \  method: get\n  operationId: getPaymentReconciliationSettlementVatReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-reconciliations/transactions/vat-report\n  method: get\n  operationId: getPaymentReconciliationTransactionVatReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-schedules/{paymentScheduleId}\n  method: get\n  operationId: getPaymentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-schedules\n  method: get\n  operationId: getPaymentSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-schedules\n\
  \  method: delete\n  operationId: revokePaymentSchedules\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /payment-sessions\n  method: post\n  operationId: createPaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-sessions/{sessionId}\n  method: get\n  operationId: getPaymentSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /payment-sessions/{sessionId}/close\n  method: post\n  operationId: closePaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/billing-key\n  method: post\n  operationId: payWithBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cancellations/{cancellationId}/stop\n  method: post\n  operationId: stopPaymentCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /payments/{paymentId}/capture\n  method: post\n  operationId: capturePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cash-receipt/cancel\n  method: post\n  operationId: cancelCashReceiptByPaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cash-receipt\n  method: get\n  operationId: getCashReceiptByPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}/confirm\n  method: post\n  operationId: confirmPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/escrow/complete\n  method: post\n  operationId: confirmEscrow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/escrow/logistics\n  method: post\n  operationId: applyEscrowLogistics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/escrow/logistics\n  method: patch\n  operationId: modifyEscrowLogistics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/instant\n  method: post\n  operationId: payInstantly\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/pre-register\n  method: post\n\
  \  operationId: preRegisterPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/register-store-receipt\n  method: post\n  operationId: registerStoreReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/resend-webhook\n  method: post\n  operationId: resendWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/schedule\n  method: post\n  operationId: createPaymentSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/transactions\n  method: get\n  operationId: getPaymentTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}/virtual-account/close\n  method: post\n  operationId: closeVirtualAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments-by-cursor\n  method: get\n  operationId: getAllPaymentsByCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentwall/delivery/confirm\n\
  \  method: post\n  operationId: confirmPaymentwallDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/account-transfers\n  method: get\n  operationId: getPlatformAccountTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/additional-fee-policies/{id}/archive\n  method: post\n  operationId: archivePlatformAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /platform/additional-fee-policies/{id}/recover\n  method: post\n  operationId: recoverPlatformAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/additional-fee-policies/{id}/schedule\n  method: get\n  operationId: getPlatformAdditionalFeePolicySchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/additional-fee-policies/{id}/schedule\n  method: put\n  operationId: rescheduleAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/additional-fee-policies/{id}/schedule\n  method: post\n  operationId: scheduleAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/additional-fee-policies/{id}/schedule\n  method: delete\n  operationId: cancelPlatformAdditionalFeePolicySchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/additional-fee-policies/{id}\n  method: get\n  operationId: getPlatformAdditionalFeePolicy\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/additional-fee-policies/{id}\n  method: patch\n  operationId: updatePlatformAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/additional-fee-policies\n  method: get\n  operationId: getPlatformAdditionalFeePolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/additional-fee-policies\n  method: post\n  operationId: createPlatformAdditionalFeePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/bank-accounts/{bank}/{accountNumber}/holder\n  method: get\n  operationId: getPlatformAccountHolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/bulk-account-transfers\n  method: get\n  operationId: getPlatformBulkAccountTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/bulk-payouts\n  method: get\n  operationId: getPlatformBulkPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/companies/{businessRegistrationNumber}/state\n  method: get\n \
  \ operationId: getPlatformCompanyState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/contracts/{id}/archive\n  method: post\n  operationId: archivePlatformContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/contracts/{id}/recover\n  method: post\n  operationId: recoverPlatformContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (48 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/agentic-access/portone-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/agentic-access/portone-agentic-access.yml
summary_line: 147 operations · 88 acting · 2 human-in-the-loop
tags:
- Payments
- Payment Orchestration
- Fintech
- South Korea
- Billing
- Identity Verification
---
