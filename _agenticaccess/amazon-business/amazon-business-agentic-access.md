---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 13
api_specs:
- filename: amazon-business-openapi-generated.yml
  format: yaml
  label: Amazon Business API
  slug: amazon-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/_ae-authored/amazon-business-openapi-generated.yml
- filename: amazon-business-ab-invoice-api-openapi.yml
  format: yaml
  label: Amazon Business Ab Invoice API
  slug: amazon-business-ab-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/amazon-business-ab-invoice-api-openapi.yml
- filename: amazon-business-cart-api-openapi.yml
  format: yaml
  label: Amazon Business Cart API
  slug: amazon-business-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/amazon-business-cart-api-openapi.yml
- filename: amazon-business-ordering-api-openapi.yml
  format: yaml
  label: Amazon Business Ordering API
  slug: amazon-business-ordering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/amazon-business-ordering-api-openapi.yml
- filename: amazon-business-products-api-openapi.yml
  format: yaml
  label: Amazon Business Products API
  slug: amazon-business-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/amazon-business-products-api-openapi.yml
- filename: amazon-business-reports-api-openapi.yml
  format: yaml
  label: Amazon Business Reports API
  slug: amazon-business-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-business/openapi/amazon-business-reports-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Business Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordering/2022-10-30/orders
operation_count: 19
overview: 'Amazon Business exposes 19 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Business
provider_slug: amazon-business
slug: amazon-business-agentic-access
source_filename: amazon-business-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/amazon-business-ab-invoice-api-openapi.yml, openapi/amazon-business-cart-api-openapi.yml,\n  openapi/amazon-business-ordering-api-openapi.yml, openapi/amazon-business-products-api-openapi.yml,\n  openapi/amazon-business-reports-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 13\n    acting: 6\n  by_consequence:\n    read: 13\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ab-invoice/2026-02-01/invoices\n  method: get\n  operationId: get_ab_invoice_2026_02_01_invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /ab-invoice/2026-02-01/invoices/{invoicenumber}\n  method: get\n  operationId: get_ab_invoice_2026_02_01_invoices_invoicenumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ab-invoice/2026-02-01/invoices/{invoicenumber}/lineItems\n  method: get\n  operationId: get_ab_invoice_2026_02_01_invoices_invoicenumber_lineItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/2025-04-30/carts\n  method: get\n  operationId: get_cart_2025_04_30_carts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/2025-04-30/carts/{cartid}\n  method: get\n  operationId: get_cart_2025_04_30_carts_cartid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/2025-04-30/carts/{cartid}/items\n  method: delete\n  operationId: delete_cart_2025_04_30_carts_cartid_items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/2025-04-30/carts/{cartid}/items\n  method: get\n  operationId: get_cart_2025_04_30_carts_cartid_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/2025-04-30/carts/{cartid}/items\n  method: patch\n  operationId: patch_cart_2025_04_30_carts_cartid_items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/2025-04-30/carts/{cartid}/{id}\n  method: post\n  operationId: post_cart_2025_04_30_carts_cartid_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordering/2022-10-30/orders\n  method: post\n  operationId: post_ordering_2022_10_30_orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordering/2022-10-30/orders/{externalid}\n\
  \  method: get\n  operationId: get_ordering_2022_10_30_orders_externalid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/2020-08-26/products\n  method: get\n  operationId: get_products_2020_08_26_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/2020-08-26/products/B091WR26F4/offers\n  method: get\n  operationId: get_products_2020_08_26_products_B091WR26F4_offers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/2020-08-26/products/getProductsByAsins\n  method: post\n  operationId: post_products_2020_08_26_products_getProductsByAsins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /reports/2021-09-30/documents/{reportdocumentid}\n  method: get\n  operationId: get_reports_2021_09_30_documents_reportdocumentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/2021-09-30/reports\n  method: get\n  operationId: get_reports_2021_09_30_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/2021-09-30/reports\n  method: post\n  operationId: post_reports_2021_09_30_reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/2021-09-30/reports/{reportid}\n  method:\
  \ delete\n  operationId: delete_reports_2021_09_30_reports_reportid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/2021-09-30/reports/{reportid}\n  method: get\n  operationId: get_reports_2021_09_30_reports_reportid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/amazon-business/agentic-access/amazon-business-agentic-access.yml
summary_line: 19 operations · 6 acting
tags:
- Company
- B2B
- Procurement
- Marketplace
- BulkPurchasing
---
