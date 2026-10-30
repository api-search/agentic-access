---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 46
api_specs:
- filename: bol-com-commissions-api-openapi.yml
  format: yaml
  label: Bol Commissions API
  slug: bol-com-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-commissions-api-openapi.yml
- filename: bol-com-insights-api-openapi.yml
  format: yaml
  label: Bol Insights API
  slug: bol-com-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-insights-api-openapi.yml
- filename: bol-com-inventory-api-openapi.yml
  format: yaml
  label: Bol Inventory API
  slug: bol-com-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-inventory-api-openapi.yml
- filename: bol-com-invoices-api-openapi.yml
  format: yaml
  label: Bol Invoices API
  slug: bol-com-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-invoices-api-openapi.yml
- filename: bol-com-offers-api-openapi.yml
  format: yaml
  label: Bol Offers API
  slug: bol-com-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-offers-api-openapi.yml
- filename: bol-com-orders-api-openapi.yml
  format: yaml
  label: Bol Orders API
  slug: bol-com-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-orders-api-openapi.yml
- filename: bol-com-products-api-openapi.yml
  format: yaml
  label: Bol Products API
  slug: bol-com-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-products-api-openapi.yml
- filename: bol-com-promotions-api-openapi.yml
  format: yaml
  label: Bol Promotions API
  slug: bol-com-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-promotions-api-openapi.yml
- filename: bol-com-replenishments-api-openapi.yml
  format: yaml
  label: Bol Replenishments API
  slug: bol-com-replenishments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-replenishments-api-openapi.yml
- filename: bol-com-retailers-api-openapi.yml
  format: yaml
  label: Bol Retailers API
  slug: bol-com-retailers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-retailers-api-openapi.yml
- filename: bol-com-returns-api-openapi.yml
  format: yaml
  label: Bol Returns API
  slug: bol-com-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-returns-api-openapi.yml
- filename: bol-com-shipments-api-openapi.yml
  format: yaml
  label: Bol Shipments API
  slug: bol-com-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-shipments-api-openapi.yml
- filename: bol-com-shipping-labels-api-openapi.yml
  format: yaml
  label: Bol Shipping Labels API
  slug: bol-com-shipping-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-shipping-labels-api-openapi.yml
- filename: bol-com-subscriptions-api-openapi.yml
  format: yaml
  label: Bol Subscriptions API
  slug: bol-com-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-subscriptions-api-openapi.yml
- filename: bol-com-transports-api-openapi.yml
  format: yaml
  label: Bol Transports API
  slug: bol-com-transports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/openapi/bol-com-transports-api-openapi.yml
consequence_counts:
  physical: 5
  read: 46
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bol Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /retailer/orders/cancellation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /retailer/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /retailer/shipments/invoices/{shipment-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /retailer/shipping-labels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /retailer/subscriptions/test/{subscription-id}
operation_count: 69
overview: 'Bol exposes 69 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 18 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bol
provider_slug: bol-com
slug: bol-com-agentic-access
source_filename: bol-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/bol-com-retailer-api-v10.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 46\n    acting: 23\n  by_consequence:\n    read: 46\n    write: 18\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /retailer/commission\n  method: post\n  operationId: get-commissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/commission/{ean}\n  method: get\n  operationId: get-commission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /retailer/commissions\n  method: post\n  operationId: get-commission-rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/insights/offer\n  method: get\n  operationId: get-offer-insights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/insights/performance/indicator\n  method: get\n  operationId: get-performance-indicators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/insights/product-ranks\n  method: get\n  operationId: get-product-ranks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/insights/sales-forecast\n\
  \  method: get\n  operationId: get-sales-forecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/insights/search-terms\n  method: get\n  operationId: get-search-terms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/inventory\n  method: get\n  operationId: get-inventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/invoices\n  method: get\n  operationId: get-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/invoices/{invoice-id}\n  method: get\n  operationId: get-invoice\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/invoices/{invoice-id}/specification\n  method: get\n  operationId: get-invoice-specification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/offers\n  method: post\n  operationId: post-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/export\n  method: post\n  operationId: post-offer-export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/export/{report-id}\n  method: get\n  operationId: get-offer-export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/offers/unpublished\n  method: post\n  operationId: post-unpublished-offer-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/unpublished/{report-id}\n  method: get\n  operationId: get-unpublished-offer-report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/offers/{offer-id}\n  method: get\n  operationId: get-offer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/offers/{offer-id}\n  method: put\n  operationId: put-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/{offer-id}\n  method: delete\n  operationId: delete-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/{offer-id}/price\n  method: put\n  operationId: update-offer-price\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/offers/{offer-id}/stock\n  method: put\n  operationId: update-offer-stock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/orders\n  method: get\n  operationId: get-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/orders/cancellation\n  method: put\n  operationId: cancel-order-item\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/orders/{order-id}\n  method: get\n  operationId: get-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/categories\n  method: get\n  operationId: get-product-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/list\n  method: post\n  operationId: get-product-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/list-filters\n  method: get\n  operationId: get-product-list-filters\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/assets\n  method: get\n  operationId: get-product-assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/offers\n  method: get\n  operationId: get-competing-offers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/placement\n  method: get\n  operationId: get-product-placement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/price-star-boundaries\n  method: get\n  operationId: get-price-star-boundaries\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/product-ids\n  method: get\n  operationId: get-product-ids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/products/{ean}/ratings\n  method: get\n  operationId: get-product-ratings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/promotions\n  method: get\n  operationId: get-promotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/promotions/{promotion-id}\n  method: get\n  operationId: get-promotion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/promotions/{promotion-id}/products\n  method: get\n  operationId: get-products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments\n  method: get\n  operationId: get-replenishments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments\n  method: post\n  operationId: post-replenishment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/replenishments/delivery-dates\n  method: get\n  operationId: get-delivery-dates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments/pickup-time-slots\n  method: post\n  operationId: post-pickup-time-slots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/replenishments/product-destinations\n  method: post\n  operationId: post-request-product-destinations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/replenishments/product-destinations/{product-destinations-id}\n  method: get\n\
  \  operationId: get-product-destinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments/product-labels\n  method: post\n  operationId: post-product-labels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/replenishments/{replenishment-id}\n  method: get\n  operationId: get-replenishment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments/{replenishment-id}\n  method: put\n  operationId: put-replenishment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/replenishments/{replenishment-id}/load-carrier-labels\n  method: get\n  operationId: get-load-carrier-labels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/replenishments/{replenishment-id}/pick-list\n  method: get\n  operationId: get-pick-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/retailers/{retailer-id}\n  method: get\n  operationId: get-retailer-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/returns\n  method:\
  \ get\n  operationId: get-returns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/returns\n  method: post\n  operationId: create-return\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/returns/{return-id}\n  method: get\n  operationId: get-return\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/returns/{rma-id}\n  method: put\n  operationId: handle-return\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/shipments\n  method: get\n  operationId: get-shipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/shipments\n  method: post\n  operationId: create-shipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/shipments/invoices/requests\n  method: get\n  operationId: get-invoice-requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/shipments/invoices/{shipment-id}\n\
  \  method: post\n  operationId: upload-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/shipments/{shipment-id}\n  method: get\n  operationId: get-shipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/shipping-labels\n  method: post\n  operationId: post-shipping-label\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /retailer/shipping-labels/delivery-options\n  method: post\n  operationId: get-delivery-options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/shipping-labels/{shipping-label-id}\n  method: get\n  operationId: get-shipping-label\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/subscriptions\n  method: get\n  operationId: get-push-notification-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/subscriptions\n  method: post\n  operationId: post-push-notification-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/subscriptions/signature-keys\n  method: get\n  operationId: get-subscription-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/subscriptions/test/{subscription-id}\n  method: post\n  operationId: post-test-push-notification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/subscriptions/{subscription-id}\n  method: get\n  operationId: get-push-notification-subscription\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retailer/subscriptions/{subscription-id}\n  method: put\n  operationId: put-push-notification-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/subscriptions/{subscription-id}\n  method: delete\n  operationId: delete-push-notification-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retailer/transports/{transport-id}\n  method: put\n  operationId: add-transport-information-by-transport-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bol-com/refs/heads/main/agentic-access/bol-com-agentic-access.yml
summary_line: 69 operations · 23 acting
tags:
- e-commerce
- marketplace
- retail
- api
- Netherlands
---
