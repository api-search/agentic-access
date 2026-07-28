---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 35
api_specs:
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy CDR Energy API
  slug: origin-energy-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: consumer-data-standards-common-api-openapi.json
  format: json
  label: Origin Energy CDR Public Discovery API
  slug: origin-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-common-api-openapi.json
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy Plan Reference Data API (AER Energy Made Easy)
  slug: origin-energy-plan-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: origin-energy-kraken-default-openapi.yml
  format: yaml
  label: Origin Energy Kraken REST API
  slug: origin-energy-kraken-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/origin-energy-kraken-default-openapi.yml
consequence_counts:
  physical: 5
  read: 35
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Origin Energy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /energy/accounts/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_number}/payments/ad-hoc/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/data-import/business-payment-instruction/create/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/data-import/payment-instruction/create/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/
operation_count: 54
overview: 'Origin Energy exposes 54 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 14 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Origin Energy
provider_slug: origin-energy
slug: origin-energy-agentic-access
source_filename: origin-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/consumer-data-standards-common-api-openapi.json, openapi/consumer-data-standards-energy-api-openapi.json,\n  openapi/origin-energy-kraken-data-import-openapi.yml, openapi/origin-energy-kraken-default-openapi.yml,\n  openapi/origin-energy-kraken-orders-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 35\n    acting: 19\n  by_consequence:\n    read: 35\n    write: 14\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /common/customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /common/customer/detail\n  method: get\n  operationId: getCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/outages\n  method: get\n  operationId: getOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans\n  method: get\n  operationId: listEnergyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans/{planId}\n  method: get\n  operationId: getEnergyPlanDetail\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints\n  method: get\n  operationId: listElectricityServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}\n  method: get\n  operationId: getElectricityServicePointDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/usage\n  method: get\n  operationId: getElectricityServicePointUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method: get\n  operationId: listElectricityUsageBulk\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method: post\n  operationId: listElectricityUsageForServicePoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/electricity/servicepoints/{servicePointId}/der\n  method: get\n  operationId: getElectricityDERForServicePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: get\n  operationId: listElectricityDERBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: post\n  operationId: listElectricityDERForSpecificServicePoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/accounts\n  method: get\n  operationId: listEnergyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}\n  method: get\n  operationId: getEnergyAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/payment-schedule\n  method: get\n  operationId:\
  \ getEnergyAccountPaymentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/concessions\n  method: get\n  operationId: getEnergyAccountConcessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/balance\n  method: get\n  operationId: getEnergyAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: get\n  operationId: listEnergyAccountBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: post\n  operationId: listEnergyAccountBalancesSpecificAccounts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/accounts/{accountId}/invoices\n  method: get\n  operationId: getEnergyAccountInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: get\n  operationId: listEnergyAccountInvoicesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: post\n  operationId: listEnergyInvoicesForSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/accounts/{accountId}/billing\n  method: get\n  operationId: getBillingForEnergyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: get\n  operationId: listEnergyAccountBillingBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: post\n  operationId: listEnergyAccountBillingForSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/account-import-process/create-or-update/\n  method: post\n  operationId: V1 Create Or Update Account Import Process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/account-import-process/process/\n  method: post\n  operationId: V1 Process Account Import Process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/account-transfer-status/{import_supplier_code}/{external_account_number}/\n  method:\
  \ get\n  operationId: V1 Get Account Transfer Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/all-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get All Account Import Processes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/business/\n  method: post\n  operationId: V1 Create Business\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/business-payment-instruction/create/\n  method: post\n  operationId: V1 Create Business Payment Instruction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/historical-statements/create/\n  method: post\n  operationId: V1 Create Historical Statements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/imported-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get Imported Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/data-import/notes/create/\n  method: post\n  operationId: V1 Create Account Notes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/payment-instruction/create/\n  method: post\n  operationId: V1 Create Payment Instruction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/pending-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get Pending Account Import Processes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/transactions/create/\n  method: post\n  operationId: V1 Create Transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/validate-account/\n  method: post\n  operationId: V1 Validate Account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-import/accounts/\n  method: post\n  operationId: V2 Schedule Account Creation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-import/accounts/{import_supplier_code}/{external_identifier}/\n  method: get\n  operationId: V2 Account Import Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data-import/accounts/validate/\n  method: post\n  operationId: V2 Validate Account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-import/schema/\n  method: get\n  operationId: Data Import Open Api Schema\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-client-healthcheck/\n  method: get\n  operationId: External Client Health Check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-events/schema/\n  method: get\n  operationId: Open Api Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_number}/payments/ad-hoc/\n  method: post\n  operationId: Ad Hoc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/energetiq-public-key/\n  method: get\n  operationId: Get Energetiq Public Key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unbundled-network-charges/energetiq-public-key/\n  method: get\n  operationId: Get Energetiq Public Key_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voice/twilio/enqueue-audio/\n  method: post\n  operationId: Twilio Enqueue Audio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voice/twilio/voice-announcement/\n  method: get\n  operationId: Voice Announcement\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/schema/\n  method: get\n  operationId: Order Management Open Api Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/\n  method: post\n  operationId: V2 Schedule Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{external_order_id}/\n  method: get\n  operationId: V2 Order Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/agentic-access/origin-energy-agentic-access.yml
summary_line: 54 operations · 19 acting
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- Smart Metering
- Solar
- DER
- Demand Response
- Energy Markets
---
