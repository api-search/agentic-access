---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 30
api_specs:
- filename: microsoft-dynamics-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Accounts API
  slug: microsoft-dynamics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-accounts-api-openapi.yml
- filename: microsoft-dynamics-activities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Activities API
  slug: microsoft-dynamics-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-activities-api-openapi.yml
- filename: microsoft-dynamics-cases-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Cases API
  slug: microsoft-dynamics-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-cases-api-openapi.yml
- filename: microsoft-dynamics-companies-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Companies API
  slug: microsoft-dynamics-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-companies-api-openapi.yml
- filename: microsoft-dynamics-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Contacts API
  slug: microsoft-dynamics-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-contacts-api-openapi.yml
- filename: microsoft-dynamics-customers-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Customers API
  slug: microsoft-dynamics-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-customers-api-openapi.yml
- filename: microsoft-dynamics-employees-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Employees API
  slug: microsoft-dynamics-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-employees-api-openapi.yml
- filename: microsoft-dynamics-general-ledger-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics General Ledger API
  slug: microsoft-dynamics-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-general-ledger-api-openapi.yml
- filename: microsoft-dynamics-human-resources-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Human Resources API
  slug: microsoft-dynamics-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-human-resources-api-openapi.yml
- filename: microsoft-dynamics-items-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Items API
  slug: microsoft-dynamics-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-items-api-openapi.yml
- filename: microsoft-dynamics-journals-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Journals API
  slug: microsoft-dynamics-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-journals-api-openapi.yml
- filename: microsoft-dynamics-leads-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Leads API
  slug: microsoft-dynamics-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-leads-api-openapi.yml
- filename: microsoft-dynamics-opportunities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Opportunities API
  slug: microsoft-dynamics-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-opportunities-api-openapi.yml
- filename: microsoft-dynamics-products-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Products API
  slug: microsoft-dynamics-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-products-api-openapi.yml
- filename: microsoft-dynamics-purchase-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Purchase Invoices API
  slug: microsoft-dynamics-purchase-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-purchase-invoices-api-openapi.yml
- filename: microsoft-dynamics-purchase-orders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Purchase Orders API
  slug: microsoft-dynamics-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-purchase-orders-api-openapi.yml
- filename: microsoft-dynamics-sales-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Sales Invoices API
  slug: microsoft-dynamics-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-sales-invoices-api-openapi.yml
- filename: microsoft-dynamics-sales-orders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Sales Orders API
  slug: microsoft-dynamics-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-sales-orders-api-openapi.yml
- filename: microsoft-dynamics-vendors-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Vendors API
  slug: microsoft-dynamics-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-vendors-api-openapi.yml
consequence_counts:
  physical: 6
  read: 30
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Dynamics Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrderHeaders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /SalesOrderHeaders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies({companyId})/purchaseInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies({companyId})/purchaseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies({companyId})/salesInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies({companyId})/salesOrders
operation_count: 59
overview: 'Microsoft Dynamics exposes 59 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 23 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
slug: microsoft-dynamics-agentic-access
source_filename: microsoft-dynamics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-dynamics-business-central-openapi.yml, openapi/microsoft-dynamics-dataverse-openapi.yml,\n  openapi/microsoft-dynamics-finance-operations-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 30\n    acting: 29\n  by_consequence:\n    read: 30\n    write: 23\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/customers({customerId})\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/customers({customerId})\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/customers({customerId})\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/vendors\n  method: get\n  operationId: listVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/vendors\n  method: post\n  operationId: createVendor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/items\n  method: post\n  operationId: createItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/salesOrders\n  method: get\n  operationId: listSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/salesOrders\n  method: post\n  operationId: createSalesOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/salesInvoices\n  method: get\n  operationId: listSalesInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/salesInvoices\n  method: post\n  operationId: createSalesInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /companies({companyId})/purchaseOrders\n  method: get\n  operationId: listPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/purchaseOrders\n  method: post\n  operationId: createPurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/purchaseInvoices\n  method: get\n  operationId: listPurchaseInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/purchaseInvoices\n  method: post\n  operationId:\
  \ createPurchaseInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/generalLedgerEntries\n  method: get\n  operationId: listGeneralLedgerEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/journals\n  method: get\n  operationId: listJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/journals\n  method: post\n  operationId: createJournal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies({companyId})/employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies({companyId})/employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts({accountid})\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts({accountid})\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts({accountid})\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts({contactid})\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts({contactid})\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts({contactid})\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads({leadid})\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads({leadid})\n  method: patch\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads({leadid})\n  method: delete\n  operationId: deleteLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities\n  method: get\n  operationId: listOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: post\n  operationId: createOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /opportunities({opportunityid})\n  method: get\n  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities({opportunityid})\n  method: patch\n  operationId: updateOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities({opportunityid})\n  method: delete\n  operationId: deleteOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /incidents\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customers\n  method: post\n\
  \  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Vendors\n  method: get\n  operationId: listVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Vendors\n  method: post\n  operationId: createVendor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ReleasedProducts\n  method: get\n  operationId: listReleasedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ReleasedProducts\n  method: post\n  operationId: createReleasedProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SalesOrderHeaders\n  method: get\n  operationId: listSalesOrderHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrderHeaders\n  method: post\n  operationId: createSalesOrderHeader\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PurchaseOrderHeaders\n  method: get\n  operationId: listPurchaseOrderHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PurchaseOrderHeaders\n  method: post\n  operationId: createPurchaseOrderHeader\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GeneralJournalAccountEntries\n  method: get\n  operationId: listGeneralJournalAccountEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Workers\n \
  \ method: get\n  operationId: listWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/agentic-access/microsoft-dynamics-agentic-access.yml
summary_line: 59 operations · 29 acting
tags:
- CRM
- ERP
- Microsoft Dynamics
---
