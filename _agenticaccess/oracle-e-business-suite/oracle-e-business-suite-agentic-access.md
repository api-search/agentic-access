---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 38
api_specs:
- filename: isg-rest-api.yml
  format: yaml
  label: Oracle EBS Integrated SOA Gateway REST API
  slug: oracle-ebs-integrated-soa-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/isg-rest-api.yml
- filename: financial-services-api.yml
  format: yaml
  label: Oracle EBS Financial Services API
  slug: oracle-ebs-financial-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/financial-services-api.yml
- filename: supply-chain-api.yml
  format: yaml
  label: Oracle EBS Supply Chain Management API
  slug: oracle-ebs-supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/supply-chain-api.yml
- filename: human-resources-api.yml
  format: yaml
  label: Oracle EBS Human Resources API
  slug: oracle-ebs-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/human-resources-api.yml
- filename: manufacturing-api.yml
  format: yaml
  label: Oracle EBS Manufacturing API
  slug: oracle-ebs-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/manufacturing-api.yml
- filename: ecommerce-gateway-api.yml
  format: yaml
  label: Oracle EBS e-Commerce Gateway API
  slug: oracle-ebs-e-commerce-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/ecommerce-gateway-api.yml
consequence_counts:
  physical: 5
  read: 38
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oracle E Business Suite Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ar/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /oe/salesOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /po/purchaseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /po/purchaseOrders/{poHeaderId}
operation_count: 53
overview: 'Oracle E-Business Suite exposes 53 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 10 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
slug: oracle-e-business-suite-agentic-access
source_filename: oracle-e-business-suite-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ecommerce-gateway-api.yml, openapi/financial-services-api.yml, openapi/human-resources-api.yml,\n  openapi/isg-rest-api.yml, openapi/manufacturing-api.yml, openapi/supply-chain-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 38\n    acting: 15\n  by_consequence:\n    read: 38\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /ece/tradingPartners\n  method: get\n  operationId: getTradingPartners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ece/tradingPartners/{tradingPartnerId}\n  method: get\n\
  \  operationId: getTradingPartnerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ece/transactions/inbound\n  method: get\n  operationId: getInboundTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ece/transactions/inbound\n  method: post\n  operationId: importInboundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ece/transactions/outbound\n  method: get\n  operationId: getOutboundTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ece/transactions/outbound\n  method: post\n  operationId: extractOutboundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ece/codeConversions\n  method: get\n  operationId: getCodeConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gl/journals\n  method: get\n  operationId: getJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gl/journals\n  method: post\n  operationId: createJournal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap/invoices\n  method: get\n  operationId: getApInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap/invoices\n  method: post\n  operationId: createApInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap/invoices/{invoiceId}\n  method: get\n  operationId: getApInvoiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ap/payments\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar/invoices\n  method: get\n  operationId: getArInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar/invoices\n  method: post\n  operationId: createArInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ar/receipts\n  method: get\n  operationId: getReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fa/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ce/bankAccounts\n  method: get\n  operationId: getBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hr/employees\n  method: get\n  operationId: getEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hr/employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /hr/employees/{personId}\n  method: get\n  operationId: getEmployeeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hr/employees/{personId}\n  method: put\n  operationId: updateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hr/assignments\n  method: get\n  operationId: getAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hr/organizations\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hr/positions\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/payrolls\n  method: get\n  operationId: getPayrolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/payrollRuns\n  method: get\n  operationId: getPayrollRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ben/benefits\n  method: get\n  operationId: getBenefitEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: get\n  operationId: login\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /initialize\n  method: post\n  operationId: initialize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{serviceAlias}\n  method: get\n  operationId: getServiceWADL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{serviceAlias}/{methodName}\n  method: post\n  operationId: invokeRestMethod\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bom/billsOfMaterial\n  method: get\n  operationId: getBillsOfMaterial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bom/billsOfMaterial/{billSequenceId}\n  method: get\n  operationId: getBillOfMaterialById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bom/routings\n  method: get\n  operationId: getRoutings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wip/discreteJobs\n  method: get\n  operationId: getDiscreteJobs\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wip/discreteJobs\n  method: post\n  operationId: createDiscreteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wip/discreteJobs/{wipEntityId}\n  method: get\n  operationId: getDiscreteJobById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wip/operations\n  method: get\n  operationId: getWipOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wip/completions\n  method: post\n \
  \ operationId: completeAssembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wip/materialTransactions\n  method: post\n  operationId: issueMaterial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /po/purchaseOrders\n  method: get\n  operationId: getPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /po/purchaseOrders\n  method: post\n  operationId: createPurchaseOrder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /po/purchaseOrders/{poHeaderId}\n  method: get\n  operationId: getPurchaseOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /po/purchaseOrders/{poHeaderId}\n  method: put\n  operationId: updatePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /po/requisitions\n  method: get\n\
  \  operationId: getRequisitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /po/suppliers\n  method: get\n  operationId: getSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oe/salesOrders\n  method: get\n  operationId: getSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oe/salesOrders\n  method: post\n  operationId: createSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /inv/items\n  method: get\n  operationId: getInventoryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inv/onhandQuantities\n  method: get\n  operationId: getOnhandQuantities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wsh/deliveries\n  method: get\n  operationId: getDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/agentic-access/oracle-e-business-suite-agentic-access.yml
summary_line: 53 operations · 15 acting
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
---
