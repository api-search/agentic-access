---
acting_count: 102
action_class_counts:
  acting: 102
  connected: 93
api_specs:
- filename: openapi.json
  format: json
  label: BTCPay Server Greenfield API
  slug: btcpay-server-greenfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/openapi/openapi.json
consequence_counts:
  physical: 42
  read: 93
  safety-critical: 6
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Btcpay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api-keys/current
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api-keys/{apikey}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory/{payoutMethodId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedPayoutSenderFactory/{paymentMethodId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedTransferSenderFactory
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/users/{idOrEmail}/api-keys/{apikey}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoiceId}/payment-methods/{paymentMethodId}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoiceId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoiceId}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoiceId}/unarchive
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/payment-requests/{paymentRequestId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/payment-requests/{paymentRequestId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-requests/{paymentRequestId}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/plan-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/plan-checkout/{checkoutId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/pull-payments/{pullPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pull-payments/{pullPaymentId}/boltcards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pull-payments/{pullPaymentId}/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/server/lightning/{cryptoCode}/address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/server/lightning/{cryptoCode}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/server/lightning/{cryptoCode}/invoices/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/stores/{storeId}/email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/stores/{storeId}/invoices
operation_count: 195
overview: 'BTCPay Server exposes 195 API operations that an AI agent could call, of which 102 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 93 read, 54 write, 42 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BTCPay Server
provider_slug: btcpay
slug: btcpay-agentic-access
source_filename: btcpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 195\n  by_action_class:\n    acting: 102\n    connected: 93\n  by_consequence:\n    safety-critical: 6\n    read: 93\n    write: 54\n    physical: 42\n  human_in_the_loop_required: 6\noperations:\n- path: /api/v1/api-keys/{apikey}\n  method: delete\n  operationId: ApiKeys_DeleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - unrestricted\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/v1/users/{idOrEmail}/api-keys/{apikey}\n  method: delete\n  operationId: ApiKeys_DeleteUserApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - unrestricted\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/api-keys/current\n  method: get\n  operationId: ApiKeys_GetCurrentApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canmanageusers\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys/current\n  method: delete\n  operationId: ApiKeys_DeleteCurrentApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n     \
  \ exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/api-keys\n  method: post\n  operationId: ApiKeys_CreateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - unrestricted\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{idOrEmail}/api-keys\n  method: post\n  operationId: ApiKeys_CreateUserApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.server.canmanageusers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/apps/pos\n\
  \  method: post\n  operationId: Apps_CreatePointOfSaleApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/pos/{appId}\n  method: put\n  operationId: Apps_PutPointOfSaleApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/pos/{appId}\n  method: get\n  operationId: Apps_GetPointOfSaleApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/crowdfund/{appId}\n  method: put\n  operationId: Apps_PutCrowdfundApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/crowdfund/{appId}\n  method: get\n  operationId: Apps_GetCrowdfundApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/apps/crowdfund\n  method: post\n  operationId: Apps_CreateCrowdfundApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{appId}\n  method: get\n  operationId: Apps_GetApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canmodifystoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{appId}\n  method: delete\n  operationId: Apps_DeleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{appId}/image\n  method: post\n  operationId: Apps_UploadAppItemImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{appId}/image/{fileId}\n  method: delete\n  operationId: App_DeleteAppItemImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{appId}/sales\n  method: get\n  operationId: Apps_GetAppSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canmodifystoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{appId}/top-items\n \
  \ method: get\n  operationId: Apps_GetAppTopItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canmodifystoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/apps\n  method: get\n  operationId: Apps_GetAllAppsForStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canmodifystoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps\n  method: get\n  operationId: Apps_GetAllApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canmodifystoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/authorize\n  method: get\n  operationId: ApiKeys_Authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/files\n  method: get\n  operationId: Files_GetFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canmodifyserversettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files\n  method: post\n  operationId: Files_UploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.server.canmodifyserversettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files/{fileId}\n  method: get\n  operationId: Files_GetFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canmodifyserversettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/files/{fileId}\n  method: delete\n  operationId: Files_DeleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.server.canmodifyserversettings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/health\n  method: get\n  operationId: Health_GetHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/invoices\n  method: get\n  operationId: Invoices_GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewinvoices\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/invoices\n  method: post\n  operationId: Invoices_CreateInvoice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.cancreateinvoice\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}\n  method: get\n  operationId: Invoices_GetInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewinvoices\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{invoiceId}\n  method: delete\n  operationId: Invoices_ArchiveInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifyinvoices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}\n  method: put\n  operationId: Invoices_UpdateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifyinvoices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}/payment-methods\n  method: get\n  operationId: Invoices_GetInvoicePaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewinvoices\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{invoiceId}/status\n  method: post\n  operationId:\
  \ Invoices_MarkInvoiceStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifyinvoices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}/unarchive\n  method: post\n  operationId: Invoices_UnarchiveInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifyinvoices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}/payment-methods/{paymentMethodId}/activate\n  method: post\n  operationId:\
  \ Invoices_ActivatePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canviewinvoices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}/refund\n  method: post\n  operationId: Invoices_Refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.cancreatepullpayments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoiceId}/refund/{paymentMethodId}\n  method: get\n  operationId: Invoices_GetInvoiceRefundTriggerData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.cancreatepullpayments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/info\n  method: get\n  operationId: InternalLightningNodeApi_GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/balance\n  method: get\n  operationId: InternalLightningNodeApi_GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/histogram\n  method: get\n  operationId: InternalLightningNodeApi_GetHistogram\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/connect\n  method: post\n  operationId: InternalLightningNodeApi_ConnectToNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/server/lightning/{cryptoCode}/channels\n  method: get\n  operationId: InternalLightningNodeApi_GetChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/channels\n\
  \  method: post\n  operationId: InternalLightningNodeApi_OpenChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/server/lightning/{cryptoCode}/address\n  method: post\n  operationId: InternalLightningNodeApi_GetDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/server/lightning/{cryptoCode}/payments/{paymentHash}\n\
  \  method: get\n  operationId: InternalLightningNodeApi_GetPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/invoices/{id}\n  method: get\n  operationId: InternalLightningNodeApi_GetInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canviewlightninginvoiceinternalnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/invoices/pay\n  method: post\n  operationId: InternalLightningNodeApi_PayInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/server/lightning/{cryptoCode}/invoices\n  method: get\n  operationId: InternalLightningNodeApi_GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canviewlightninginvoiceinternalnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/server/lightning/{cryptoCode}/invoices\n  method: post\n  operationId: InternalLightningNodeApi_CreateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.server.cancreatelightninginvoiceinternalnode\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/server/lightning/{cryptoCode}/payments\n  method: get\n  operationId: InternalLightningNodeApi_GetPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.server.canuseinternallightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/info\n  method: get\n  operationId: StoreLightningNodeApi_GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canuselightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/balance\n  method: get\n  operationId: StoreLightningNodeApi_GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canuselightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/histogram\n\
  \  method: get\n  operationId: StoreLightningNodeApi_GetHistogram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canuselightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/connect\n  method: post\n  operationId: StoreLightningNodeApi_ConnectToNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/channels\n  method: get\n  operationId: StoreLightningNodeApi_GetChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/channels\n  method: post\n  operationId: StoreLightningNodeApi_OpenChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/address\n  method: post\n  operationId: StoreLightningNodeApi_GetDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/payments/{paymentHash}\n  method: get\n  operationId: StoreLightningNodeApi_GetPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canuselightningnode\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices/{id}\n  method: get\n  operationId: StoreLightningNodeApi_GetInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewlightninginvoice\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices/pay\n  method: post\n  operationId: StoreLightningNodeApi_PayInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices\n  method: get\n  operationId: StoreLightningNodeApi_GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewlightninginvoice\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices\n  method: post\n  operationId: StoreLightningNodeApi_CreateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.server.cancreatelightninginvoiceinternalnode\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/lightning/{cryptoCode}/payments\n  method: get\n  operationId: StoreLightningNodeApi_GetPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.cancreatelightninginvoice\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/rate-sources\n  method: get\n  operationId: GetRateSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/permissions\n  method: get\n  operationId: permissionsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/lang\n  method: get\n  operationId: langCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /i/{invoiceId}\n  method: get\n  operationId: Invoice_Checkout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/notifications\n  method: get\n  operationId: Notifications_GetNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    - btcpay.user.canviewnotificationsforuser\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/notifications/{id}\n  method: get\n  operationId: Notifications_GetNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    - btcpay.user.canviewnotificationsforuser\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/users/me/notifications/{id}\n  method: put\n  operationId: Notifications_UpdateNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/me/notifications/{id}\n  method: delete\n  operationId: Notifications_DeleteNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/me/notification-settings\n  method: get\n  operationId: Notifications_GetNotificationSettings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/notification-settings\n  method: put\n  operationId: Notifications_UpdateNotificationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - btcpay.user.canmanagenotificationsforuser\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/payment-requests\n  method: get\n  operationId: PaymentRequests_GetPaymentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewpaymentrequests\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/payment-requests\n\
  \  method: post\n  operationId: PaymentRequests_CreatePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifypaymentrequests\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-requests/{paymentRequestId}\n  method: get\n  operationId: PaymentRequests_GetPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewpaymentrequests\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payment-requests/{paymentRequestId}\n  method: delete\n  operationId: PaymentRequests_ArchivePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - btcpay.store.canmodifypaymentrequests\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-requests/{paymentRequestId}\n  method: put\n  operationId: PaymentRequests_UpdatePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifypaymentrequests\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-requests/{paymentRequestId}/pay\n  method: post\n  operationId: PaymentRequests_Pay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - btcpay.store.canviewpaymentrequests\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stores/{storeId}/payout-processors\n  method: get\n  operationId: StorePayoutProcessors_GetStorePayoutProcessors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewstoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/payout-processors/{processor}/{paymentMethodId}\n  method: delete\n  operationId: StorePayoutProcessors_RemoveStorePayoutProcessor\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - btcpay.store.canmodifystoresettings\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout-processors\n  method: get\n  operationId: PayoutProcessors_GetPayoutProcessors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedPayoutSenderFactory/{paymentMethodId}\n  method: get\n  operationId: GreenfieldStoreAutomatedOnChainPayoutProcessorsController_GetStoreOnChainAutomatedPayoutProcessorsForPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewstoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedPayoutSenderFactory/{paymentMethodId}\n  method: put\n  operationId:\
  \ GreenfieldStoreAutomatedOnChainPayoutProcessorsController_UpdateStoreOnChainAutomatedPayoutProcessorForPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - btcpay.store.canviewstoresettings\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory/{payoutMethodId}\n  method: get\n  operationId: GreenfieldStoreAutomatedLightningPayoutProcessorsController_GetStoreLightningAutomatedPayoutProcessorsForPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - btcpay.store.canviewstoresettings\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory/{payoutMethodId}\n\
  \  method: put\n  operationId: GreenfieldStoreAutomatedLightningPayoutProcessorsController_UpdateStoreLightningAutomatedPayoutProcessor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - btcpay.store.canviewstoresettings\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedTransferSenderFactory\n  method: get\n  operationId: GreenfieldStoreAutomatedOnChainPayoutProcessorsController_GetStoreOnChainAutomatedTransferSenderFactory\n  x-agentic-access:\n    action-c\n\n# --- truncated at 32 KB (73 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/agentic-access/btcpay-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/agentic-access/btcpay-agentic-access.yml
summary_line: 195 operations · 102 acting · 6 human-in-the-loop
tags:
- Bitcoin
- Cryptocurrency
- Payments
- Lightning Network
- Open Source
- Self-Hosted
---
