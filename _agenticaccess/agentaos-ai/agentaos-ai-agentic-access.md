---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 44
api_specs:
- filename: agentaos-ai-bank-accounts-api-openapi.yml
  format: yaml
  label: AgentaOS Bank Accounts API
  slug: agentaos-ai-bank-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-bank-accounts-api-openapi.yml
- filename: agentaos-ai-businesses-api-openapi.yml
  format: yaml
  label: AgentaOS Businesses API
  slug: agentaos-ai-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-businesses-api-openapi.yml
- filename: agentaos-ai-checkouts-api-openapi.yml
  format: yaml
  label: AgentaOS Checkouts API
  slug: agentaos-ai-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-checkouts-api-openapi.yml
- filename: agentaos-ai-customers-api-openapi.yml
  format: yaml
  label: AgentaOS Customers API
  slug: agentaos-ai-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-customers-api-openapi.yml
- filename: agentaos-ai-discount-codes-api-openapi.yml
  format: yaml
  label: AgentaOS Discount Codes API
  slug: agentaos-ai-discount-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-discount-codes-api-openapi.yml
- filename: agentaos-ai-invoices-api-openapi.yml
  format: yaml
  label: AgentaOS Invoices API
  slug: agentaos-ai-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-invoices-api-openapi.yml
- filename: agentaos-ai-payment-links-api-openapi.yml
  format: yaml
  label: AgentaOS Payment Links API
  slug: agentaos-ai-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-payment-links-api-openapi.yml
- filename: agentaos-ai-subscriptions-api-openapi.yml
  format: yaml
  label: AgentaOS Subscriptions API
  slug: agentaos-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-subscriptions-api-openapi.yml
- filename: agentaos-ai-transactions-api-openapi.yml
  format: yaml
  label: AgentaOS Transactions API
  slug: agentaos-ai-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentaos-ai/openapi/agentaos-ai-transactions-api-openapi.yml
consequence_counts:
  physical: 20
  read: 44
  safety-critical: 4
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Agentaos Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gateway/businesses/{id}/invitation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gateway/businesses/{id}/invitation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gateway/discount-codes/{id}/archive
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gateway/discount-codes/{id}/archive
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/businesses/{id}/invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/businesses/{id}/invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/invoices/{invoiceId}/send-receipt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/invoices/{invoiceId}/send-receipt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/invoices/{invoiceId}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/invoices/{invoiceId}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /gateway/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /gateway/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /gateway/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /gateway/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/payment-links/{id}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/payment-links/{id}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/sessions/{sessionId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/sessions/{sessionId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/transactions/{id}/refund-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gateway/transactions/{id}/refund-request
operation_count: 88
overview: 'AgentaOS exposes 88 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 20 write, 20 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentaOS
provider_slug: agentaos-ai
slug: agentaos-ai-agentic-access
source_filename: agentaos-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agentaos-ai-openapi.json, openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    connected: 44\n    acting: 44\n  by_consequence:\n    read: 44\n    write: 20\n    physical: 20\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /gateway/bank-accounts/requirements\n  method: get\n  operationId: getBankAccountRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/bank-accounts/requirements/refresh\n  method: post\n  operationId: refreshBankAccountRequirements\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/bank-accounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/bank-accounts\n  method: post\n  operationId: createBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/bank-accounts/{id}\n  method: delete\n  operationId: deactivateBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links\n  method: get\n  operationId: listPaymentLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/payment-links/{id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/payment-links/{id}\n  method: patch\n  operationId: updatePaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links/{id}\n  method: delete\n  operationId: cancelPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links/{id}/activate\n  method: post\n  operationId: activatePaymentLink\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/sessions\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/sessions\n  method: get\n  operationId: listCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/sessions/{sessionId}\n  method:\
  \ get\n  operationId: getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/sessions/{sessionId}/cancel\n  method: post\n  operationId: cancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/subscriptions/{id}/plan-change/preview\n  method: get\n  operationId: previewSubscriptionPlanChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/plan-change\n  method: post\n  operationId: changeSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/statement\n  method: get\n  operationId: downloadStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/export\n  method: get\n  operationId: exportInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/void\n\
  \  method: post\n  operationId: voidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/invoices/{invoiceId}/pdf\n  method: get\n  operationId: downloadInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/receipt\n  method: get\n  operationId: downloadReceiptPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/send-receipt\n  method: post\n  operationId: resendReceipt\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/transactions/{id}/refund-request\n  method: post\n  operationId: requestRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/all-transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses\n  method: get\n  operationId:\
  \ listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses\n  method: post\n  operationId: createBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/businesses/{id}\n  method: get\n  operationId: retrieveBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses/{id}/invitation\n  method: post\n  operationId: resendBusinessInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/businesses/{id}/invitation\n  method: delete\n  operationId: revokeBusinessInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gateway/businesses/{id}/verification-link\n  method: post\n  operationId: createBusinessVerificationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/discount-codes\n\
  \  method: post\n  operationId: createDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/discount-codes\n  method: get\n  operationId: listDiscountCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/discount-codes/{id}\n  method: get\n  operationId: getDiscountCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/discount-codes/{id}/archive\n  method: post\n  operationId: archiveDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gateway/subscriptions/{id}/credits\n  method: post\n  operationId: grantSubscriptionCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/subscriptions/{id}/credits\n  method: get\n  operationId: getSubscriptionCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/invoices\n  method: get\n  operationId: getSubscriptionInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/resume\n  method: post\n  operationId: resumeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/bank-accounts/requirements\n  method: get\n  operationId: getBankAccountRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/bank-accounts/requirements/refresh\n  method: post\n  operationId: refreshBankAccountRequirements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/bank-accounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/bank-accounts\n  method: post\n  operationId: createBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/bank-accounts/{id}\n  method: delete\n  operationId: deactivateBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /gateway/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links\n  method: get\n  operationId: listPaymentLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/payment-links/{id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/payment-links/{id}\n  method: patch\n  operationId: updatePaymentLink\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links/{id}\n  method: delete\n  operationId: cancelPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/payment-links/{id}/activate\n  method: post\n  operationId: activatePaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/sessions\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/sessions\n  method: get\n  operationId: listCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/sessions/{sessionId}\n  method: get\n  operationId: getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /gateway/sessions/{sessionId}/cancel\n  method: post\n  operationId: cancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /gateway/subscriptions/{id}/plan-change/preview\n  method: get\n  operationId: previewSubscriptionPlanChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/plan-change\n  method: post\n  operationId: changeSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/statement\n  method: get\n  operationId: downloadStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/export\n  method: get\n  operationId: exportInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/void\n  method: post\n  operationId: voidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/invoices/{invoiceId}/pdf\n  method: get\n  operationId: downloadInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/receipt\n  method: get\n  operationId: downloadReceiptPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/invoices/{invoiceId}/send-receipt\n  method: post\n  operationId: resendReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/transactions/{id}/refund-request\n  method: post\n  operationId: requestRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/all-transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /gateway/businesses\n  method: post\n  operationId: createBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/businesses/{id}\n  method: get\n  operationId: retrieveBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses/{id}/invitation\n  method: post\n  operationId: resendBusinessInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /gateway/businesses/{id}/invitation\n  method: delete\n  operationId: revokeBusinessInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gateway/businesses/{id}/verification-link\n  method: post\n  operationId: createBusinessVerificationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/discount-codes\n  method: post\n  operationId: createDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/discount-codes\n  method: get\n  operationId: listDiscountCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/discount-codes/{id}\n  method: get\n  operationId: getDiscountCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/discount-codes/{id}/archive\n  method: post\n  operationId: archiveDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /gateway/subscriptions/{id}/credits\n  method: post\n  operationId: grantSubscriptionCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/subscriptions/{id}/credits\n  method: get\n  operationId: getSubscriptionCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/invoices\n  method: get\n  operationId: getSubscriptionInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/subscriptions/{id}/resume\n  method: post\n  operationId:\
  \ resumeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentaos-ai/agentic-access/agentaos-ai-agentic-access.yml
summary_line: 88 operations · 44 acting · 4 human-in-the-loop
tags:
- Payments
- Billing
- Software-as-a-Service
- Freelancers
- Artificial Intelligence
---
