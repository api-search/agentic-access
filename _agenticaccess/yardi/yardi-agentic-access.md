---
acting_count: 13
action_class_counts:
  acting: 13
api_specs:
- filename: yardi-voyager-api-openapi.yml
  format: yaml
  label: Yardi Voyager API
  slug: yardi-voyager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/openapi/yardi-voyager-api-openapi.yml
consequence_counts:
  physical: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yardi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfResidentTransactions20.asmx/GetBudgetData_Login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfResidentTransactions20.asmx/GetResidentTransactions_ByChargeDate_Login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfResidentTransactions20.asmx/GetResidentTransactions_Login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfResidentTransactions20.asmx/ImportResidentTransactions_Login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfVendorInvoice.asmx/GetVendorInvoices_Login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ItfVendorInvoice.asmx/ImportVendorInvoices_Login
operation_count: 13
overview: 'Yardi exposes 13 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 write and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yardi
provider_slug: yardi
slug: yardi-agentic-access
source_filename: yardi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yardi-voyager-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 13\n  by_consequence:\n    physical: 6\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ItfResidentTransactions20.asmx/GetResidentTransactions_Login\n  method: post\n  operationId: getResidentTransactionsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfResidentTransactions20.asmx/GetResidentTransactions_ByChargeDate_Login\n\
  \  method: post\n  operationId: getResidentTransactionsByChargeDateLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfResidentTransactions20.asmx/ImportResidentTransactions_Login\n  method: post\n  operationId: importResidentTransactionsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfResidentTransactions20.asmx/GetBudgetData_Login\n  method: post\n  operationId: getBudgetDataLogin\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfCommonData.asmx/GetPropertyConfigurations_Login\n  method: post\n  operationId: getPropertyConfigurationsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfCommonData.asmx/GetUnitInformation_Login\n  method: post\n  operationId: getUnitInformationLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfCommonData.asmx/GetTenants_Login\n  method: post\n  operationId: getTenantsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfCommonData.asmx/GetChartOfAccounts_Login\n  method: post\n  operationId: getChartOfAccountsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfServiceRequests.asmx/GetServiceRequests_Login\n  method: post\n  operationId: getServiceRequestsLogin\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfServiceRequests.asmx/ImportServiceRequests_Login\n  method: post\n  operationId: importServiceRequestsLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfVendorInvoice.asmx/GetVendorInvoices_Login\n  method: post\n  operationId: getVendorInvoicesLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfVendorInvoice.asmx/ImportVendorInvoices_Login\n  method: post\n  operationId: importVendorInvoicesLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ItfJobCost.asmx/GetJobCostData_Login\n  method: post\n  operationId: getJobCostDataLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/agentic-access/yardi-agentic-access.yml
summary_line: 13 operations · 13 acting
tags:
- Accounting
- Commercial Real Estate
- Coworking
- Investment Management
- Multifamily
- Property Management
- Real Estate
- Residential
- Self Storage
- Senior Living
---
