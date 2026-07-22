---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 26
api_specs:
- filename: loop-openapi-original.json
  format: json
  label: Loop API
  slug: loop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-openapi-original.json
- filename: loop-onboarding-openapi-original.json
  format: json
  label: Loop Onboarding API
  slug: loop-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-onboarding-openapi-original.json
consequence_counts:
  physical: 9
  read: 26
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loop Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/artifacts/payable-invoice-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/artifacts/purchase-order-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/artifacts/receivable-invoice-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/artifacts/shipment-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/factoring-relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoicing-relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/organizations/create-organization-with-payment-detail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/receivable-invoices/{qid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/receivable-invoices/{qid}/void
operation_count: 41
overview: 'Loop exposes 41 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 6 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loop
provider_slug: loop
slug: loop-agentic-access
source_filename: loop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/loop-onboarding-openapi-original.json, openapi/loop-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    acting: 15\n    connected: 26\n  by_consequence:\n    physical: 9\n    read: 26\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/organizations/create-organization-with-payment-detail\n  method: post\n  operationId: Organizations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/artifact-ingestion-state\n  method: get\n  operationId: ArtifactIngestionState_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifact-ingestion-state/{qid}\n  method: get\n  operationId: ArtifactIngestionState_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts\n  method: post\n  operationId: Artifacts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/cost-coding-table-entry-list\n  method: post\n  operationId: CostCodingTableEntryListArtifact_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/organization-factor-assignment-record\n  method: post\n  operationId: OrganizationFactorAssignmentRecordArtifacts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/payable-invoice-record\n  method: post\n  operationId: CreatePayableInvoiceRecordArtifact_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/purchase-order-record\n  method: post\n  operationId: PurchaseOrderRecordArtifact_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/receivable-invoice-record\n  method: post\n  operationId: ReceivableInvoiceRecordArtifact_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/artifacts/shipment-record\n  method: post\n  operationId: ShipmentRecordArtifacts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/tagged/{tagType}/{tagTypeValue}\n  method: get\n  operationId: Artifacts_getByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts/{qid}\n  method: get\n  operationId: Artifacts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts/{qid}/download\n  method: get\n  operationId:\
  \ Artifacts_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-exceptions/target-entity-qid/{targetEntityQid}\n  method: get\n  operationId: BusinessExceptions_listForTargetEntityQid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-exceptions/{qid}\n  method: get\n  operationId: BusinessExceptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-exceptions/{qid}/resolve\n  method: put\n  operationId: BusinessExceptions_resolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/factoring-relationships\n  method: post\n  operationId: FactoringRelationships_upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/factoring-relationships\n  method: get\n  operationId: FactoringRelationships_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/factoring-relationships/{qid}\n  method: get\n  operationId: FactoringRelationships_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/invoicing-relationships\n  method: post\n  operationId: InvoicingRelationships_upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoicing-relationships\n  method: get\n  operationId: InvoicingRelationships_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoicing-relationships/{qid}\n  method: get\n  operationId: InvoicingRelationships_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: post\n  operationId: Organizations_create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/tagged/{tagType}/{tagTypeValue}\n  method: get\n  operationId: Organizations_getByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{qid}\n  method: get\n  operationId: Organizations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{qid}\n  method: put\n  operationId: Organizations_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payable-allocations\n  method: get\n  operationId: PayableAllocations_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payable-allocations/{qid}\n  method: get\n  operationId: PayableAllocations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payable-invoice-reviews\n  method: get\n  operationId: PayableInvoiceReview_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payable-invoices\n  method: get\n  operationId: PayableInvoices_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v1/payable-invoices/{qid}\n  method: get\n  operationId: PayableInvoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payable-invoices/{qid}/review\n  method: get\n  operationId: PayableInvoiceReview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments\n  method: get\n  operationId: Payments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{qid}\n  method: get\n  operationId: Payments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ping\n  method: get\n  operationId: Ping_ping\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receivable-invoices\n  method: get\n  operationId: ReceivableInvoices_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receivable-invoices/{qid}\n  method: get\n  operationId: ReceivableInvoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receivable-invoices/{qid}\n  method: delete\n  operationId: ReceivableInvoices_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/receivable-invoices/{qid}/void\n  method: put\n  operationId: ReceivableInvoices_void\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipment-jobs\n  method: get\n  operationId: ShipmentJobs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipment-jobs/{qid}\n  method: get\n  operationId: ShipmentJobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/agentic-access/loop-agentic-access.yml
summary_line: 41 operations · 15 acting
tags:
- Company
- Logistics
- Supply Chain
- Freight
- Freight Audit
- Payments
- Transportation
- Artificial Intelligence
- Data Platform
---
