---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 25
api_specs:
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Companies API
  slug: simpro-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Customers API
  slug: simpro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Sites API
  slug: simpro-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Jobs API
  slug: simpro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Quotes API
  slug: simpro-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Invoices API
  slug: simpro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Schedules API
  slug: simpro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Vendor Orders API
  slug: simpro-vendor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Cost Centers API
  slug: simpro-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Stock API
  slug: simpro-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Webhooks API
  slug: simpro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
consequence_counts:
  physical: 6
  read: 25
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simpro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{companyID}/invoices/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /companies/{companyID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /companies/{companyID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{companyID}/vendorOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /companies/{companyID}/vendorOrders/{vendorOrderID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /companies/{companyID}/vendorOrders/{vendorOrderID}
operation_count: 52
overview: 'Simpro exposes 52 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 21 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simpro
provider_slug: simpro
slug: simpro-agentic-access
source_filename: simpro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/simpro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 25\n    acting: 27\n  by_consequence:\n    read: 25\n    write: 21\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /companies/\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/\n\
  \  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/companies/\n  method: get\n  operationId: listCompanyCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/companies/\n  method: post\n  operationId: createCompanyCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/customers/companies/{customerID}\n  method: get\n  operationId: getCompanyCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/companies/{customerID}\n  method: patch\n  operationId: updateCompanyCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/customers/companies/{customerID}\n  method: delete\n  operationId: deleteCompanyCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/customers/individuals/\n  method: get\n  operationId: listIndividualCustomers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/individuals/\n  method: post\n  operationId: createIndividualCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/customers/individuals/{customerID}\n  method: get\n  operationId: getIndividualCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/customers/individuals/{customerID}\n  method: patch\n  operationId: updateIndividualCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/customers/individuals/{customerID}\n  method: delete\n  operationId: deleteIndividualCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/sites/\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/sites/\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/sites/{siteID}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/sites/{siteID}\n  method: patch\n  operationId: updateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/sites/{siteID}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/jobs/\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/jobs/\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/jobs/{jobID}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/jobs/{jobID}\n  method:\
  \ patch\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/jobs/{jobID}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/quotes/\n  method: get\n  operationId: listQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/quotes/\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/quotes/{quoteID}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/quotes/{quoteID}\n  method: patch\n  operationId: updateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/quotes/{quoteID}\n  method: delete\n  operationId: deleteQuote\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/invoices/\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/invoices/\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/invoices/{invoiceID}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/invoices/{invoiceID}\n  method: patch\n  operationId: updateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/invoices/{invoiceID}\n  method: delete\n  operationId: deleteInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/schedules/\n\
  \  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/schedules/{scheduleID}\n  method: get\n  operationId: getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/vendorOrders/\n  method: get\n  operationId: listVendorOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/vendorOrders/\n  method: post\n  operationId: createVendorOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/vendorOrders/{vendorOrderID}\n  method: get\n  operationId: getVendorOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/vendorOrders/{vendorOrderID}\n  method: patch\n  operationId: updateVendorOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/vendorOrders/{vendorOrderID}\n  method: delete\n  operationId: deleteVendorOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/setup/accounts/costCenters/\n  method: get\n  operationId: listCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/setup/accounts/costCenters/\n  method: post\n  operationId: createCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/setup/accounts/costCenters/{costCenterID}\n  method: get\n  operationId: getCostCenter\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/setup/accounts/costCenters/{costCenterID}\n  method: patch\n  operationId: updateCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/setup/accounts/costCenters/{costCenterID}\n  method: delete\n  operationId: deleteCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/storageDevices/{storageDeviceID}/stock/\n\
  \  method: get\n  operationId: listStock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/storageDevices/{storageDeviceID}/stock/{catalogID}\n  method: get\n  operationId: getStockItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/setup/webhooks/\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/setup/webhooks/\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/setup/webhooks/{webhookID}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyID}/setup/webhooks/{webhookID}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyID}/setup/webhooks/{webhookID}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/agentic-access/simpro-agentic-access.yml
summary_line: 52 operations · 27 acting
tags:
- Field Service Management
- Trades
- Job Management
- Project Management
- Scheduling
- Inventory
- Estimating
- Workforce
- SaaS
- Contractors
---
