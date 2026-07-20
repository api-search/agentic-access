---
acting_count: 340
action_class_counts:
  acting: 340
  connected: 114
api_specs:
- filename: fulcrumpro-openapi-original.json
  format: json
  label: Fulcrum Public API
  slug: fulcrum-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/openapi/fulcrumpro-openapi-original.json
consequence_counts:
  physical: 118
  read: 114
  safety-critical: 5
  write: 217
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Fulcrumpro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/inventory/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/job-tracking-timers/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/operations/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/reporting/time-clock/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/timers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/deposit-adjustment-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/deposit-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/fee-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/invoices/{invoiceId}/fee-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/invoices/{invoiceId}/fee-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/notes/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/part-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/invoices/{invoiceId}/part-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/invoices/{invoiceId}/part-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/refund-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/invoices/{invoiceId}/refund-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/invoices/{invoiceId}/refund-line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices/{invoiceId}/tax-line-items/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/items/{itemId}/purchase-price-breaks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/items/{itemId}/purchase-price-breaks/list
operation_count: 454
overview: 'Fulcrumpro exposes 454 API operations that an AI agent could call, of which 340 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 114 read, 217 write, 118 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fulcrumpro
provider_slug: fulcrumpro
slug: fulcrumpro-agentic-access
source_filename: fulcrumpro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/fulcrumpro-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 454\n  by_action_class:\n    acting: 340\n    connected: 114\n  by_consequence:\n    write: 217\n    read: 114\n    safety-critical: 5\n    physical: 118\n  human_in_the_loop_required: 5\noperations:\n- path: /api/accounting-codes\n  method: post\n  operationId: CreateAccountingCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounting-codes/{id}\n  method: get\n\
  \  operationId: GetAccountingCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounting-codes/list\n  method: post\n  operationId: ListAccountingCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments\n  method: post\n  operationId: CreateAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/remote\n  method: post\n  operationId: CreateRemoteAttachment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/{attachmentId}\n  method: delete\n  operationId: DeleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/{attachmentId}\n  method: get\n  operationId: GetAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attachments/{attachmentId}/download\n  method: get\n  operationId: DownloadAttachment\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attachments/download\n  method: post\n  operationId: DownloadAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/list\n  method: post\n  operationId: ListAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/certification\n  method: post\n  operationId: CreateCertificationAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/validate\n  method: get\n  operationId: GetValidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capas/{capaId}\n  method: get\n  operationId: GetCapa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capas/list\n  method: post\n  operationId: ListCAPA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chart-of-accounts/{id}\n\
  \  method: get\n  operationId: GetChartOfAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chart-of-accounts/list\n  method: post\n  operationId: ListChartOfAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/companies/{companyId}\n  method: get\n  operationId: GetCompanyInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/companies/list\n  method: post\n  operationId: ListCompanyInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/custom-fields/{id}\n  method: get\n  operationId: GetCustomField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/custom-fields/list\n  method: post\n  operationId: ListCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers\n  method: post\n  operationId: CreateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}\n  method: delete\n  operationId: DeleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}\n  method: get\n  operationId: GetCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/customers/{customerId}\n  method: patch\n  operationId: PatchCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/customers/{customerId}\n  method: put\n  operationId: UpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/list\n  method: post\n  operationId: ListCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customer-tiers/{id}\n  method: get\n  operationId: GetCustomerTier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/customer-tiers/list\n  method:\
  \ post\n  operationId: ListCustomerTier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/addresses\n  method: post\n  operationId: CreateCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/addresses/{customerAddressId}\n  method: delete\n  operationId: DeleteCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/addresses/{customerAddressId}\n  method: get\n  operationId: GetCustomerAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/customers/{customerId}/addresses/{customerAddressId}\n  method: put\n  operationId: UpdateCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/addresses/list\n  method: post\n  operationId: ListCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/contacts\n  method: post\n  operationId: CreateCustomerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/contacts/{contactId}\n  method: delete\n  operationId: DeleteCustomerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/contacts/{contactId}\n  method: get\n  operationId: GetCustomerContact\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/customers/{customerId}/contacts/{contactId}\n  method: put\n  operationId: UpdateCustomerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/customers/{customerId}/contacts/list\n  method: post\n  operationId: ListCustomerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/departments\n  method: post\n  operationId: CreateDepartment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/departments/{id}\n  method: get\n  operationId: GetDepartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/departments/{id}\n  method: put\n  operationId: UpdateDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/departments/list\n  method: post\n  operationId: ListDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/equipment\n  method: post\n  operationId: CreateEquipment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/equipment/{id}\n  method: get\n  operationId: GetEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/equipment/{id}\n  method: put\n  operationId: UpdateEquipment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/equipment/list\n  method: post\n  operationId: ListEquipment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gauge-codes/{id}\n  method: get\n  operationId: GetGaugeCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gauge-codes/list\n  method: post\n  operationId: ListGaugeCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/grade-codes/{id}\n  method: get\n  operationId: GetGradeCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/grade-codes/list\n  method: post\n  operationId: ListGradeCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/in-process-tracking-field-types/{id}\n  method: get\n  operationId: GetInProcessTrackingFieldType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/in-process-tracking-field-types\n  method: post\n  operationId: ListInProcessTrackingFieldType\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory/list\n  method: post\n  operationId: ListInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory/byItem\n  method: get\n  operationId: OnHandByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inventory/override\n  method: post\n  operationId: OverrideInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/inventory/pick\n  method: post\n  operationId: PickInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory/availableByItem\n  method: get\n  operationId: QuantityAvailableByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inventory/receive\n  method: post\n  operationId: ReceiveInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-events/{inventoryEventId}\n  method: get\n  operationId: GetInventoryEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inventory-events/list\n  method: post\n  operationId: ListInventoryEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-events/{inventoryEventId}/details\n  method: patch\n  operationId: PatchInventoryEventDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-events/{inventoryEventId}/details\n  method: put\n  operationId: UpdateInventoryEventDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-events/{inventoryEventId}/details\n  method: get\n  operationId: GetInventoryEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inventory-lots\n  method: post\n  operationId: CreateInventoryLot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-lots/{id}\n  method: get\n  operationId: GetInventoryLot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inventory-lots/list\n  method: post\n  operationId: ListInventoryLot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inventory-transactions/list\n  method: post\n  operationId: ListInventoryTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}\n  method: get\n  operationId: GetInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}\n  method: patch\n  operationId: PatchInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}\n  method: put\n  operationId: UpdateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/list\n  method: post\n  operationId: ListInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/status\n  method: post\n  operationId: StatusUpdateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/invoices/{invoiceId}/deposit-adjustment-line-items/{lineItemId}\n  method: get\n  operationId: GetDepositAdjustmentLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/deposit-adjustment-line-items/list\n  method: post\n  operationId: ListDepositAdjustmentLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/deposit-line-items/{lineItemId}\n  method: get\n  operationId: GetInvoiceDepositLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/deposit-line-items/list\n  method: post\n  operationId: ListInvoiceDepositLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/discount-line-item\n  method: get\n  operationId: GetInvoiceDiscountLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/fee-line-items/{lineItemId}\n  method: get\n  operationId: GetInvoiceFeeLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/invoices/{invoiceId}/fee-line-items/{lineItemId}\n  method: patch\n  operationId: PatchInvoiceFeeLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/fee-line-items/{lineItemId}\n  method: put\n  operationId: UpdateInvoiceFeeLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/fee-line-items/list\n  method: post\n  operationId: ListInvoiceFeeLineItem\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/line-items/{lineItemId}\n  method: get\n  operationId: GetInvoiceLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/line-items/list\n  method: post\n  operationId: ListInvoiceLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/invoices/{invoiceId}/notes/list\n  method: post\n  operationId: ListInvoiceNote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/part-line-items/{lineItemId}\n  method: get\n  operationId: GetInvoicePartLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/part-line-items/{lineItemId}\n  method: patch\n  operationId: PatchInvoicePartLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/part-line-items/{lineItemId}\n  method: put\n  operationId: UpdateInvoicePartLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/part-line-items/list\n  method: post\n  operationId: ListInvoicePartLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/refund-line-items/{lineItemId}\n  method: get\n  operationId: GetInvoiceRefundLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/refund-line-items/{lineItemId}\n  method: patch\n  operationId: PatchInvoiceRefundLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/refund-line-items/{lineItemId}\n  method: put\n  operationId: UpdateInvoiceRefundLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/refund-line-items/list\n  method: post\n  operationId: ListInvoiceRefundLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}/shipping-charge-line-item\n  method: get\n  operationId: GetInvoiceShippingChargeLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/tax-line-items/{lineItemId}\n\
  \  method: get\n  operationId: GetInvoiceTaxLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoiceId}/tax-line-items/list\n  method: post\n  operationId: ListInvoiceTaxLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{itemId}/revision\n  method: post\n  operationId: AddRevisionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/items\n  method: post\n  operationId: CreateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{itemId}\n  method: get\n  operationId: GetItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items/{itemId}\n  method: patch\n  operationId: PatchItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{itemId}\n  method: put\n  operationId: UpdateItem\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-tt\n\n# --- truncated at 32 KB (157 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/agentic-access/fulcrumpro-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/agentic-access/fulcrumpro-agentic-access.yml
summary_line: 454 operations · 340 acting · 5 human-in-the-loop
tags:
- Company
- Manufacturing
- ERP
- MES
- Manufacturing Execution
- Job Shop
- CNC Machining
- Sheet Metal
- Inventory
- Purchasing
- Quoting
- Scheduling
---
