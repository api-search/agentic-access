---
acting_count: 112
action_class_counts:
  acting: 112
  connected: 143
api_specs:
- filename: payabli-api-reference-openapi.json
  format: json
  label: Payabli API
  slug: payabli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/openapi/payabli-api-reference-openapi.json
consequence_counts:
  physical: 40
  read: 143
  safety-critical: 2
  write: 70
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Payabli Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /User/authreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /User/mfa/{userId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Bill/approval/{idBill}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ChargeBacks/response/{Id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Funding/depositFunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /Invoice/attachedFileFromInvoice/{idInvoice}/{filename}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoice/{entry}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoice/{idInvoice}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /Invoice/{idInvoice}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MoneyIn/refund/{transId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MoneyOut/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /MoneyOut/cancel/{referenceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MoneyOut/cancelAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MoneyOut/captureAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MoneyOut/reissue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /MoneyOut/status/{transId}/{checkPaymentStatus}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PaymentLink/bill/lotNumber/{lotNumber}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PaymentLink/bill/{billId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /PaymentLink/out/{paylinkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PaymentLink/push/{payLinkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PaymentLink/update/{payLinkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /PaymentLink/updateOut/{paylinkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PaymentLink/{idInvoice}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /PaymentLink/{payLinkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PaymentMethodDomain
operation_count: 255
overview: 'Payabli exposes 255 API operations that an AI agent could call, of which 112 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 143 read, 70 write, 40 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Payabli
provider_slug: payabli
slug: payabli-agentic-access
source_filename: payabli-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/payabli-api-reference-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 255\n  by_action_class:\n    acting: 112\n    connected: 143\n  by_consequence:\n    write: 70\n    physical: 40\n    read: 143\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/Token/serverside\n  method: post\n  operationId: createServerSideToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/MoneyIn/getpaid\n  method: post\n  operationId:\
  \ getpaidv2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/MoneyIn/authorize\n  method: post\n  operationId: authorizev2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/MoneyIn/capture/{transId}\n  method: post\n  operationId: capturev2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/MoneyIn/void/{transId}\n  method: post\n  operationId: voidv2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/MoneyIn/refund/{transId}\n  method: post\n  operationId: refundv2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/MoneyIn/refund/{transId}/{amount}\n  method: post\n  operationId: refundv2amount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/getpaid\n  method: post\n  operationId: getpaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/authorize\n  method: post\n  operationId: Authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/capture/{transId}\n  method: post\n  operationId: CaptureAuth\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/capture/{transId}/{amount}\n  method: get\n  operationId: Capture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/void/{transId}\n  method: get\n  operationId: Void\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/refund/{transId}/{amount}\n  method: get\n  operationId: Refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/refund/{transId}\n  method: post\n  operationId: RefundWithInstructions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/reverse/{transId}/{amount}\n  method: get\n  operationId: Reverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/sendreceipt/{transId}\n  method: get\n  operationId: SendReceipt2Trans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/details/{transId}\n  method: get\n  operationId: Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /MoneyIn/makecredit\n  method: post\n  operationId: Credit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyIn/reverseCredit/{transId}\n  method: get\n  operationId: ReverseCredit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyIn/validate\n  method: post\n  operationId: Validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CheckCapture/CheckProcessing\n  method: post\n  operationId: CheckProcessing\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Query/transactions/{entry}\n  method: get\n  operationId: ListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/transactions/org/{orgId}\n  method: get\n  operationId: ListTransactionsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/settlements/{entry}\n  method: get\n  operationId: ListSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/settlements/org/{orgId}\n\
  \  method: get\n  operationId: ListSettlementsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/batches/{entry}\n  method: get\n  operationId: ListBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/batches/org/{orgId}\n  method: get\n  operationId: ListBatchesOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/batchDetails/{entry}\n  method: get\n  operationId: ListBatchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/batchDetails/org/{orgId}\n  method: get\n  operationId: ListBatchDetailsOrg\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/transfers/{entry}\n  method: get\n  operationId: ListTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/transfers/org/{orgId}\n  method: get\n  operationId: ListTransfersOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/transferDetails/{entry}/{transferId}\n  method: get\n  operationId: ListTransferDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/batches/{format}/{entry}\n  method: get\n  operationId: ExportBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/batches/{format}/org/{orgId}\n  method: get\n  operationId: ExportBatchesOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/batchDetails/{format}/{entry}\n  method: get\n  operationId: ExportBatchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/batchDetails/{format}/org/{orgId}\n  method: get\n  operationId: ExportBatchDetailsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/settlements/{format}/{entry}\n  method: get\n  operationId: ExportSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /Export/settlements/{format}/org/{orgId}\n  method: get\n  operationId: ExportSettlementsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/transactions/{format}/{entry}\n  method: get\n  operationId: ExportTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/transactions/{format}/org/{orgId}\n  method: get\n  operationId: ExportTransactionsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/transfers/{entry}\n  method: get\n  operationId: ExportTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /Export/transferDetails/{format}/{entry}/{transferId}\n  method: get\n  operationId: ExportTransferDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscription/add\n  method: post\n  operationId: NewSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subscription/{subId}\n  method: get\n  operationId: GetSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscription/{subId}\n  method: put\n  operationId: UpdateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subscription/{subId}\n  method: delete\n  operationId: RemoveSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Query/subscriptions/{entry}\n  method: get\n  operationId: ListSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/subscriptions/org/{orgId}\n  method: get\n  operationId: ListSubscriptionsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /Export/subscriptions/{format}/{entry}\n  method: get\n  operationId: ExportSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/subscriptions/{format}/org/{orgId}\n  method: get\n  operationId: ExportSubscriptionsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Statistic/subscriptions/{interval}/{level}/{entryId}\n  method: get\n  operationId: SubStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customer/single/{entry}\n  method: post\n  operationId: AddCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Customer/{customerId}\n  method: get\n  operationId: GetCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customer/{customerId}\n  method: put\n  operationId: UpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Customer/{customerId}\n  method: delete\n  operationId: DeleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /Customer/link/{customerId}/{transId}\n  method: get\n  operationId: LinkCustomerTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customer/{customerId}/consent\n  method: post\n  operationId: RequestConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Import/customersForm/{entry}\n  method: post\n  operationId: ImportCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /Query/customers/{entry}\n  method: get\n  operationId: ListCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/customers/org/{orgId}\n  method: get\n  operationId: ListCustomersOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/customers/{format}/{entry}\n  method: get\n  operationId: ExportCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/customers/{format}/org/{orgId}\n  method: get\n  operationId: ExportCustomersOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Statistic/customerbasic/{mode}/{freq}/{customerId}\n\
  \  method: get\n  operationId: CustomerBasicStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Cloud/register/{entry}\n  method: post\n  operationId: addDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Cloud/list/{entry}\n  method: get\n  operationId: ListDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Cloud/history/{entry}/{deviceId}\n  method: get\n  operationId: HistoryDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /Cloud/register/{entry}/{deviceId}\n  method: delete\n  operationId: RemoveDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Query/devices/{entry}\n  method: get\n  operationId: ListDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/devices/org/{orgId}\n  method: get\n  operationId: ListDevicesOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/{entry}\n  method: post\n  operationId: AddInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoice/{idInvoice}\n  method: get\n  operationId: GetInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/{idInvoice}\n  method: put\n  operationId: EditInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoice/{idInvoice}\n  method: delete\n  operationId: DeleteInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoice/send/{idInvoice}\n  method: get\n  operationId: SendInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/attachedFileFromInvoice/{idInvoice}/{filename}\n  method: get\n  operationId: GetAttachedFileFromInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/attachedFileFromInvoice/{idInvoice}/{filename}\n  method: delete\n  operationId: deleteAttachedFromInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoice/getNumber/{entry}\n  method: get\n  operationId: GetInvoiceNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/invoices/{entry}\n  method: get\n  operationId: ListInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/invoices/org/{orgId}\n  method: get\n  operationId: ListInvoicesOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/invoices/{format}/{entry}\n  method: get\n  operationId: ExportInvoices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/invoices/{format}/org/{orgId}\n  method: get\n  operationId: ExportInvoicesOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/invoicePdf/{idInvoice}\n  method: get\n  operationId: GetInvoicePDF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Paypoint/{entry}\n  method: post\n  operationId: newPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Paypoint/{entry}\n\
  \  method: get\n  operationId: getEntryConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Paypoint/{entry}/{subdomain}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Paypoint/{entry}/{subdomain}\n  method: put\n  operationId: savePage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Paypoint/{entry}/{subdomain}\n  method: delete\n  operationId: removePage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Paypoint/load/{entry}/{subdomain}\n  method: get\n  operationId: loadPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ChargeBacks/read/{Id}\n  method: get\n  operationId: GetChargeback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ChargeBacks/response/{Id}\n  method: post\n  operationId: AddResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ChargeBacks/getChargebackAttachments/{Id}/{fileName}\n  method: get\n  operationId: getChargebackAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/chargebacks/{entry}\n  method: get\n  operationId: ListChargebacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Query/chargebacks/org/{orgId}\n  method: get\n  operationId: ListChargebacksOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/chargebacks/{format}/{entry}\n  method: get\n  operationId: ExportChargebacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Export/chargebacks/{format}/org/{orgId}\n  method: get\n  operationId: ExportChargebacksOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wallet/applepay/configure-organization\n  method: post\n  operationId: ConfigureApplePayOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wallet/applepay/configure-paypoint\n  method: post\n  operationId: ConfigureApplePayPaypoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wallet/googlepay/configure-organization\n  method: post\n  operationId: ConfigureGooglePayOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wallet/googlepay/configure-paypoint\n  method: post\n  operationId: ConfigureGooglePayPaypoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain\n  method: post\n  operationId: AddPaymentMethodDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain/{domainId}/cascade\n  method: post\n  operationId: CascadePaymentMethodDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain/{domainId}/verify\n  method: post\n  operationId: VerifyPaymentMethodDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain/{domainId}\n  method: get\n  operationId: GetPaymentMethodDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PaymentMethodDomain/{domainId}\n  method: patch\n  operationId: UpdatePaymentMethodDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain/{domainId}\n  method: delete\n  operationId: DeletePaymentMethodDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PaymentMethodDomain/list\n  method: get\n  operationId: ListPaymentMethodDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyOut/authorize\n  method: post\n  operationId: AuthorizeOut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyOut/capture/{referenceId}\n  method: get\n  operationId: CaptureOut\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyOut/captureAll\n  method: post\n  operationId: CaptureAllOut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyOut/cancel/{referenceId}\n  method: delete\n  operationId: CancelOutDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyOut/cancel/{referenceId}\n  method: get\n  operationId:\
  \ CancelOutGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyOut/cancelAll\n  method: post\n  operationId: CancelAllOut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MoneyOut/details/{transId}\n  method: get\n  operationId: PayoutDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MoneyOut/checkimage/{assetName}\n  method: get\n  operationId: GetCheckImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /MoneyOut/status/{transId}/{checkPaymentStatus}\n  method: patch\n  o\n\n# --- truncated at 32 KB (71 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/agentic-access/payabli-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/agentic-access/payabli-agentic-access.yml
summary_line: 255 operations · 112 acting · 2 human-in-the-loop
tags:
- Company
- Payments
- Embedded Payments
- Fintech
- Payment Processing
- Payments API
- Payouts
- Billing
- ACH
- Cards
- Tokenization
- Webhooks
---
