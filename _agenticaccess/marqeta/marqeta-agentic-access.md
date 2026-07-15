---
acting_count: 204
action_class_counts:
  acting: 204
  connected: 232
api_specs:
- filename: marqeta-core-api-openapi.yml
  format: yaml
  label: Marqeta Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-core-api-openapi.yml
- filename: marqeta-diva-api-openapi.yml
  format: yaml
  label: Marqeta Diva API
  slug: diva-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-diva-api-openapi.yml
consequence_counts:
  physical: 55
  read: 232
  safety-critical: 12
  write: 137
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Marqeta Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authcontrols
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authcontrols/exemptmids
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /authcontrols/exemptmids/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /authcontrols/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cards/{token}/stoporders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /cards/{token}/stoporders/{stop_order_token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pins/controltoken
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/auth/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/auth/resetpassword/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /velocitycontrols
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /velocitycontrols/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /velocitycontrols/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/creditbalancerefunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/payments/{payment_token}/releasehold
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/payments/{payment_token}/transitions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/paymentschedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/paymentschedules/{payment_schedule_token}/transitions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_token}/refunds/{refund_token}/transitions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/{short_code}/retryachpayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /banktransfers/ach
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /banktransfers/ach/earlyfunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /banktransfers/ach/transitions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chargebacks
operation_count: 436
overview: 'Marqeta exposes 436 API operations that an AI agent could call, of which 204 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 232 read, 137 write, 55 physical, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Marqeta
provider_slug: marqeta
slug: marqeta-agentic-access
source_filename: marqeta-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/marqeta-core-api-openapi.yml, openapi/marqeta-diva-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 436\n  by_action_class:\n    connected: 232\n    acting: 204\n  by_consequence:\n    read: 232\n    write: 137\n    physical: 55\n    safety-critical: 12\n  human_in_the_loop_required: 12\noperations:\n- path: /acceptedcountries\n  method: get\n  operationId: getAcceptedcountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acceptedcountries/{token}\n  method: get\n  operationId: getAcceptedcountriesToken\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountholdergroups\n  method: get\n  operationId: getAccountholdergroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountholdergroups\n  method: post\n  operationId: postAccountholdergroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountholdergroups/{token}\n  method: get\n  operationId: getAccountholdergroupsToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountholdergroups/{token}\n  method: put\n  operationId: putAccountholdergroupsToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}\n  method: get\n  operationId: retrieveAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/accounttransitions\n  method: get\n  operationId: listAccountTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/accounttransitions\n  method: post\n  operationId: transitionAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/accounttransitions/{token}\n  method: get\n  operationId: getAccountTransition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/adjustments\n\
  \  method: get\n  operationId: getAdjustmentsByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/adjustments\n  method: post\n  operationId: createAdjustmentForAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/adjustments/{adjustment_token}\n  method: get\n  operationId: retrieveAdjustment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/billingcycle\n  method: get\n  operationId: retrieveBillingCycleForAccount\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/bundletransitions\n  method: get\n  operationId: listAccountBundleTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/bundletransitions\n  method: post\n  operationId: transitionAccountBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/bundletransitions/{token}\n  method: get\n  operationId: getAccountBundleTransition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /accounts/{account_token}/cards\n  method: get\n  operationId: getCardsByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/cards\n  method: post\n  operationId: createCardForAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/cards/{card_token}\n  method: get\n  operationId: getCardByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/creditbalancerefunds\n  method: post\n  operationId: createBalanceRefund\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/delinquencystate\n  method: get\n  operationId: retrieveDelinquencyState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/delinquencystate/transitions\n  method: get\n  operationId: retrieveDelinquencyTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/delinquencystate/transitions/{delinquency_transition_token}\n  method: get\n  operationId: retrieveDelinquencyTransition\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/disputes\n  method: get\n  operationId: getDisputesByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/disputes\n  method: post\n  operationId: createDisputeForAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/disputes/{dispute_token}\n  method: get\n  operationId: retrieveDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /accounts/{account_token}/disputes/{dispute_token}/transitions\n  method: post\n  operationId: transitionDispute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/documents\n  method: get\n  operationId: getAccountDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/documents/{document_type}\n  method: get\n  operationId: getDocumentByAccountAndType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/documents/{document_type}/history\n  method: get\n  operationId:\
  \ getDocumentHistoryByAccountAndType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/fees\n  method: get\n  operationId: getFeesByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/fees\n  method: post\n  operationId: createFee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/fees/{fee_token}\n  method: get\n  operationId: retrieveFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounts/{account_token}/journalentries\n  method: get\n  operationId: ListAccountJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/journalentries/{journal_entry_token}\n  method: get\n  operationId: getAccountJournalEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/ledgerentries\n  method: get\n  operationId: ListAccountLedgerEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/ledgerentries/{ledger_entry_token}\n  method: get\n  operationId: getAccountLedgerEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/payments/{payment_token}\n  method: get\n  operationId: retrievePayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/payments/{payment_token}/releasehold\n\
  \  method: post\n  operationId: releasePaymentHold\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/payments/{payment_token}/transitions\n  method: post\n  operationId: transitionPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/paymentschedules\n  method: get\n  operationId: retrievePaymentSchedules\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/paymentschedules\n  method: post\n  operationId: createPaymentSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/paymentschedules/{payment_schedule_token}\n  method: get\n  operationId: retrievePaymentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/paymentschedules/{payment_schedule_token}/transitions\n  method: get\n  operationId: retrievePaymentScheduleTransitions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/paymentschedules/{payment_schedule_token}/transitions\n  method: post\n  operationId: createPaymentScheduleTransition\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/paymentschedules/{payment_schedule_token}/transitions/{token}\n  method: get\n  operationId: retrievePaymentScheduleTransition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/periodicfeeschedules\n  method: get\n  operationId: getPeriodicFeeSchedules\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/refunds/{refund_token}\n  method: get\n  operationId: retrieveRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/refunds/{refund_token}/transitions\n  method: get\n  operationId: retrieveRefundTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/refunds/{refund_token}/transitions\n  method: post\n  operationId: transitionRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/rewards\n  method: post\n  operationId: createReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_token}/signupbonusprogress\n  method: get\n  operationId: retrieveSignupBonusProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements\n  method: get\n  operationId: getStatementSummariesByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/files\n  method: get\n  operationId: getStatementFilesByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}\n  method: get\n  operationId:\
  \ retrieveStatementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/files\n  method: get\n  operationId: retrieveStatementFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/interestcharges\n  method: get\n  operationId: retrieveStatementInterestCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/journalentries\n  method: get\n  operationId: listStatementJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/ledgerentries\n  method: get\n  operationId: listStatementLedgerEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/paymentinfo\n  method: get\n  operationId: retrieveStatementPaymentInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/paymentreminders/\n  method: get\n  operationId: getPaymentRemindersByStatementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/paymentreminders/{token}\n\
  \  method: get\n  operationId: getPaymentReminder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/rewards\n  method: get\n  operationId: retrieveStatementReward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/statements/{statement_summary_token}/yeartodate\n  method: get\n  operationId: retrieveYearToDateForStatementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_token}/transactions\n  method: get\n  operationId: ListAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /accountusers/{user_token}\n  method: get\n  operationId: retrieveAccountUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/programs/funding\n  method: get\n  operationId: getProgramFundings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/replayfailedstatements\n  method: post\n  operationId: replayFailedStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/replayfailedstatements/{short_code}\n  method: post\n  operationId: replayFailedStatementsByShortCode\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/schedulestatements\n  method: post\n  operationId: scheduleStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/{short_code}/replayfailedstatement/{account_token}\n  method: post\n  operationId: replaySingleFailedStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /admin/{short_code}/retryachpayments\n  method: post\n  operationId: retryAchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authcontrols\n  method: get\n  operationId: getAuthcontrols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authcontrols\n  method: post\n  operationId: postAuthcontrols\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n     \
  \ human-in-the-loop: required\n    audit: required\n- path: /authcontrols/exemptmids\n  method: get\n  operationId: getAuthcontrolsExemptmids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authcontrols/exemptmids\n  method: post\n  operationId: postAuthcontrolsExemptmids\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authcontrols/exemptmids/{token}\n  method: get\n  operationId: getAuthcontrolsExemptmidsToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authcontrols/exemptmids/{token}\n  method: put\n\
  \  operationId: putAuthcontrolsExemptmidsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authcontrols/{token}\n  method: get\n  operationId: getAuthcontrolsToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authcontrols/{token}\n  method: put\n  operationId: putAuthcontrolsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /autoreloads\n\
  \  method: get\n  operationId: getAutoreloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoreloads\n  method: post\n  operationId: postAutoreloads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoreloads/{token}\n  method: get\n  operationId: getAutoreloadsToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoreloads/{token}\n  method: put\n  operationId: putAutoreloadsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balances/account/{token}\n  method: get\n  operationId: getAccountBalancesToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/user/{token}\n  method: get\n  operationId: getUserAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/{token}\n  method: get\n  operationId: getBalancesToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banktransfers/ach\n  method: get\n  operationId: getBanktransfersAch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /banktransfers/ach\n  method: post\n  operationId: postBanktransfersAch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banktransfers/ach/earlyfunds\n  method: post\n  operationId: postApplyProvisionalCreditToBankTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banktransfers/ach/transitions\n  method: get\n  operationId: getBanktransfersAchTransitions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banktransfers/ach/transitions\n  method: post\n  operationId: postBanktransfersAchTransitions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banktransfers/ach/{token}\n  method: get\n  operationId: getBanktransfersAchToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulkissuances\n  method: get\n  operationId: getBulkissuances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /bulkissuances\n  method: post\n  operationId: postBulkissuances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulkissuances/{token}\n  method: get\n  operationId: getBulkissuancesToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles\n  method: get\n  operationId: listBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles\n  method: post\n  operationId: createBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{token}\n  method: get\n  operationId: retrieveBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{token}\n  method: put\n  operationId: updateBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{token}/clone\n  method: post\n  operationId: cloneBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{token}/lineage\n  method: get\n  operationId: listRelatedBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{token}/promote\n  method: put\n  operationId: promoteBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{token}/transitions\n  method: post\n  operationId: transitionBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\n\
  \n# --- truncated at 32 KB (127 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/agentic-access/marqeta-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/agentic-access/marqeta-agentic-access.yml
summary_line: 436 operations · 204 acting · 12 human-in-the-loop
tags:
- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance
---
