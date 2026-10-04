---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: red-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Customers API
  slug: red-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-customers-api-openapi.yml
- filename: red-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Operations API
  slug: red-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-operations-api-openapi.yml
- filename: red-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Red Energy Distributed Energy Resources API
  slug: red-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-distributed-energy-resources-api-openapi.yml
- filename: red-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Service Points API
  slug: red-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-service-points-api-openapi.yml
- filename: red-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Usage API
  slug: red-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-usage-api-openapi.yml
- filename: red-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Red Energy Account Balances API
  slug: red-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-balances-api-openapi.yml
- filename: red-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Red Energy Account Billing API
  slug: red-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-billing-api-openapi.yml
- filename: red-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Red Energy Accounts API
  slug: red-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-accounts-api-openapi.yml
- filename: red-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Red Energy Plans API
  slug: red-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-plans-api-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Red Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Red Energy exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Red Energy
provider_slug: red-energy
slug: red-energy-agentic-access
source_filename: red-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/red-energy-data-holder-customers-api-openapi.yml, openapi/red-energy-data-holder-operations-api-openapi.yml,\n  openapi/red-energy-distributed-energy-resources-api-openapi.yml, openapi/red-energy-electricity-service-points-api-openapi.yml,\n  openapi/red-energy-electricity-usage-api-openapi.yml, openapi/red-energy-energy-account-balances-api-openapi.yml,\n  openapi/red-energy-energy-account-billing-api-openapi.yml, openapi/red-energy-energy-accounts-api-openapi.yml,\n  openapi/red-energy-energy-plans-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n\
  - path: /common/customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /common/customer/detail\n  method: get\n  operationId: getCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/outages\n  method: get\n  operationId: getOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: get\n  operationId: listElectricityDERBulk\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: post\n  operationId: listElectricityDERForSpecificServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/der\n  method: get\n  operationId: getElectricityDERForServicePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints\n  method: get\n  operationId: listElectricityServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}\n  method: get\n  operationId: getElectricityServicePointDetail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method: get\n  operationId: listElectricityUsageBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n  method: post\n  operationId: listElectricityUsageForServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/usage\n  method: get\n  operationId: getElectricityServicePointUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: get\n  operationId:\
  \ listEnergyAccountBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: post\n  operationId: listEnergyAccountBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/balance\n  method: get\n  operationId: getEnergyAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: get\n  operationId: listEnergyAccountBillingBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: post\n  operationId: listEnergyAccountBillingForSpecificAccounts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: get\n  operationId: listEnergyAccountInvoicesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: post\n  operationId: listEnergyInvoicesForSpecificAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/billing\n  method: get\n  operationId: getBillingForEnergyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/invoices\n  method: get\n  operationId: getEnergyAccountInvoices\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts\n  method: get\n  operationId: listEnergyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}\n  method: get\n  operationId: getEnergyAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/concessions\n  method: get\n  operationId: getEnergyAccountConcessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/payment-schedule\n  method: get\n  operationId: getEnergyAccountPaymentSchedule\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans\n  method: get\n  operationId: listEnergyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans/{planId}\n  method: get\n  operationId: getEnergyPlanDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/agentic-access/red-energy-agentic-access.yml
summary_line: 27 operations
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Open Data
---
