---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 22
api_specs:
- filename: simply-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Simply Energy Data Holder Customers API
  slug: simply-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-data-holder-customers-api-openapi.yml
- filename: simply-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Simply Energy Data Holder Operations API
  slug: simply-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-data-holder-operations-api-openapi.yml
- filename: simply-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Simply Energy Distributed Energy Resources API
  slug: simply-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-distributed-energy-resources-api-openapi.yml
- filename: simply-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Simply Energy Electricity Service Points API
  slug: simply-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-electricity-service-points-api-openapi.yml
- filename: simply-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Simply Energy Electricity Usage API
  slug: simply-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-electricity-usage-api-openapi.yml
- filename: simply-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Account Balances API
  slug: simply-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-account-balances-api-openapi.yml
- filename: simply-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Account Billing API
  slug: simply-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-account-billing-api-openapi.yml
- filename: simply-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Accounts API
  slug: simply-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-accounts-api-openapi.yml
- filename: simply-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Plans API
  slug: simply-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-plans-api-openapi.yml
consequence_counts:
  physical: 1
  read: 22
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simply Energy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /energy/accounts/invoices
operation_count: 27
overview: 'Simply Energy exposes 27 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simply Energy
provider_slug: simply-energy
slug: simply-energy-agentic-access
source_filename: simply-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/simply-energy-cds-common-openapi.yml, openapi/simply-energy-cds-energy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 22\n    acting: 5\n  by_consequence:\n    read: 22\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /common/customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /common/customer/detail\n  method: get\n  operationId: getCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/outages\n  method: get\n  operationId: getOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans\n  method: get\n  operationId: listEnergyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans/{planId}\n  method: get\n  operationId: getEnergyPlanDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints\n  method: get\n  operationId: listElectricityServicePoints\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}\n  method: get\n  operationId: getElectricityServicePointDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/usage\n  method: get\n  operationId: getElectricityServicePointUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method: get\n  operationId: listElectricityUsageBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method:\
  \ post\n  operationId: listElectricityUsageForServicePoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/electricity/servicepoints/{servicePointId}/der\n  method: get\n  operationId: getElectricityDERForServicePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: get\n  operationId: listElectricityDERBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: post\n  operationId: listElectricityDERForSpecificServicePoints\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/accounts\n  method: get\n  operationId: listEnergyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}\n  method: get\n  operationId: getEnergyAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/payment-schedule\n  method: get\n  operationId: getEnergyAccountPaymentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/concessions\n\
  \  method: get\n  operationId: getEnergyAccountConcessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/balance\n  method: get\n  operationId: getEnergyAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: get\n  operationId: listEnergyAccountBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: post\n  operationId: listEnergyAccountBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /energy/accounts/{accountId}/invoices\n  method: get\n  operationId: getEnergyAccountInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: get\n  operationId: listEnergyAccountInvoicesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: post\n  operationId: listEnergyInvoicesForSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /energy/accounts/{accountId}/billing\n  method: get\n  operationId: getBillingForEnergyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: get\n  operationId: listEnergyAccountBillingBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: post\n  operationId: listEnergyAccountBillingForSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/agentic-access/simply-energy-agentic-access.yml
summary_line: 27 operations · 5 acting
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Smart Metering
- Energy Markets
---
