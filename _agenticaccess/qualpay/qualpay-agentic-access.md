---
acting_count: 78
action_class_counts:
  acting: 78
  connected: 58
api_specs:
- filename: qualpay-account-updater-api-openapi.yml
  format: yaml
  label: Qualpay Account Updater API
  slug: qualpay-account-updater-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-account-updater-api-openapi.yml
- filename: qualpay-application-boarding-api-openapi.yml
  format: yaml
  label: Qualpay Application Boarding API
  slug: qualpay-application-boarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-application-boarding-api-openapi.yml
- filename: qualpay-checkout-api-openapi.yml
  format: yaml
  label: Qualpay Checkout API
  slug: qualpay-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-checkout-api-openapi.yml
- filename: qualpay-customer-vault-api-openapi.yml
  format: yaml
  label: Qualpay Customer Vault API
  slug: qualpay-customer-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-customer-vault-api-openapi.yml
- filename: qualpay-disputes-v0-5-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v0.5 API
  slug: qualpay-disputes-v0-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v0-5-api-openapi.yml
- filename: qualpay-disputes-v1-0-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v1.0 API
  slug: qualpay-disputes-v1-0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v1-0-api-openapi.yml
- filename: qualpay-embedded-fields-api-openapi.yml
  format: yaml
  label: Qualpay Embedded Fields API
  slug: qualpay-embedded-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-embedded-fields-api-openapi.yml
- filename: qualpay-integrator-api-openapi.yml
  format: yaml
  label: Qualpay Integrator API
  slug: qualpay-integrator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-integrator-api-openapi.yml
- filename: qualpay-invoicing-api-openapi.yml
  format: yaml
  label: Qualpay Invoicing API
  slug: qualpay-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-invoicing-api-openapi.yml
- filename: qualpay-payee-vault-api-openapi.yml
  format: yaml
  label: Qualpay Payee Vault API
  slug: qualpay-payee-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payee-vault-api-openapi.yml
- filename: qualpay-payment-gateway-api-openapi.yml
  format: yaml
  label: Qualpay Payment Gateway API
  slug: qualpay-payment-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payment-gateway-api-openapi.yml
- filename: qualpay-recurring-billing-api-openapi.yml
  format: yaml
  label: Qualpay Recurring Billing API
  slug: qualpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-recurring-billing-api-openapi.yml
- filename: qualpay-reporting-api-openapi.yml
  format: yaml
  label: Qualpay Reporting API
  slug: qualpay-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-reporting-api-openapi.yml
- filename: qualpay-token-api-openapi.yml
  format: yaml
  label: Qualpay Token API
  slug: qualpay-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-token-api-openapi.yml
- filename: qualpay-transaction-api-openapi.yml
  format: yaml
  label: Qualpay Transaction API
  slug: qualpay-transaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-transaction-api-openapi.yml
- filename: qualpay-webhooks-api-openapi.yml
  format: yaml
  label: Qualpay Webhooks API
  slug: qualpay-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-webhooks-api-openapi.yml
consequence_counts:
  physical: 36
  read: 58
  safety-critical: 1
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Qualpay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /platform/webhook/{webhook_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/auth
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/balance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/batchClose
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/capture/{pgIdOrig}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/credit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/emailReceipt/{pgId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/expireToken
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/force
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/recharge/{pgIdOrig}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/refund/{pgIdOrig}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/sale
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/tokenize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pg/void/{pgIdOrig}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /platform/checkout/{checkout_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /platform/invoice/{invoice_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/invoice/{invoice_id}/copy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /platform/invoice/{invoice_id}/draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /platform/invoice/{invoice_id}/outstanding
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/invoice/{invoice_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /platform/invoice/{invoice_id}/payments/{payment_id}
operation_count: 136
overview: 'Qualpay exposes 136 API operations that an AI agent could call, of which 78 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 58 read, 41 write, 36 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qualpay
provider_slug: qualpay
slug: qualpay-agentic-access
source_filename: qualpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/qualpay-apis-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 136\n  by_action_class:\n    connected: 58\n    acting: 78\n  by_consequence:\n    read: 58\n    physical: 36\n    write: 41\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /pg/ardef\n  method: post\n  operationId: Get Card Type Information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pg/auth\n  method: post\n  operationId: Authorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/balance\n  method: post\n  operationId: Request Balance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/batchClose\n  method: post\n  operationId: Batch Close\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /pg/capture/{pgIdOrig}\n  method: post\n  operationId: Capture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/credit\n  method: post\n  operationId: Credit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/emailReceipt/{pgId}\n  method: post\n  operationId: Send Receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/expireToken\n  method: post\n  operationId: Expire\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/force\n  method: post\n  operationId: Force\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/payment\n\
  \  method: post\n  operationId: Initiate Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/recharge/{pgIdOrig}\n  method: post\n  operationId: Recharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/refund/{pgIdOrig}\n  method: post\n  operationId: Refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/sale\n  method: post\n  operationId: Sale\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/tokenize\n  method: post\n  operationId: Tokenize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/verify\n  method:\
  \ post\n  operationId: Verify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg/void/{pgIdOrig}\n  method: post\n  operationId: Void\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/application/add\n  method: post\n  operationId: addApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/application/browse\n  method: get\n  operationId: browseApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/application/sales/browse\n  method: get\n  operationId: browseSalesReps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/application/{appId}/data\n  method: post\n  operationId: saveData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/application/{appId}/email\n  method: post\n\
  \  operationId: emailApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/application/{appId}/get\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/application/{appId}/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/application/{appId}/validate\n  method: get\n  operationId: validateApp\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/aus/add\n  method: post\n  operationId: addAusJsonRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/aus/hold\n  method: post\n  operationId: putOnAusHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/aus/release\n  method: post\n  operationId: releaseFromAusHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/aus/request/cancel/{request_id}\n  method: post\n  operationId: cancelAusRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/aus/request/create\n  method: post\n  operationId: createAusRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/aus/request/detail\n  method: get\n  operationId: browseAusRequestsDetail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/aus/request/detail/{request_id}\n  method: get\n  operationId: getAusDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/aus/request/summary\n  method: get\n  operationId: browseAusRequestsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/aus/request/summary/{request_id}\n  method: get\n  operationId: getAusSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/aus/{requestId}\n  method: get\n  operationId: getAusResponse\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/checkout\n  method: post\n  operationId: addCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/checkout/{checkoutId}\n  method: get\n  operationId: getDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/checkout/{checkout_id}/cancel\n  method: delete\n  operationId: cancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/dispute/browse\n  method: get\n  operationId: getDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{merchantId}/create\n  method: get\n  operationId: createDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}\n  method: get\n  operationId: getDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/accept\n  method: get\n  operationId: acceptDispute\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/action\n  method: post\n  operationId: submitDisputeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/dispute/{recId}/creditedtrans\n  method: get\n  operationId: getCreditedTran\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/doc/delete\n  method: post\n  operationId: deleteDisputeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /platform/dispute/{recId}/doc/list\n  method: get\n  operationId: getDisputeFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/doc/upload\n  method: post\n  operationId: uploadDisputeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/dispute/{recId}/nondisputedtrans\n  method: get\n  operationId: getNonDisputedTran\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/remedyundisputedtrans\n  method: get\n  operationId:\
  \ getRemedyUndisputedTran\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/reset\n  method: get\n  operationId: resetDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/dispute/{recId}/respond\n  method: post\n  operationId: submitDisputesResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/dispute/{recId}/response\n  method: get\n  operationId: getDisputeResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /platform/embedded\n  method: get\n  operationId: getEmbeddedTransientKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice\n  method: get\n  operationId: browseInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/bounced\n  method: get\n  operationId: browseBouncedInvoices\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice/payments\n  method: get\n  operationId: browseInvoicePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice/{invoice_id}/cancel\n  method: delete\n  operationId: cancelInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/copy\n  method: post\n  operationId: copyInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/detail\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice/{invoice_id}/draft\n  method: put\n  operationId: updateDraftInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/outstanding\n  method: put\n  operationId: updateOutstandingInvoice\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/payments\n  method: get\n  operationId: browseInvoicePaymentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/invoice/{invoice_id}/payments\n  method: post\n  operationId: addInvoicePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/payments/{payment_id}\n\
  \  method: put\n  operationId: updateInvoicePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/payments/{payment_id}\n  method: delete\n  operationId: removeInvoicePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/resend\n  method: post\n  operationId: resendInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/invoice/{invoice_id}/send\n  method: post\n  operationId: sendInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/pg-tokens/pending\n  method: post\n  operationId: generatePendingToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /platform/pg-tokens/status/{cardId}\n  method: get\n  operationId: tokenStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/pg-tokens/unblock\n  method: post\n  operationId: unblockToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/plan\n  method: get\n  operationId: browsePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/plan\n  method: post\n  operationId: addPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/plan/{plan_code}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/plan/{plan_code}\n  method: put\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/plan/{plan_code}/archive\n  method: post\n  operationId: archivePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/plan/{plan_id}/delete\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/reporting/batches\n  method: get\n  operationId: browseBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/deposits\n  method: get\n  operationId: browseDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/disputes\n  method: get\n  operationId:\
  \ browseDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/disputeAdjustment\n  method: get\n  operationId: browseStatementDisputeAdjustmentData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/fees\n  method: get\n  operationId: browseStatementFeeData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/planType\n  method: get\n  operationId: browseStatementPlanData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/reserve\n\
  \  method: get\n  operationId: browseStatementReserveData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/settlement\n  method: get\n  operationId: browseStatementSettlementData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/statement-report/summary\n  method: get\n  operationId: browseStatementSummaryData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/transaction-requests\n  method: get\n  operationId: getTransactionRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/transactions\n\
  \  method: get\n  operationId: browseTrans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/reporting/transactions/bypgid/{pg_id}\n  method: get\n  operationId: getTransactionByPgId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription\n  method: get\n  operationId: browseSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription\n  method: post\n  operationId: addSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /platform/subscription/transactions\n  method: get\n  operationId: getAllSubscriptionTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription/transactions/{subscription_id}\n  method: get\n  operationId: getSubscriptionTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription/{subscription_id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription/{subscription_id}\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/subscription/{subscription_id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/subscription/{subscription_id}/labels/add\n  method: post\n  operationId: subscriptionLabelsAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/subscription/{subscription_id}/labels/browse\n\
  \  method: get\n  operationId: subscriptionLabelsBrowse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/subscription/{subscription_id}/labels/delete\n  method: post\n  operationId: subscriptionLabelsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/subscription/{subscription_id}/labels/edit\n  method: post\n  operationId: subscriptionLabelsEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /platform/subscription/{subscription_id}/pause\n  method: post\n  operationId: pauseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/subscription/{subscription_id}/resume\n  method: post\n  operationId: resumeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/transaction/refund_non_pg\n  method: post\n  operationId: refundNonPg\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/vault/customer\n  method: get\n  operationId: browseCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/vault/customer\n  method: post\n  operationId: addCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/vault/customer/cardid/{card_id}\n  method: get\n  operationId: getCustomerByCardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n\n\n# --- truncated at 32 KB (42 KB total) ---\n# Full source: https://artifacts.apis.io/qualpay/agentic-access/qualpay-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/qualpay/agentic-access/qualpay-agentic-access.yml
summary_line: 136 operations · 78 acting · 1 human-in-the-loop
tags:
- Payments
- Payment Processing
- Merchant Services
- B2B Payments
- Reporting
- Tokenization
---
