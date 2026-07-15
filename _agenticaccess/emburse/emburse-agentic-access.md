---
acting_count: 118
action_class_counts:
  acting: 118
  connected: 95
api_specs:
- filename: emburse-virtual-cards-openapi.yml
  format: yaml
  label: Emburse Virtual Cards API
  slug: emburse-virtual-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-virtual-cards-openapi.yml
- filename: emburse-enterprise-allocation-openapi.yml
  format: yaml
  label: Emburse Enterprise REST APIs
  slug: emburse-enterprise-rest-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-enterprise-allocation-openapi.yml
consequence_counts:
  physical: 3
  read: 95
  safety-critical: 77
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 77
kind: agentic-access
layout: agentic-access
method: generated
name: Emburse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/token/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /po-api
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /po-api/create-or-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /po-api/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /po-api/item/catalog/create-or-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /po-api/poNumber/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /po-api/receipts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /po-api/receipts/create-or-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /po-api/receipts/{receiptNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /po-api/receipts/{receiptNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /po-api/requestNumber/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /po-api/{poNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /po-api/{requestNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/allocations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/allocations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/allocations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-report-approvals/{reportId}/submit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/reassign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/return
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/expense-reports/{reportId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports/{reportId}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/expense-reports/{reportId}/line-items
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/expense-reports/{reportId}/notes
operation_count: 213
overview: 'Emburse exposes 213 API operations that an AI agent could call, of which 118 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 95 read, 38 write, 3 physical, and 77 safety-critical.


  77 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Emburse
provider_slug: emburse
slug: emburse-agentic-access
source_filename: emburse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/emburse-enterprise-allocation-openapi.yml, openapi/emburse-enterprise-contacts-openapi.yml,\n  openapi/emburse-enterprise-entity-openapi.yml, openapi/emburse-enterprise-expense-image-openapi.yml,\n  openapi/emburse-enterprise-expense-openapi.yml, openapi/emburse-enterprise-exported-reports-openapi.yml,\n  openapi/emburse-enterprise-invoice-openapi.yml, openapi/emburse-enterprise-paid-expense-openapi.yml,\n  openapi/emburse-enterprise-person-openapi.yml, openapi/emburse-enterprise-preapproval-openapi.yml,\n  openapi/emburse-enterprise-purchase-order-openapi.yml, openapi/emburse-enterprise-vendor-openapi.yml,\n  openapi/emburse-virtual-cards-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n\
  \  operations: 213\n  by_action_class:\n    connected: 95\n    acting: 118\n  by_consequence:\n    read: 95\n    safety-critical: 77\n    write: 38\n    physical: 3\n  human_in_the_loop_required: 77\noperations:\n- path: /v1/allocations\n  method: get\n  operationId: getAllocationUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/allocations\n  method: post\n  operationId: createAllocationV1UsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/allocations\n  method: put\n  operationId: updateAllocationV1UsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/allocations\n  method: delete\n  operationId: deleteAllocationV1UsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/allocations\n  method: get\n  operationId: getAllocationsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/allocations\n  method: post\n  operationId: bulkUpsertAllocationsUsingPOST\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/allocations\n  method: get\n  operationId: getAllocationsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/allocations\n  method: post\n  operationId: bulkUpsertAllocationsUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/allocations/entity\n  method: post\n  operationId: createMatterOnSelectUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/allocations/entity\n  method: put\n  operationId: updateMatterOnSelectUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/allocations/matterFilter\n  method: post\n  operationId: updateMatterFilterUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/allocations/search\n  method: get\n  operationId: searchAllocationsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts\n  method: post\n  operationId: createContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities\n  method: post\n  operationId: upsertEntitiesUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities\n  method: delete\n  operationId: deleteEntitiesUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types\n  method: get\n  operationId: getEntityTypesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entity-types\n  method: post\n  operationId: createEntityTypeUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types/{code}\n  method: get\n  operationId: getEntityTypeByCodeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entity-types/{code}\n  method: put\n  operationId: replaceEntityTypeByCodeUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types/{entityTypeCode}\n  method: delete\n  operationId: deleteEntityTypeByCodeUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types/{entityTypeCode}/languages\n  method: get\n  operationId: getLanguagesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entity-types/{entityTypeCode}/languages\n  method: post\n  operationId: addLanguageUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types/{entityTypeCode}/languages/{languageCode}\n  method: put\n  operationId: updateLanguageUsingPUT\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entity-types/{entityTypeCode}/languages/{languageCode}\n  method: delete\n  operationId: deleteLanguageUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/entities\n  method: get\n  operationId: getUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/entities/search\n  method: get\n  operationId: searchUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getVoucherInvoices\n  method: get\n  operationId: getByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getVoucherInvoicesForXML\n  method: get\n  operationId: getVoucherInvoicesForXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getVoucherInvoicesForOFD\n  method: get\n  operationId: getVoucherInvoicesForOFD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getReceipts\n  method: get\n  operationId: getReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getReceiptsWithCoverPage\n  method: get\n  operationId: getReceiptsWithCoverPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getReceiptsForXml\n  method: get\n  operationId: getReceiptsForXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getReceiptsForOFD\n  method: get\n  operationId: getReceiptsForOFD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getLineItemVoucherInvoices\n  method: get\n  operationId: getLineItemVoucherInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getLineItemReceipts\n  method: get\n  operationId: getLineItemReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getLineItemReceiptsWithMileageDetails\n  method: get\n  operationId: getLineItemReceiptsWithMileageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense-image-api/getLineItemReceiptsFromLineItemId\n  method: get\n  operationId: getLineItemReceiptsFromLineItemId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-receipts/{reportId}\n  method: get\n  operationId: getExpenseReceiptsUsingGET\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-report-approvals\n  method: get\n  operationId: getApprovalsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-report-approvals/count\n  method: get\n  operationId: getExpenseReportCountUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-report-approvals/{reportId}\n  method: get\n  operationId: getExpenseReportUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-report-approvals/{reportId}/submit\n  method: post\n  operationId: submitExpenseReportForApprovalUsingPOST\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-report-line-item-search\n  method: get\n  operationId: getLineItemsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-reports\n  method: get\n  operationId: getExpenseReportsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-reports\n  method: post\n  operationId: createExpenseReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/approve\n  method: post\n  operationId: approveExpenseReportLineItemUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/reassign\n  method: post\n  operationId: reassignExpenseReportLineItemUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{report-id}/line-items/{report-line-item-id}/return\n  method: post\n  operationId: returnExpenseReportLineItemUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}\n  method: get\n  operationId: getExpenseReportUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense-reports/{reportId}\n  method: delete\n  operationId: deleteExpenseReportUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/approve\n  method: post\n  operationId: approveExpenseReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/line-items\n  method: delete\n  operationId: deleteExpenseReportLineItemUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/notes\n  method: post\n  operationId: createExpenseHeaderNoteUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/reassign\n  method: post\n  operationId: reassignExpenseReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/return\n  method: post\n  operationId:\
  \ returnExpenseReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/submit\n  method: post\n  operationId: submitExpenseReportUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/expense-reports/{reportId}/tracking\n  method: get\n  operationId: getReportForTrackingUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/expense-types\n  method: get\n  operationId: getExpenseTypesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-expense-reports\n  method: get\n  operationId: getOpenExpenseReportsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/returned-payment-expense-reports/lite\n  method: get\n  operationId: getReturnedPaymentExpenseReportHeaderIdsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trip-reports-summary\n  method: get\n  operationId: getTripReportsSummaryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/expense-report-approvals\n  method: get\n  operationId: getApprovalsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/expense-report-approvals/count\n  method: get\n  operationId: getExpenseReportCountUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/expense-report-approvals/{reportId}\n  method: get\n  operationId: getExpenseReportUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/expense-reports/{reportId}/approve\n  method: post\n  operationId: approveExpenseReportUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/expense-reports/{reportId}/reassign\n  method: post\n  operationId: reassignExpenseReportUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/expense-reports/{reportId}/return\n  method: post\n  operationId: returnExpenseReportUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v2/expense-reports/{reportId}/submit\n  method: post\n  operationId: submitExpenseReportUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/expense-reports\n  method: get\n  operationId: getExpenseReportsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/expense-reports/{reportId}\n  method: get\n  operationId: getExpenseReportUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/expense-reports/{reportId}/line-items\n  method: get\n\
  \  operationId: getLineItemsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/export-status\n  method: post\n  operationId: updateExpenseExportStatusUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/export-status/re-post\n  method: patch\n  operationId: repostExternalExportStatusByExportIdsUsingPATCH\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/exports\n  method: get\n  operationId: getExportIdsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/export-status\n  method: post\n  operationId: updateExportStatusUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/export-status/re-post\n  method: patch\n  operationId: repostExternalExportStatusByExportIdsUsingPATCH_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/exports\n  method: get\n  operationId: getExportIdsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice-api/invoices\n  method: put\n  operationId: getInvoicesUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/images/pdf\n  method: get\n  operationId: getImagesInPdfUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice-api/invoices/payments\n  method: put\n  operationId:\
  \ getInvoicePaymentsUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/sdi/xml\n  method: post\n  operationId: postInvoicePaymentStatusUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/{invoiceId}/approve\n  method: post\n  operationId: approveInvoiceUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/{invoiceId}/assign\n  method: post\n  operationId: assignInvoiceUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/{invoiceId}/ocr/images\n  method: get\n  operationId: getInvoiceOcrImagesReportUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice-api/invoices/{invoiceId}/payment\n  method: post\n  operationId: postInvoicePaymentStatusExternalUsingPOST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoice-api/invoices/{invoiceId}/return\n  method: post\n  operationId: returnInvoiceUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/paid-expense\n  method: post\n  operationId: createPaidExpenseUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/paid-expenses\n  method: post\n  operationId: createPaidExpensesUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons/{personUniqueId}/person-entities/{person-entity-id}\n  method: get\n  operationId: getPersonEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/persons/{personUniqueId}/person-entities/{person-entity-id}\n  method: put\n  operationId: modifyPersonEntityById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons/{personUniqueId}/person-entities/{person-entity-id}\n  method: delete\n  operationId: deletePersonEntityById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/sap-persons\n  method: post\n  operationId: sapPatchyPostBecauseReasons\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons\n  method: get\n  operationId: getPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/persons\n  method: post\n  operationId: createPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons/{toPersonUniqueId}/assists/{fromPersonUniqueId}\n  method: post\n  operationId: addPersonDelegate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons/{toPersonUniqueId}/assists/{fromPersonUniqueId}\n  method: delete\n  operationId: deletePersonDelegate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v4/persons/{personUniqueId}/udas\n  method: get\n  operationId: getPersonUdas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/persons/{personUniqueId}/udas\n  method: post\n  operationId: createPersonUda\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-requir\n\n# --- truncated at 32 KB (66 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/agentic-access/emburse-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/agentic-access/emburse-agentic-access.yml
summary_line: 213 operations · 118 acting · 77 human-in-the-loop
tags:
- Expense Management
- AP Automation
- Corporate Cards
- Virtual Cards
- Receipt Capture
- Reimbursement
- Invoice Processing
- Finance
- FinTech
---
