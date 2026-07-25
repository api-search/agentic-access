---
acting_count: 86
action_class_counts:
  acting: 86
  connected: 76
api_specs:
- filename: propertyware-accounting-api-openapi.yml
  format: yaml
  label: Propertyware Accounting API
  slug: propertyware-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-accounting-api-openapi.yml
- filename: propertyware-bills-api-openapi.yml
  format: yaml
  label: Propertyware Bills API
  slug: propertyware-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-bills-api-openapi.yml
- filename: propertyware-buildings-api-openapi.yml
  format: yaml
  label: Propertyware Buildings API
  slug: propertyware-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-buildings-api-openapi.yml
- filename: propertyware-contacts-api-openapi.yml
  format: yaml
  label: Propertyware Contacts API
  slug: propertyware-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-contacts-api-openapi.yml
- filename: propertyware-custom-field-definitions-api-openapi.yml
  format: yaml
  label: Propertyware Custom field definitions API
  slug: propertyware-custom-field-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-custom-field-definitions-api-openapi.yml
- filename: propertyware-documents-api-openapi.yml
  format: yaml
  label: Propertyware Documents API
  slug: propertyware-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-documents-api-openapi.yml
- filename: propertyware-health-check-api-openapi.yml
  format: yaml
  label: Propertyware Health check API
  slug: propertyware-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-health-check-api-openapi.yml
- filename: propertyware-inspections-api-openapi.yml
  format: yaml
  label: Propertyware Inspections API
  slug: propertyware-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-inspections-api-openapi.yml
- filename: propertyware-leases-api-openapi.yml
  format: yaml
  label: Propertyware Leases API
  slug: propertyware-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-leases-api-openapi.yml
- filename: propertyware-portfolios-api-openapi.yml
  format: yaml
  label: Propertyware Portfolios API
  slug: propertyware-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-portfolios-api-openapi.yml
- filename: propertyware-prospects-api-openapi.yml
  format: yaml
  label: Propertyware Prospects API
  slug: propertyware-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-prospects-api-openapi.yml
- filename: propertyware-units-api-openapi.yml
  format: yaml
  label: Propertyware Units API
  slug: propertyware-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-units-api-openapi.yml
- filename: propertyware-vendors-api-openapi.yml
  format: yaml
  label: Propertyware Vendors API
  slug: propertyware-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-vendors-api-openapi.yml
- filename: propertyware-work-orders-api-openapi.yml
  format: yaml
  label: Propertyware Work orders API
  slug: propertyware-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/openapi/propertyware-work-orders-api-openapi.yml
consequence_counts:
  physical: 24
  read: 76
  write: 62
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Propertyware Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/bankdeposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounting/bankdeposits/{bankDepositID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/glaccounts/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bills/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /bills/payment/{billPaymentID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bills/payments/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /leases/autocharges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /leases/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /leases/charges/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /leases/charges/{chargeID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /leases/charges/{chargeID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /leases/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /leases/payments/{entityID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /leases/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /leases/refunds/{refundID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/closeworkorder/{workOrderID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/customfields
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workorders/{workOrderID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workorders/{workOrderID}/tasks/{taskID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/{workOrderId}/tasks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workOrderId}/tasks/{taskId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/{workOrderId}/tasks/{taskId}/comments
operation_count: 162
overview: 'Propertyware exposes 162 API operations that an AI agent could call, of which 86 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 76 read, 62 write, and 24 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Propertyware
provider_slug: propertyware
slug: propertyware-agentic-access
source_filename: propertyware-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/propertyware-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 162\n  by_action_class:\n    acting: 86\n    connected: 76\n  by_consequence:\n    physical: 24\n    read: 76\n    write: 62\n  human_in_the_loop_required: 0\noperations:\n- path: /accounting/bankdeposits\n  method: post\n  operationId: createBankDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/bankdeposits/{bankDepositID}\n\
  \  method: delete\n  operationId: deleteBankDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/generalledger\n  method: get\n  operationId: getGeneralLedgerTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/glaccounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/glaccounts\n  method: post\n  operationId: createGLAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/glaccounts/bulk\n  method: post\n  operationId: createBillPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/glaccounts/{glAccountID}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/glaccounts/{glAccountID}\n  method: put\n  operationId: updateGLAccount\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/glaccounts/{glAccount}\n  method: delete\n  operationId: deleteGLAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/ownercontributions\n  method: get\n  operationId: getOwnerContributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/ownercontributions\n  method: post\n  operationId: createOwnerContribution\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/ownercontributions/{ownerContributionID}\n  method: delete\n  operationId: deleteOwnerContribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/ownerdraws\n  method: get\n  operationId: getOwnerDraws\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/ownerdraws\n  method: post\n  operationId: createOwnerDraw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/ownerdraws/{drawID}\n  method: put\n  operationId: updateOwnerDraw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills\n  method: get\n  operationId: getBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills\n  method: post\n  operationId: createBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/bulk\n  method: post\n  operationId: createBills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/credit\n  method: post\n  operationId: createCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/credit/{creditID}\n  method: put\n  operationId: updateCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/payment\n  method: post\n  operationId: createBillPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/payment/{billPaymentID}\n  method: put\n  operationId: updateBillPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/payments\n  method: get\n  operationId: getBillPayments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/payments/bulk\n  method: post\n  operationId: createBillPaymentsUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/payments/{billPaymentID}\n  method: get\n  operationId: getBillPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/vendorchecks\n  method: get\n  operationId: getVendorChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /bills/vendorchecks\n  method: post\n  operationId: createVendorCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/vendorchecks/{vendorCheckID}\n  method: put\n  operationId: updateVendorCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{billID}\n  method: get\n  operationId: getBill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{billID}\n  method: delete\n\
  \  operationId: deleteBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{billId}\n  method: put\n  operationId: updateBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings\n  method: get\n  operationId: getBuildings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings\n  method: post\n  operationId: createBuilding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/bulk\n  method: post\n  operationId: createContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/customfields\n  method: put\n  operationId: updateBuilding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/{buildingID}\n  method: get\n  operationId: getBuilding\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{buildingID}\n  method: put\n  operationId: updateBuildingUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/{buildingID}\n  method: delete\n  operationId: deleteBuilding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/{buildingID}/conversations\n  method: get\n  operationId: getBuildingConversations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{buildingID}/conversations/{conversationID}\n  method: get\n  operationId: getBuildingConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{buildingID}/conversations/{conversationID}\n  method: delete\n  operationId: deleteBuildingConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/{buildingID}/managementfees\n  method: get\n  operationId: getBuildingManagementFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /buildings/{buildingID}/managers\n  method: get\n  operationId: getBuildingManagers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{buildingID}/notes\n  method: get\n  operationId: getBuildingNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /contacts/bulk\n  method: post\n  operationId: createContactsUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/categories\n  method: get\n  operationId: getContactCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/customfields\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactID}\n\
  \  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactID}\n  method: put\n  operationId: updateContactUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactID}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactID}/conversations\n  method: get\n  operationId: getContactConversations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactID}/conversations/{conversationID}\n  method: get\n  operationId: getContactConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactID}/conversations/{conversationID}\n  method: delete\n  operationId: deleteContactConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customfields/{entityType}/definitions\n  method: get\n  operationId: retrieveCustomFieldDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: retrieveAllDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docs/{documentId}\n  method: get\n  operationId: retrieveDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/{documentId}\n  method: put\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docs/{documentId}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docs/{documentId}/download\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspections\n  method:\
  \ get\n  operationId: getInspections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspections/{inspectionId}\n  method: get\n  operationId: getInspection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases\n  method: get\n  operationId: getLeases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases\n  method: post\n  operationId: createLease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/adjustments\n  method: get\n \
  \ operationId: getLeaseAdjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/adjustments\n  method: post\n  operationId: createLeaseAdjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/adjustments/{adjustmentID}\n  method: put\n  operationId: updateLeaseAdjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/autocharges\n  method: get\n  operationId: getLeaseAutoCharges\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/autocharges\n  method: post\n  operationId: createLeaseAutoCharges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/charges\n  method: get\n  operationId: getLeaseCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/charges\n  method: post\n  operationId: createLeaseCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/charges/bulk\n  method: post\n  operationId: createLeaseCharges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/charges/{chargeID}\n  method: put\n  operationId: updateLeaseCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /leases/charges/{chargeID}\n  method: delete\n  operationId: deleteLeaseCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/creditmemos\n  method: get\n  operationId: getLeaseCreditMemos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/customfields\n  method: put\n  operationId: updateLease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /leases/discounts\n  method: get\n  operationId: getLeaseDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/discounts\n  method: post\n  operationId: createLeaseDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/discounts/{discountID}\n  method: put\n  operationId: updateLeaseDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/journalentries\n  method: get\n  operationId:\
  \ getLeaseJournalEntryUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/journalentries\n  method: post\n  operationId: createJournalEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/journalentries/{journalentryID}\n  method: put\n  operationId: updateLeaseJournalEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/journalentries/{leaseID}\n  method: get\n  operationId: getLeaseJournalEntry\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/payments\n  method: get\n  operationId: getLeasePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/payments\n  method: post\n  operationId: createLeasePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/payments/{entityID}\n  method: put\n  operationId: updateLeasePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/refunds\n  method: get\n  operationId: getLeaseRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/refunds\n  method: post\n  operationId: createLeaseRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/refunds/{refundID}\n  method: put\n  operationId: updateLeaseRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/statuses\n  method: get\n  operationId: getAllLeaseStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseID}\n  method: delete\n  operationId: deleteLease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/{leaseID}/conversations\n  method: get\n  operationId: getLeaseConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseID}/conversations\n  method: post\n  operationId: createLeaseConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/{leaseID}/conversations/{conversationID}\n  method: get\n  operationId: getLeaseConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseID}/conversations/{conversationID}\n  method: delete\n  operationId: deleteLeaseConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/{leaseID}/conversations/{conversationID}/comments\n  method: post\n  operationId: addCommentToLeaseConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leases/{leaseId}\n  method: get\n  operationId: getLease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}\n  method: put\n  operationId: updateLeaseUsingPUT_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /leases/{leaseId}/autocharges\n  method: get\n  operationId: getLeaseAutoChargesUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/autoepayments\n  method: get\n  operationId: getLeaseAutoEPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/autojournalentries\n  method: get\n  operationId: getLeaseAutoJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/contacts\n  method: get\n  operationId: getLeaseContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /leases/{leaseId}/customfields\n  method: get\n  operationId: getLeaseCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/document\n  method: get\n  operationId: getLeaseDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/latefeerule\n  method: get\n  operationId: getLeaseLateFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/notes\n  method: get\n  operationId: getLeaseNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leases/{leaseId}/workorders\n  method: get\n  operationId:\
  \ getLeaseWorkOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    au\n\n# --- truncated at 32 KB (47 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/agentic-access/propertyware-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyware/refs/heads/main/agentic-access/propertyware-agentic-access.yml
summary_line: 162 operations · 86 acting
tags:
- Property Management
- Real Estate
- Rental Properties
- Single-Family Rentals
- Leases
- Tenants
- Maintenance
- Work Orders
- Financial Transactions
- Owner Reports
---
