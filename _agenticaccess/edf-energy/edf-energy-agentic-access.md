---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 25
api_specs:
- filename: edf-energy-kraken-openapi.yml
  format: yaml
  label: EDF Kraken REST API
  slug: edf-kraken-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-kraken-openapi.yml
- filename: edf-energy-kraken-data-import-openapi.yml
  format: yaml
  label: EDF Kraken Customer Migration (Data Import) API
  slug: edf-kraken-customer-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-kraken-data-import-openapi.yml
consequence_counts:
  physical: 5
  read: 25
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edf Energy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/data-import/payment-instruction/create/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/data-import/send-registration-flows/{import_supplier_code}/{external_account_number}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-intents/confirm/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-intents/create/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-intents/fail/
operation_count: 43
overview: 'EDF Energy exposes 43 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 13 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EDF Energy
provider_slug: edf-energy
slug: edf-energy-agentic-access
source_filename: edf-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/edf-energy-kraken-data-import-openapi.yml, openapi/edf-energy-kraken-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 18\n    connected: 25\n  by_consequence:\n    write: 13\n    read: 25\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/data-import/account-import-process/create-or-update/\n  method: post\n  operationId: V1 Create Or Update Account Import Process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/data-import/account-import-process/process/\n  method: post\n  operationId: V1 Process Account Import Process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/account-transfer-status/{import_supplier_code}/{external_account_number}/\n  method: get\n  operationId: V1 Get Account Transfer Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/all-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get All Account Import Processes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/data-import/historical-statements/create/\n  method: post\n  operationId: V1 Create Historical Statements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/imported-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get Imported Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/meterpoint-statuses-for-account/{import_supplier_code}/{external_account_number}/\n  method: get\n  operationId: V1 Get Meter Point Statuses For Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/data-import/notes/create/\n  method: post\n  operationId: V1 Create Account Notes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/payment-instruction/create/\n  method: post\n  operationId: V1 Create Payment Instruction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/pending-account-import-processes/{import_supplier_code}/\n  method: get\n  operationId: V1 Get Pending Account Import Processes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-import/send-registration-flows/{import_supplier_code}/{external_account_number}/\n  method: post\n  operationId: V1 Send Registration Flows\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data-import/transactions/create/\n  method: post\n  operationId: V1 Create Transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/data-import/validate-account/\n  method: post\n  operationId: V1 Validate Account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-import/accounts/\n  method: post\n  operationId: V2 Schedule Account Creation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-import/accounts/{import_supplier_code}/{external_identifier}/\n  method: get\n  operationId: V2 Account Import Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/data-import/accounts/validate/\n  method: post\n  operationId: V2 Validate Account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-import/schema/\n  method: get\n  operationId: Data Import Open Api Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-client-healthcheck/\n  method: get\n  operationId: External Client Health Check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-events/schema/\n  method: get\n  operationId: Open Api Schema\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/\n  method: post\n  operationId: Create an account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_number}/tariff-renewal/\n  method: post\n  operationId: Renew a business tariff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/electricity-meter-points/{mpan}/\n  method: get\n  operationId: Get Electricity Meter Point\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/electricity-meter-points/{mpan}/meters/{serial_number}/consumption/\n  method: get\n  operationId: List consumption for an electricity meter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gas-meter-points/{mprn}/meters/{serial_number}/consumption/\n  method: get\n  operationId: List consumption for a gas meter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/industry/grid-supply-points/\n  method: get\n  operationId: List Industry Grid Supply Points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-intents/confirm/\n  method: post\n  operationId: Confirm a Stripe\
  \ payment intent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment-intents/create/\n  method: post\n  operationId: Create a Stripe payment intent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment-intents/fail/\n  method: post\n  operationId: Mark a Stripe payment intent as failed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products/\n  method: get\n  operationId: List Products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/\n  method: get\n  operationId: Product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/day-unit-rates/\n  method: get\n  operationId: Electricity Tariff Day Unit Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/ev-device-off-peak-unit-rates/\n\
  \  method: get\n  operationId: Electricity Tariff Ev Device Off Peak Unit Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/ev-device-peak-unit-rates/\n  method: get\n  operationId: Electricity Tariff Ev Device Peak Unit Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/night-unit-rates/\n  method: get\n  operationId: Electricity Tariff Night Unit Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/standard-unit-rates/\n  method: get\n  operationId: Electricity Tariff Standard Unit\
  \ Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/electricity-tariffs/{tariff_code}/standing-charges/\n  method: get\n  operationId: Electricity Tariff Standing Charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/gas-tariffs/{tariff_code}/standard-unit-rates/\n  method: get\n  operationId: Gas Tariff Standard Unit Rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_code}/gas-tariffs/{tariff_code}/standing-charges/\n  method: get\n  operationId: Gas Tariff Standing Charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v1/quotes/\n  method: post\n  operationId: Create a quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/{code}/products/{product_id}/\n  method: post\n  operationId: Share a quote via email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voice/twilio/enqueue-audio/\n  method: post\n  operationId: Twilio Enqueue Audio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voice/twilio/voice-announcement/\n  method: get\n  operationId: Voice Announcement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/schema/\n  method: get\n  operationId: Order Management Open Api Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/agentic-access/edf-energy-agentic-access.yml
summary_line: 43 operations · 18 acting
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Energy Supplier
- Smart Metering
- Nuclear
- Renewables
- EV Charging
- Demand Response
- Tariffs
- Energy Markets
---
