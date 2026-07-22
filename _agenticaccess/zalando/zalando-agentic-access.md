---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 31
api_specs:
- filename: zalando-orders-openapi.yml
  format: yaml
  label: zDirect Platform Orders API
  slug: zalando-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-orders-openapi.yml
- filename: zalando-products-openapi.yml
  format: yaml
  label: zDirect Platform Products API
  slug: zalando-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-products-openapi.yml
- filename: zalando-product-attributes-openapi.yml
  format: yaml
  label: Merchant Product Attributes API
  slug: zalando-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-product-attributes-openapi.yml
- filename: zalando-article-requirements-openapi.yml
  format: yaml
  label: Article Requirements API
  slug: zalando-article-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-article-requirements-openapi.yml
- filename: zalando-prices-openapi.yml
  format: yaml
  label: Merchant Price Service API
  slug: zalando-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-prices-openapi.yml
- filename: zalando-price-reporting-openapi.yml
  format: yaml
  label: Price Reporting API
  slug: zalando-price-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-price-reporting-openapi.yml
- filename: zalando-stocks-openapi.yml
  format: yaml
  label: Merchant Stock Service API
  slug: zalando-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-stocks-openapi.yml
- filename: zalando-offer-blocking-openapi.yml
  format: yaml
  label: Article Availability (Offer Blocking) API
  slug: zalando-offer-blocking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-offer-blocking-openapi.yml
- filename: zalando-sales-channels-openapi.yml
  format: yaml
  label: Sales Channels API
  slug: zalando-sales-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-sales-channels-openapi.yml
- filename: zalando-logistic-centers-openapi.yml
  format: yaml
  label: Logistic Centers API
  slug: zalando-logistic-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-logistic-centers-openapi.yml
- filename: zalando-zfs-stock-movements-openapi.yml
  format: yaml
  label: ZFS Stock Movements API
  slug: zalando-zfs-stock-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-stock-movements-openapi.yml
- filename: zalando-zfs-cross-border-movements-openapi.yml
  format: yaml
  label: ZFS Cross-Border Movements Report API
  slug: zalando-zfs-cross-border-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-cross-border-movements-openapi.yml
consequence_counts:
  physical: 4
  read: 31
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zalando Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /merchants/{merchant-id}/orders/{order-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}/lines/{order-line-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchants/{merchant-id}/orders/{order-id}/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /merchants/{merchant-id}/orders/{order-id}/shipments/{shipment-id}
operation_count: 41
overview: 'Zalando exposes 41 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zalando
provider_slug: zalando
slug: zalando-agentic-access
source_filename: zalando-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/zalando-article-requirements-openapi.yml, openapi/zalando-logistic-centers-openapi.yml,\n  openapi/zalando-offer-blocking-openapi.yml, openapi/zalando-orders-openapi.yml, openapi/zalando-price-reporting-openapi.yml,\n  openapi/zalando-prices-openapi.yml, openapi/zalando-product-attributes-openapi.yml, openapi/zalando-products-openapi.yml,\n  openapi/zalando-sales-channels-openapi.yml, openapi/zalando-stocks-openapi.yml, openapi/zalando-zfs-cross-border-movements-openapi.yml,\n  openapi/zalando-zfs-stock-movements-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 31\n    acting: 10\n  by_consequence:\n    read: 31\n    write: 6\n    physical:\
  \ 4\n  human_in_the_loop_required: 0\noperations:\n- path: /partners/{businessPartnerId}/attribute-types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{businessPartnerId}/attribute-types/{typeLabel}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{businessPartnerId}/attribute-types/{typeLabel}/attributes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{businessPartnerId}/attribute-types/{typeLabel}/attributes/{attributeLabel}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/logistic-centers\n\
  \  method: get\n  operationId: get-logistic-centers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profile/logistic-centers/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/logistic-centers/{logisticCenterId}\n  method: get\n  operationId: get-logistic-center\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profile/logistic-centers/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/offer-blockers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products/blockers/write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/offer-blockers\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/blockers/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/offer-blockers\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products/blockers/write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/offer-blockers/{offer-blocker-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/blockers/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders/write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/orders/{order-id}/transitions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/shipments\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/shipments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders/write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/orders/{order-id}/shipments/{shipment-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/shipments/{shipment-id}\n  method: patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders/write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/orders/{order-id}/items\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}/lines\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}/lines/{order-line-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}/lines/{order-line-id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders/write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/orders/{order-id}/items/{order-item-id}/lines/{order-line-id}/transitions\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/orders-deletion-requests\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/announced-returns\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/price-attempts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products/price/read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant-id}/prices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products/price/write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchant_id}/outlines\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/attributes/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant_id}/outlines/{outline_label}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/attributes/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant_id}/attribute-types/{type_label}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/attributes/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant_id}/attribute-types/{type_label}/attributes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/attributes/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant_id}/attribute-types/{type_label}/attributes/{attribute_label}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products/attributes/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant_id}/products/identifiers/{ean}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lemur.prototype.write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/identifiers/{ean}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lemur.prototype.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sales-channels\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profile/sales-channels/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchant-id}/stocks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products/stock/write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /cross-border-movements/{merchant_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zfs.icm-reports.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/received-items/{merchant-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - partner-inbound-tracker.received.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /returned-items/{merchant-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zfs/returned-item/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liquidated-items/{merchant-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zfs/liquidated-item/read\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/agentic-access/zalando-agentic-access.yml
summary_line: 41 operations · 10 acting
tags:
- Company
- Consumer; Marketplace
- Fashion
- E-Commerce
- Retail
- Marketplace
- Fulfillment
- Merchant Platform
- Orders
- Products
---
