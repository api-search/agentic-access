---
acting_count: 198
action_class_counts:
  acting: 198
api_specs:
- filename: mews-connector-openapi.yaml
  format: yaml
  label: Mews Connector API
  slug: connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mews/refs/heads/main/openapi/mews-connector-openapi.yaml
consequence_counts:
  physical: 27
  safety-critical: 1
  write: 170
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Mews Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/connector/v1/creditCards/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/billingAutomationPaymentPlans/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/commands/addPaymentTerminal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/companionships/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/creditCards/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/customers/getRelationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/loyaltyMemberships/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/loyaltyMemberships/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/loyaltyMemberships/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/loyaltyMemberships/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/orderItems/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/orderItems/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/orders/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/paymentMethodRequests/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/paymentPlans/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/paymentRequests/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/paymentRequests/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/paymentRequests/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/payments/addAlternative
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/payments/addCreditCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/payments/addExternal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/payments/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/payments/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/productServiceOrders/getAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/connector/v1/serviceOrderNotes/add
operation_count: 198
overview: 'Mews exposes 198 API operations that an AI agent could call, of which 198 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 170 write, 27 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mews
provider_slug: mews
slug: mews-agentic-access
source_filename: mews-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mews-connector-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 198\n  by_action_class:\n    acting: 198\n  by_consequence:\n    write: 170\n    physical: 27\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/connector/v1/accountNotes/getAll\n  method: post\n  operationId: accountNotes_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accountNotes/add\n  method: post\n  operationId:\
  \ accountNotes_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accountNotes/update\n  method: post\n  operationId: accountNotes_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accountNotes/delete\n  method: post\n  operationId: accountNotes_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/connector/v1/accountingCategories/getAll\n  method: post\n  operationId: accountingCategories_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accountingItems/update\n  method: post\n  operationId: accountingItems_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accountingItems/getAll\n  method: post\n  operationId: accountingItems_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accounts/update\n  method: post\n  operationId: accounts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accounts/addFile\n  method: post\n  operationId: accounts_addFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/accounts/merge\n  method: post\n  operationId:\
  \ accounts_merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/addresses/getAll\n  method: post\n  operationId: addresses_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/addresses/add\n  method: post\n  operationId: addresses_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/connector/v1/addresses/update\n  method: post\n  operationId: addresses_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/addresses/delete\n  method: post\n  operationId: addresses_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/ageCategories/getAll\n  method: post\n  operationId: ageCategories_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/availabilityAdjustments/getAll\n  method: post\n  operationId: availabilityAdjustments_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/availabilityBlocks/delete\n  method: post\n  operationId: availabilityBlocks_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/availabilityBlocks/getAll\n  method: post\n  operationId:\
  \ availabilityBlocks_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/availabilityBlocks/add\n  method: post\n  operationId: availabilityBlocks_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/availabilityBlocks/update\n  method: post\n  operationId: availabilityBlocks_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/billingAutomations/getAll\n  method: post\n  operationId: billingAutomations_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/billingAutomations/add\n  method: post\n  operationId: billingAutomations_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/billingAutomations/update\n  method: post\n  operationId: billingAutomations_update\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/billingAutomations/updateAssignments\n  method: post\n  operationId: billingAutomations_updateAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/billingAutomations/delete\n  method: post\n  operationId: billingAutomations_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/connector/v1/bills/update\n  method: post\n  operationId: bills_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/bills/getAll\n  method: post\n  operationId: bills_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/bills/getPdf\n  method: post\n  operationId: bills_getPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/bills/add\n  method: post\n  operationId: bills_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/bills/delete\n  method: post\n  operationId: bills_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/bills/close\n  method: post\n  operationId: bills_close\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/businessSegments/getAll\n  method: post\n  operationId: businessSegments_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/cancellationPolicies/getAll\n  method: post\n  operationId: cancellationPolicies_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/cancellationPolicies/getByReservations\n\
  \  method: post\n  operationId: cancellationPolicies_getByReservations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/cancellationPolicies/getByRates\n  method: post\n  operationId: cancellationPolicies_getByRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/cashierTransactions/getAll\n  method: post\n  operationId: cashierTransactions_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/cashiers/getAll\n  method: post\n  operationId: cashiers_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/commands/getAllByIds\n  method: post\n  operationId: commands_getAllByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/commands/getAllActive\n  method: post\n  operationId: commands_getAllActive\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/commands/addPrinter\n  method: post\n  operationId: commands_addPrinter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/commands/addKeyCutter\n  method: post\n  operationId: commands_addKeyCutter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/connector/v1/commands/addPaymentTerminal\n  method: post\n  operationId: commands_addPaymentTerminal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/commands/update\n  method: post\n  operationId: commands_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/fiscalMachineCommands/getAll\n  method: post\n  operationId: fiscalMachineCommands_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companies/add\n  method: post\n  operationId: companies_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companies/update\n  method: post\n  operationId: companies_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companies/getAll\n  method:\
  \ post\n  operationId: companies_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companies/delete\n  method: post\n  operationId: companies_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companionships/getAll\n  method: post\n  operationId: companionships_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companyContracts/getAll\n  method: post\n  operationId: companyContracts_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companyContracts/add\n  method: post\n  operationId: companyContracts_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companyContracts/update\n  method: post\n  operationId: companyContracts_update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/companyContracts/delete\n  method: post\n  operationId: companyContracts_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/configuration/get\n  method: post\n  operationId: configuration_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/connector/v1/counters/getAll\n  method: post\n  operationId: counters_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/countries/getAll\n  method: post\n  operationId: countries_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/creditCards/getAll\n  method: post\n  operationId: creditCards_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/creditCards/addTokenized\n  method: post\n  operationId: creditCards_addTokenized\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/creditCards/charge\n  method: post\n  operationId: creditCards_charge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/creditCards/disable\n  method: post\n  operationId:\
  \ creditCards_disable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/connector/v1/currencies/getAll\n  method: post\n  operationId: currencies_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/getAll\n  method: post\n  operationId: customers_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/search\n  method: post\n  operationId: customers_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/getOpenItems\n  method: post\n  operationId: customers_getOpenItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/add\n  method: post\n  operationId: customers_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/update\n  method: post\n  operationId: customers_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/merge\n  method: post\n  operationId: customers_merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/addFile\n  method: post\n  operationId:\
  \ customers_addFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/customers/getRelationships\n  method: post\n  operationId: customers_getRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/departments/getAll\n  method: post\n  operationId: departments_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/devices/getAll\n  method: post\n  operationId: devices_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/enterprises/getAll\n  method: post\n  operationId: enterprises_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/exchangeRates/getAll\n  method: post\n  operationId: exchangeRates_getAll\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/exports/add\n  method: post\n  operationId: exports_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/exports/getAll\n  method: post\n  operationId: exports_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/identityDocuments/getAll\n\
  \  method: post\n  operationId: identityDocuments_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/identityDocuments/delete\n  method: post\n  operationId: identityDocuments_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/identityDocuments/clear\n  method: post\n  operationId: identityDocuments_clear\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/identityDocuments/update\n  method: post\n  operationId: identityDocuments_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/identityDocuments/add\n  method: post\n  operationId: identityDocuments_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/images/getUrls\n  method: post\n  operationId: images_getUrls\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/languages/getAll\n  method: post\n  operationId: languages_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/languages/getTexts\n  method: post\n  operationId: languages_getTexts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/ledgerBalances/getAll\n\
  \  method: post\n  operationId: ledgerBalances_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/loyaltyMemberships/getAll\n  method: post\n  operationId: loyaltyMemberships_getAll\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/loyaltyMemberships/add\n  method: post\n  operationId: loyaltyMemberships_add\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/loyaltyMemberships/update\n  method: post\n  operationId: loyaltyMemberships_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/connector/v1/loyaltyMemberships/delete\n  method: post\n  operationId: loyaltyMemberships_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n  \n\n# --- truncated at 32 KB (72 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/mews/refs/heads/main/agentic-access/mews-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mews/refs/heads/main/agentic-access/mews-agentic-access.yml
summary_line: 198 operations · 198 acting · 1 human-in-the-loop
tags:
- Hospitality
- Hotels
- PMS
- Property Management
---
