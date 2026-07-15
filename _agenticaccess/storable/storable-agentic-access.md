---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 37
api_specs:
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tenants API
  slug: storable-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Units & Rate Management API
  slug: storable-units-rate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Ledgers & Payments API
  slug: storable-ledgers-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Leads & Reservations API
  slug: storable-leads-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Move Ins & Move Outs API
  slug: storable-move-ins-move-outs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Gate Access API
  slug: storable-gate-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Insurance API
  slug: storable-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tasks API
  slug: storable-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Documents & eSign API
  slug: storable-documents-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Delinquency & Auctions API
  slug: storable-delinquency-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Reporting API
  slug: storable-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
consequence_counts:
  physical: 4
  read: 37
  safety-critical: 1
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Storable Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /{facility_id}/ledgers/{ledger_id}/update_autopay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{facility_id}/authorize_funds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{facility_id}/documents/{event_id}/send_esignable_documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{facility_id}/ledgers/{ledger_id}/make_payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{facility_id}/tenants/{tenant_id}/payment_methods
operation_count: 69
overview: 'Storable exposes 69 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 27 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Storable
provider_slug: storable
slug: storable-agentic-access
source_filename: storable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/storable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 37\n    acting: 32\n  by_consequence:\n    read: 37\n    write: 27\n    physical: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /{facility_id}/tenants\n  method: get\n  operationId: listTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/tenants/{id}\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{facility_id}/tenants/{id}\n  method: patch\n  operationId: updateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/tenants/search\n  method: get\n  operationId: searchTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/tenants/{tenant_id}/preferences\n  method: get\n  operationId: getTenantPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/tenants/{tenant_id}/preferences\n  method: put\n  operationId: updateTenantPreferences\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/tenants/{tenant_id}/notes\n  method: post\n  operationId: createTenantNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/tenants/sign_in\n  method: post\n  operationId: tenantSignIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/units\n\
  \  method: get\n  operationId: listUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/units\n  method: post\n  operationId: createUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/units/available\n  method: get\n  operationId: listAvailableUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/units/bulk_create\n  method: post\n  operationId: bulkCreateUnits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/units/bulk_update\n  method: put\n  operationId: bulkUpdateUnits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/units/rate_history\n  method: get\n  operationId: getUnitRateHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/units/{unit_id}/future_scheduled_rates\n  method: get\n  operationId: getFutureScheduledRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /{facility_id}/unit_groups\n  method: get\n  operationId: listUnitGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/unit_groups\n  method: post\n  operationId: createUnitGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/unit_group_tier_rates\n  method: get\n  operationId: listUnitGroupTierRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/unit_group_tier_rates/update\n  method: put\n  operationId: updateUnitGroupTierRates\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/discount_plans\n  method: get\n  operationId: listDiscountPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/ledgers\n  method: get\n  operationId: listLedgers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/ledgers/{id}\n  method: get\n  operationId: getLedger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/ledgers/{ledger_id}/make_payment\n  method: post\n  operationId: makeLedgerPayment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/ledgers/{ledger_id}/update_autopay\n  method: put\n  operationId: updateLedgerAutopay\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{facility_id}/tenants/{tenant_id}/payment_methods\n  method: get\n  operationId: listTenantPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{facility_id}/tenants/{tenant_id}/payment_methods\n  method: post\n  operationId: createTenantPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/payment_intents\n  method: get\n  operationId: listPaymentIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/invoiceable_items\n  method: get\n  operationId:\
  \ listInvoiceableItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/authorize_funds\n  method: post\n  operationId: authorizeFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/leads/{id}\n  method: patch\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/leads/{id}\n  method: delete\n  operationId: deleteLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/leads/reservations\n  method: get\n  operationId: listReservationLeads\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/leads/waitlist\n  method: get\n  operationId: listWaitlistLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/leads\n  method: get\n  operationId: listCompanyLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/move_ins\n  method: get\n  operationId: listMoveIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/move_ins/review_cost\n  method: post\n  operationId: reviewMoveInCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/move_ins/process_move_in\n  method: post\n  operationId: processMoveIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/move_outs\n  method: get\n  operationId: listMoveOuts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/move_outs/reasons\n  method: get\n  operationId: listMoveOutReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/move_outs/schedule_move_out\n\
  \  method: post\n  operationId: scheduleMoveOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/move_outs/process_move_out\n  method: post\n  operationId: processMoveOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/gate_codes/availability_check\n  method: post\n  operationId: checkGateCodeAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/gate_codes/open\n  method: post\n  operationId: openGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/access_points\n  method: get\n  operationId: listAccessPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/gate_activities\n  method: post\n  operationId: logGateActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{facility_id}/insurance/summary\n  method: get\n  operationId: getInsuranceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/insurance/activity\n  method: get\n  operationId: getInsuranceActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/insurance/tenant_auto_enroll_settings\n  method: put\n  operationId: updateTenantAutoEnrollSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/tasks/{id}/complete\n  method: put\n  operationId: completeTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/units/{unit_id}/tasks\n  method: get\n  operationId: listUnitTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/units/{unit_id}/tasks\n  method: post\n  operationId: createUnitTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/events/{event_id}/documents\n  method: get\n  operationId: listEventDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/documents/{event_id}/send_esignable_documents\n  method:\
  \ post\n  operationId: sendEsignableDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/events/{event_id}/esign\n  method: post\n  operationId: esignEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/delinquency_events\n  method: get\n  operationId: listDelinquencyEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/delinquency_events/{id}\n\
  \  method: get\n  operationId: getDelinquencyEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/delinquency_events/{id}/{verb}\n  method: patch\n  operationId: transitionDelinquencyEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/auctions/scheduled\n  method: get\n  operationId: listScheduledAuctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/active_auctions\n  method: get\n  operationId: listActiveCompanyAuctions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/report_requests\n  method: post\n  operationId: createFacilityReportRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{facility_id}/report_requests/{id}\n  method: get\n  operationId: getFacilityReportRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{facility_id}/report_requests/{id}/completed_json\n  method: get\n  operationId: getFacilityReportRequestResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/report_requests\n\
  \  method: post\n  operationId: createCompanyReportRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/agentic-access/storable-agentic-access.yml
summary_line: 69 operations · 32 acting · 1 human-in-the-loop
tags:
- Self Storage
- Property Management
- Facility Management
- Tenants
- Reservations
- Payments
- SiteLink
- storEDGE
- SpareFoot
---
