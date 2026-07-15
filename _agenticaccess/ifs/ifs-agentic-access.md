---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: ifs-cloud-erp-openapi.yml
  format: yaml
  label: IFS Cloud ERP API
  slug: ifs-cloud-erp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-cloud-erp-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ifs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'IFS exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IFS
provider_slug: ifs
slug: ifs-agentic-access
source_filename: ifs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ifs-cloud-erp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /VOUCHER_API\n  method: get\n  operationId: listVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VOUCHER_API(AccountingYear='{accountingYear}',VoucherType='{voucherType}',VoucherNo={voucherNo},Company='{company}')\n  method: get\n  operationId: getVoucher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /PURCHASE_ORDER_API\n  method: get\n  operationId: listPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PURCHASE_ORDER_API(OrderNo='{orderNo}')\n  method: get\n  operationId: getPurchaseOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /WORK_ORDER_API\n  method: get\n  operationId: listWorkOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /WORK_ORDER_API(WoNo={woNo})\n  method: get\n  operationId: getWorkOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PART_CATALOG_API\n  method: get\n  operationId: listParts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/agentic-access/ifs-agentic-access.yml
summary_line: 7 operations
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
---
