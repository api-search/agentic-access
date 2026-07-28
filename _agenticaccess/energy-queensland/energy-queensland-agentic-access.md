---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: energy-queensland-cds-energy-openapi.yml
  format: yaml
  label: Ergon Energy Retail CDR Energy Product Reference Data API
  slug: ergon-energy-retail-cdr-energy-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-cds-energy-openapi.yml
- filename: energy-queensland-cds-common-openapi.yml
  format: yaml
  label: Ergon Energy Retail CDR Discovery API
  slug: ergon-energy-retail-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-cds-common-openapi.yml
- filename: energy-queensland-cds-energy-openapi.yml
  format: yaml
  label: Ergon Energy Retail CDR Energy Consumer Data API
  slug: ergon-energy-retail-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-cds-energy-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Energy Queensland Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Energy Queensland exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Energy Queensland
provider_slug: energy-queensland
slug: energy-queensland-agentic-access
source_filename: energy-queensland-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/energy-queensland-cds-common-openapi.yml, openapi/energy-queensland-cds-energy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\n  anonymously_callable: 4\n  accreditation_gated: 23\noperations:\n- path: /common/customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /common/customer/detail\n  method: get\n  operationId: getCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/outages\n  method: get\n  operationId: getOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts\n  method: get\n  operationId: listEnergyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method: get\n  operationId: listEnergyAccountBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/balances\n  method:\
  \ post\n  operationId: listEnergyAccountBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n  note: Corrected from the heuristic classification. This is a POST only because the Consumer Data Standards\n    use a request body to carry a list of account or service point ids; the operation retrieves data and\n    creates, updates or deletes nothing. The whole CDR energy surface is read-only.\n- path: /energy/accounts/billing\n  method: get\n  operationId: listEnergyAccountBillingBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/billing\n  method: post\n  operationId: listEnergyAccountBillingForSpecificAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n  note: Corrected from the heuristic classification. This is a POST only because the Consumer Data Standards\n    use a request body to carry a list of account or service point ids; the operation retrieves data and\n    creates, updates or deletes nothing. The whole CDR energy surface is read-only.\n- path: /energy/accounts/invoices\n  method: get\n  operationId: listEnergyAccountInvoicesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/invoices\n  method: post\n  operationId: listEnergyInvoicesForSpecificAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n  note: Corrected from the heuristic classification. This is a POST only because the Consumer Data Standards\n    use a request body to\
  \ carry a list of account or service point ids; the operation retrieves data and\n    creates, updates or deletes nothing. The whole CDR energy surface is read-only.\n- path: /energy/accounts/{accountId}\n  method: get\n  operationId: getEnergyAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/balance\n  method: get\n  operationId: getEnergyAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/billing\n  method: get\n  operationId: getBillingForEnergyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/concessions\n  method: get\n  operationId: getEnergyAccountConcessions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/invoices\n  method: get\n  operationId: getEnergyAccountInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/accounts/{accountId}/payment-schedule\n  method: get\n  operationId: getEnergyAccountPaymentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints\n  method: get\n  operationId: listElectricityServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: get\n  operationId: listElectricityDERBulk\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/der\n  method: post\n  operationId: listElectricityDERForSpecificServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n  note: Corrected from the heuristic classification. This is a POST only because the Consumer Data Standards\n    use a request body to carry a list of account or service point ids; the operation retrieves data and\n    creates, updates or deletes nothing. The whole CDR energy surface is read-only.\n- path: /energy/electricity/servicepoints/usage\n  method: get\n  operationId: listElectricityUsageBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/usage\n\
  \  method: post\n  operationId: listElectricityUsageForServicePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n  note: Corrected from the heuristic classification. This is a POST only because the Consumer Data Standards\n    use a request body to carry a list of account or service point ids; the operation retrieves data and\n    creates, updates or deletes nothing. The whole CDR energy surface is read-only.\n- path: /energy/electricity/servicepoints/{servicePointId}\n  method: get\n  operationId: getElectricityServicePointDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/der\n  method: get\n  operationId: getElectricityDERForServicePoint\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/electricity/servicepoints/{servicePointId}/usage\n  method: get\n  operationId: getElectricityServicePointUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans\n  method: get\n  operationId: listEnergyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy/plans/{planId}\n  method: get\n  operationId: getEnergyPlanDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\ncurated_by: API Evangelist\ncuration_note: 'The mechanical heuristic classified the five POST operations as acting/write (one as physical,\n  on a billing keyword match). All five were re-classified\
  \ to connected/read after reading the specification:\n  CDR energy exposes no write operation at all. Everything else is as derived. Consequence classes here\n  are about DATA SENSITIVITY, not physical effect - nothing on this surface can switch, dispatch or control\n  anything on the electricity network, because the network businesses (Energex, Ergon Energy Network)\n  publish no API whatsoever.'\naccess_note: Only four of the 27 operations (listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages)\n  are reachable by any agent without ACCC Consumer Data Right accreditation, mutual TLS and a per-consumer\n  consent. The remaining 23 cannot be called by an autonomous agent at all unless it operates inside an\n  accredited data recipient.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/agentic-access/energy-queensland-agentic-access.yml
summary_line: 27 operations
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Queensland
- Smart Metering
- Solar
- DER
- Open Data
---
