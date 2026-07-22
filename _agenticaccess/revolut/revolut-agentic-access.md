---
acting_count: 119
action_class_counts:
  acting: 119
  connected: 118
api_specs:
- filename: revolut-business-openapi.yaml
  format: yaml
  label: Revolut Business API
  slug: revolut-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-business-openapi.yaml
- filename: revolut-merchant-openapi.yaml
  format: yaml
  label: Revolut Merchant API
  slug: revolut-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-merchant-openapi.yaml
- filename: revolut-open-banking-openapi.yaml
  format: yaml
  label: Revolut Open Banking API
  slug: revolut-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-open-banking-openapi.yaml
- filename: revolut-crypto-ramp-openapi.yaml
  format: yaml
  label: Revolut Crypto Ramp API
  slug: revolut-crypto-ramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-crypto-ramp-openapi.yaml
- filename: revolut-x-openapi.yaml
  format: yaml
  label: Revolut X API
  slug: revolut-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-x-openapi.yaml
consequence_counts:
  physical: 48
  read: 118
  safety-critical: 1
  write: 70
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Revolut Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cards/{card_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/customers/{customer_id}/payment-methods/{payment_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/customers/{customer_id}/payment-methods/{payment_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/increment-authorisation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/payment-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-intents/{payment_intent_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/synchronous-webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /counterparties/{counterparty_id}/payment-methods/{payment_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-scheduled-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-scheduled-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-standing-order-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-standing-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /draft-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /draft-payments/{DraftPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /draft-payments/{DraftPaymentId}/transfers/{DraftPaymentTransferId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /file-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /file-payment-consents/{ConsentId}/file
operation_count: 237
overview: 'Revolut exposes 237 API operations that an AI agent could call, of which 119 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 118 read, 70 write, 48 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Revolut
provider_slug: revolut
slug: revolut-agentic-access
source_filename: revolut-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/revolut-business-openapi.yaml, openapi/revolut-crypto-ramp-openapi.yaml, openapi/revolut-merchant-openapi.yaml,\n  openapi/revolut-open-banking-openapi.yaml, openapi/revolut-x-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 237\n  by_action_class:\n    acting: 119\n    connected: 118\n  by_consequence:\n    write: 70\n    read: 118\n    safety-critical: 1\n    physical: 48\n  human_in_the_loop_required: 1\noperations:\n- path: /accounting-categories\n  method: post\n  operationId: createAccountingCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting-categories\n  method: get\n  operationId: getAccountingCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting-categories/{accounting_category_id}\n  method: get\n  operationId: getAccountingCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting-categories/{accounting_category_id}\n  method: patch\n  operationId: updateAccountingCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting-categories/{accounting_category_id}\n  method: delete\n  operationId: deleteAccountingCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-name-validation\n  method: post\n  operationId: validateAccountName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/bank-details\n  method: get\n  operationId: getAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-invitations\n  method: post\n  operationId: createCardInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /card-invitations\n  method: get\n  operationId: getCardInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-invitations/{card_invitation_id}\n  method: get\n  operationId: getCardInvitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-invitations/{card_invitation_id}\n  method: patch\n  operationId: updateCardInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-invitations/{cardInvitationId}/cancel\n  method: post\n\
  \  operationId: cancelCardInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: get\n  operationId: getCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}\n  method: delete\n  operationId: deleteCard\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cards/{card_id}/contacts\n  method: put\n  operationId: updateCardContacts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/references\n  method: put\n  operationId: updateCardReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/freeze\n  method: post\n  operationId: freezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/unfreeze\n  method: post\n  operationId: unfreezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/lock\n  method: post\n  operationId: lockCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/unlock\n  method: post\n  operationId: unlockCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/sensitive-details\n  method: get\n  operationId: getSensitiveCardDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ_SENSITIVE_CARD_DATA\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparties\n  method: get\n  operationId: getCounterparties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparty\n  method: post\n  operationId: addCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counterparties/countries\n  method: get\n  operationId: getCounterpartyCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparties/fields\n  method: get\n  operationId: getCounterpartyRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparty/{counterparty_id}\n  method: get\n  operationId: getCounterparty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparty/{counterparty_id}\n  method: delete\n  operationId: deleteCounterparty\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counterparties/{counterparty_id}/payment-methods/{payment_method_id}\n  method: patch\n  operationId: updateCounterpartyPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rate\n  method: get\n  operationId: getRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /exchange\n  method: post\n  operationId: exchangeMoney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - PAY\n    - READ\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange-reasons\n  method: get\n  operationId: getExchangeReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expenses/{expense_id}\n  method: get\n  operationId: getExpense\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expenses/{expense_id}/receipts/{receipt_id}/content\n  method: get\n  operationId: getExpenseReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /label-groups\n  method: post\n  operationId: createLabelGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label-groups\n  method: get\n  operationId: getLabelGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /label-groups/{group_id}\n  method: get\n  operationId: getLabelGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /label-groups/{group_id}\n  method: patch\n  operationId: updateLabelGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label-groups/{group_id}\n  method: delete\n  operationId: deleteLabelGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /label-groups/{group_id}/labels\n  method: post\n  operationId: createLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label-groups/{group_id}/labels\n  method: get\n  operationId: getLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /label-groups/{group_id}/labels/{label_id}\n  method: patch\n  operationId: updateLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label-groups/{group_id}/labels/{label_id}\n  method: delete\n  operationId: deleteLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts\n  method: get\n  operationId: getPaymentDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-drafts\n  method: post\n  operationId: createPaymentDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts/{payment_draft_id}\n  method: get\n  operationId: getPaymentDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-drafts/{payment_draft_id}\n  method: delete\n  operationId: deletePaymentDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts/{payment_draft_id}\n  method: patch\n  operationId: updatePaymentDraft\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts/{payment_draft_id}/payments\n  method: post\n  operationId: addPaymentDraftPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts/{payment_draft_id}/payments/{payment_id}\n  method: patch\n  operationId: updatePaymentDraftPayment\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-drafts/{payment_draft_id}/payments/{payment_id}\n  method: delete\n  operationId: deletePaymentDraftPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout-links\n  method: post\n  operationId: createPayoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n \
  \   - PAY\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout-links\n  method: get\n  operationId: getPayoutLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payout-links/{payout_link_id}\n  method: get\n  operationId: getPayoutLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payout-links/{payout_link_id}/cancel\n  method: post\n  operationId: cancelPayoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/transactions/{id}/{action}\n  method: post\n  operationId: simulateTransferStateUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/topup\n  method: post\n  operationId: simulateTopUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /tax-rates\n  method: post\n  operationId: createTaxRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tax-rates\n  method: get\n  operationId: getTaxRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-rates/{tax_rate_id}\n  method: get\n  operationId: getTaxRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-rates/{tax_rate_id}\n  method: patch\n  operationId: updateTaxRate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tax-rates/{tax_rate_id}\n  method: delete\n  operationId: deleteTaxRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team-members\n  method: get\n  operationId: getTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team-members\n  method: post\n  operationId: inviteTeamMember\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team-members/{team_member_id}\n  method: delete\n  operationId: deleteTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n  method: get\n  operationId: getRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - PAY\n    - READ\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/indicative-quote\n  method: post\n  operationId: getIndicativeQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - PAY\n    - READ\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/fields\n  method: post\n  operationId: getPaymentRequirements\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - PAY\n    - READ\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - PAY\n    - READ\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer-reasons\n  method: get\n  operationId: getTransferReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: get\n  operationId: getWebhookV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: setUpWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook\n  method: delete\n  operationId: deleteWebhookV1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - READ\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/rotate-signing-secret\n  method: post\n  operationId: rotateWebhookSigningSecret\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/failed-events\n  method: get\n  operationId: getFailedWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: retrieve-configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: retrieve-an-order-quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /buy\n  method: get\n  operationId: retrieve-a-redirect-url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  operationId: retrieve-an-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: retrieve-all-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: get\n  operationId: retrieve-a-webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: patch\n  operationId: update-a-webhook\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: delete-a-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: retrieve-a-list-of-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: create-a-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders\n  method: get\n  operationId: retrieveOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_id}\n  method: get\n  operationId: retrieveOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/orders/{order_id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl\n\n# --- truncated at 32 KB (73 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/agentic-access/revolut-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/agentic-access/revolut-agentic-access.yml
summary_line: 237 operations · 119 acting · 1 human-in-the-loop
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Merchant Acquiring
- Cryptocurrency
- Cards
---
