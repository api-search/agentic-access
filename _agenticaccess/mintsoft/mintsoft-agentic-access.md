---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 118
api_specs:
- filename: mintsoft-accounting-api-openapi.yml
  format: yaml
  label: Mintsoft Accounting API
  slug: mintsoft-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-accounting-api-openapi.yml
- filename: mintsoft-asn-api-openapi.yml
  format: yaml
  label: Mintsoft ASN API
  slug: mintsoft-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-asn-api-openapi.yml
- filename: mintsoft-auth-api-openapi.yml
  format: yaml
  label: Mintsoft Auth API
  slug: mintsoft-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-auth-api-openapi.yml
- filename: mintsoft-batch-api-openapi.yml
  format: yaml
  label: Mintsoft Batch API
  slug: mintsoft-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-batch-api-openapi.yml
- filename: mintsoft-client-api-openapi.yml
  format: yaml
  label: Mintsoft Client API
  slug: mintsoft-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-client-api-openapi.yml
- filename: mintsoft-courier-api-openapi.yml
  format: yaml
  label: Mintsoft Courier API
  slug: mintsoft-courier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-courier-api-openapi.yml
- filename: mintsoft-order-api-openapi.yml
  format: yaml
  label: Mintsoft Order API
  slug: mintsoft-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-order-api-openapi.yml
- filename: mintsoft-orderrules-api-openapi.yml
  format: yaml
  label: Mintsoft Order Rules API
  slug: mintsoft-orderrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-orderrules-api-openapi.yml
- filename: mintsoft-product-api-openapi.yml
  format: yaml
  label: Mintsoft Product API
  slug: mintsoft-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-product-api-openapi.yml
- filename: mintsoft-refdata-api-openapi.yml
  format: yaml
  label: Mintsoft Ref Data API
  slug: mintsoft-refdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-refdata-api-openapi.yml
- filename: mintsoft-replenpoint-api-openapi.yml
  format: yaml
  label: Mintsoft Replen Point API
  slug: mintsoft-replenpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-replenpoint-api-openapi.yml
- filename: mintsoft-reports-api-openapi.yml
  format: yaml
  label: Mintsoft Reports API
  slug: mintsoft-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-reports-api-openapi.yml
- filename: mintsoft-return-api-openapi.yml
  format: yaml
  label: Mintsoft Return API
  slug: mintsoft-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-return-api-openapi.yml
- filename: mintsoft-warehouse-api-openapi.yml
  format: yaml
  label: Mintsoft Warehouse API
  slug: mintsoft-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/openapi/mintsoft-warehouse-api-openapi.yml
consequence_counts:
  physical: 34
  read: 118
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mintsoft Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/ASN
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Account/Invoice/AddAdditionalInvoiceItem
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Accounting/AddCourierCost
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Batch/AssignOrderToUser
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/Comments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order/{id}/ConnectActions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order/{id}/Documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order/{id}/Items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/Items/{ItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/Order/{id}/Items/{ItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/MarkFraudRisk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/MarkFraudRiskAccepted
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order/{id}/Shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/Order/{id}/Shipments/CancelShipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/Shipments/CreateShipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/Order/{id}/Shipments/{OrderShipmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Order/{id}/SplitOrderItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/Order/{id}/Tag
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/Order/{id}/Tag
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/OrderRules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderRules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/OrderRules/Conditions/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderRules/Run/{orderId}
operation_count: 187
overview: 'Mintsoft exposes 187 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 118 read, 35 write, and 34 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mintsoft
provider_slug: mintsoft
slug: mintsoft-agentic-access
source_filename: mintsoft-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/mintsoft-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 187\n  by_action_class:\n    connected: 118\n    acting: 69\n  by_consequence:\n    read: 118\n    physical: 34\n    write: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /api/Accounting/Invoice/List\n  method: get\n  operationId: Accounting_ListInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/All\n  method: get\n  operationId: Accounting_GetInvoicesAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/{id}\n  method: get\n  operationId: Accounting_GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/{id}/Orders\n  method: get\n  operationId: Accounting_GetInvoiceOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/Orders/{OrderId}\n  method: get\n  operationId: Accounting_GetInvoiceItemForOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/AddCourierCost\n  method: post\n  operationId: Accounting_AddCourierCost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Accounting/Invoice/{id}/Returns\n  method: get\n  operationId: Accounting_GetInvoiceReturns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/{id}/GoodsIn\n  method: get\n  operationId: Accounting_GetInvoiceGoodsIn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/{id}/Collections\n  method: get\n  operationId: Accounting_GetInvoiceCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Accounting/Invoice/{id}/Other\n\
  \  method: get\n  operationId: Accounting_GetInvoiceGenerics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/Invoice/InvoiceItemTypes\n  method: get\n  operationId: Accounting_GetInvoiceItemTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/Invoice/AddAdditionalInvoiceItem\n  method: post\n  operationId: Accounting_AddAdditionalInvoiceItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Accounting/LocationTypeStoragePrice\n  method: post\n  operationId: Accounting_AddLocationTypeStoragePrice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/Invoice/GetUnconfirmedInvoiceSummary\n  method: get\n  operationId: Accounting_GetUnconfirmedInvoiceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/Invoice/GetUnconfirmedInvoiceStorageCosts\n  method: get\n  operationId: Accounting_GetUnconfirmedInvoiceStorageCosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN\n  method: put\n  operationId: ASN_CreateASN\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ASN/{id}\n  method: get\n  operationId: ASN_GetASN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}\n  method: post\n  operationId: ASN_UpdateASN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ASN/{id}\n  method: delete\n  operationId: ASN_DeleteASN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ASN/List\n  method: get\n  operationId: ASN_ListASNs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/ConnectActions\n  method: put\n  operationId: ASN_UploadConnectAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ASN/Statuses\n  method: get\n  operationId: ASN_GetStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/GoodsInTypes\n  method: get\n  operationId:\
  \ ASN_GetGoodsInTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/Confirm\n  method: get\n  operationId: ASN_ConfirmASN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/BookIn\n  method: get\n  operationId: ASN_BookInASN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/BookInPartial\n  method: get\n  operationId: ASN_BookInASNPartial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/PartBook\n  method: get\n  operationId: ASN_PartBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/Paperwork\n  method: get\n  operationId: ASN_GetPaperwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/Items/Receive\n  method: post\n  operationId: ASN_ReceiveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ASN/{id}/MarkAwaitingPutAway\n  method: get\n  operationId: ASN_MarkAwaitingPutAway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ASN/{id}/MarkPutAwayComplete\n  method: get\n  operationId: ASN_MarkPutAwayComplete\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Auth\n  method: post\n  operationId: Auth_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch\n  method: post\n  operationId: Batch_CreateBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/AssignOrderToUser\n  method: post\n  operationId: Batch_AssignOrderToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/AssignBatchToUser\n  method: post\n  operationId: Batch_AssignBatchToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/List\n  method: get\n  operationId: Batch_ListBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Batch/{id}\n  method: get\n  operationId: Batch_GetBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Batch/StatusUpdate/{id}\n  method: put\n  operationId: Batch_UpdateBatchStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/DespatchBatch\n  method: post\n  operationId: Batch_DespatchBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/Templates\n  method: get\n  operationId: Batch_Templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/Batch/CreateBatchFromTemplate\n  method: post\n  operationId: Batch_CreateBatchFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Batch/DeleteBatch\n  method: delete\n  operationId: Batch_DeleteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Client\n  method: get\n  operationId: Client_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Client\n  method:\
  \ post\n  operationId: Client_CreateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Client/UpdateClient\n  method: post\n  operationId: Client_UpdateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Client/SubClients\n  method: get\n  operationId: Client_SubClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Client/SubClients\n  method: post\n  operationId: Client_AddSubClient\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Courier/Services\n  method: get\n  operationId: Courier_GetCourierServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Courier/Services/{id}\n  method: get\n  operationId: Courier_GetCourierService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Courier/ServiceTypes\n  method: get\n  operationId: Courier_GetCourierServiceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Courier/Services/{id}/ExternalNames\n\
  \  method: get\n  operationId: Courier_GetExternalCourierServiceNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Statuses\n  method: get\n  operationId: Order_GetOrderStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Documents/DocumentTypes\n  method: get\n  operationId: Order_GetOrderDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Documents/PaperSizes\n  method: get\n  operationId: Order_GetOrderDocumentPaperSizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Shipments/TrackingEvents/Statuses\n\
  \  method: get\n  operationId: Order_GetOrderShipmentTrackingEventsStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Shipments/TrackingEvents/List\n  method: get\n  operationId: Order_ListTrackingEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order\n  method: put\n  operationId: Order_CreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}\n  method: get\n  operationId: Order_Get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}\n  method: post\n  operationId: Order_UpdateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/Search\n  method: get\n  operationId: Order_SearchOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/GetOrderId\n  method: get\n  operationId: Order_GetOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/TrackingNumberSearch\n  method: get\n  operationId:\
  \ Order_TrackingNumberSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/Channels\n  method: get\n  operationId: Order_GetChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/List\n  method: get\n  operationId: Order_ListOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Items\n  method: get\n  operationId: Order_Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Items\n  method: put\n  operationId: Order_AddOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Items/{ItemId}\n  method: post\n  operationId: Order_UpdateOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Items/{ItemId}\n  method: delete\n  operationId: Order_DeleteOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Cancel\n  method: get\n  operationId: Order_CancelOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/CancelNoStock\n  method: get\n  operationId: Order_CancelOrderNoStock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkDespatched\n  method: get\n  operationId: Order_MarkDespatched\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkPrinted\n  method: get\n  operationId: Order_MarkPrinted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/Order/{id}/UpdateNumberOfParcels\n  method: get\n  operationId: Order_UpdateNumberOfParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkAwaitingPayment\n  method: get\n  operationId: Order_MarkAwaitingPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkPaymentReceived\n  method: get\n  operationId: Order_MarkPaymentReceived\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkAwaitingConfirmation\n  method: get\n  operationId: Order_MarkAwaitingConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/Order/{id}/MarkConfirmed\n  method: get\n  operationId: Order_MarkConfirmed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkPackAndHold\n  method: get\n  operationId: Order_MarkPackAndHold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkReleasePackAndHold\n  method: get\n  operationId: Order_MarkReleasePackAndHold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/DespatchNote\n  method: get\n  operationId: Order_DespatchNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Comments\n\
  \  method: get\n  operationId: Order_Comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Comments\n  method: post\n  operationId: Order_AddOrderComment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Splits\n  method: get\n  operationId: Order_OrderSplit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Documents\n  method: get\n  operationId: Order_Documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Documents\n  method: put\n  operationId: Order_UploadOrderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Documents/{DocumentId}/Data\n  method: get\n  operationId: Order_GetDocumentData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Documents/{DocumentId}\n  method: get\n  operationId: Order_GetDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/BoxPackingList\n\
  \  method: get\n  operationId: Order_GetBoxPackingList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Documents/{DocumentId}/MarkPrinted\n  method: get\n  operationId: Order_MarkDocumentAsPrinted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Tag\n  method: put\n  operationId: Order_AddOrderTag\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Tag\n  method: delete\n  operationId: Order_DeleteOrderTag\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Shipments\n  method: get\n  operationId: Order_GetOrderShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Shipments\n  method: put\n  operationId: Order_UploadOrderShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Shipments/{OrderShipmentId}\n\
  \  method: delete\n  operationId: Order_DeleteOrderShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Shipments/CreateShipment\n  method: post\n  operationId: Order_CreateShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Shipments/CancelShipment\n  method: delete\n  operationId: Order_CancelShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/ConnectActions\n  method: get\n  operationId: Order_GetConnectAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/ConnectActions\n  method: put\n  operationId: Order_UploadConnectAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/Allocations\n  method: get\n  operationId: Order_Allocations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/BarcodeVerifiedOrderItems\n  method: get\n  operationId: Order_BarcodeVerifiedOrderItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Queries\n  method: get\n  operationId: Order_Queries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/Queries/{QueryId}/Comments\n  method: get\n  operationId: Order_QueryComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/SplitOrderItems\n  method: post\n  operationId: Order_SplitOrderItems\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/BillingAddress\n  method: get\n  operationId: Order_BillingAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Order/{id}/MarkFraudRisk\n  method: post\n  operationId: Order_MarkFraudRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Order/{id}/MarkFraudRiskAccepted\n\
  \  method: post\n  operationId: Order_MarkFraudRiskAccepted\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderRules\n  method: get\n  operationId: OrderRules_GetOrderRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OrderRules\n  method: put\n  operationId: OrderRules_UpdateOrderRule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/OrderRules\n  method: post\n  operationId: OrderRules_AddOrderRule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderRules/{id}\n  method: delete\n  operationId: OrderRules_DeleteOrderRule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderRules/{id}/Activate\n  method: post\n  operationId: OrderRules_MarkOrderRuleActive\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderRules/{id}/Deactivate\n  method: post\n  operationId: OrderRules_MarkOrderRuleInactive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (52 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/agentic-access/mintsoft-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mintsoft/refs/heads/main/agentic-access/mintsoft-agentic-access.yml
summary_line: 187 operations · 69 acting
tags:
- warehouse-management
- logistics
- ecommerce
- fulfillment
- software
---
