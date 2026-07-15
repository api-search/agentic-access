---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 31
api_specs:
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Orders API
  slug: ezrentout-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Fixed Assets API
  slug: ezrentout-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Inventory API
  slug: ezrentout-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Bundles API
  slug: ezrentout-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Customers API
  slug: ezrentout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Members API
  slug: ezrentout-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Locations API
  slug: ezrentout-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Availability API
  slug: ezrentout-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Payments and Invoicing API
  slug: ezrentout-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Purchase Orders API
  slug: ezrentout-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Maintenance and Work Orders API
  slug: ezrentout-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
consequence_counts:
  physical: 18
  read: 31
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ezrentout Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /baskets.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/apply_taxes.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/cancel_reservation.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/charge_damages.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/charge_pre_payment.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/checkin.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/checkout.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/reservation.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /baskets/{orderNum}/update_basket_from_show.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inventory/{assetNum}/transfer_stock.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_orders.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /purchase_orders/{poId}.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /purchase_orders/{poId}/receive_items.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tasks.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tasks/{taskId}/end.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tasks/{taskId}/start.api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendors.api
operation_count: 71
overview: 'EZRentOut exposes 71 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 22 write, and 18 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EZRentOut
provider_slug: ezrentout
slug: ezrentout-agentic-access
source_filename: ezrentout-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ezrentout-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    connected: 31\n    acting: 40\n  by_consequence:\n    read: 31\n    physical: 18\n    write: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /baskets.api\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /baskets.api\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}.api\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /baskets/{orderNum}.api\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/history.api\n  method: get\n  operationId: getOrderHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /baskets/{orderNum}/update_basket_from_show.api\n  method: patch\n  operationId: addOrderLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/reservation.api\n  method: patch\n  operationId: reserveOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/cancel_reservation.api\n  method: patch\n  operationId: cancelOrderReservation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/checkout.api\n  method: patch\n  operationId: checkoutOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/checkin.api\n  method: patch\n  operationId: checkinOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets.api\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets.api\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/filter.api\n  method: get\n  operationId: filterAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetNum}.api\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetNum}.api\n  method: put\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetNum}.api\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetNum}/gps_coordinates.api\n  method: patch\n  operationId: updateAssetGps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetNum}/retire.api\n  method: put\n  operationId: retireAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search.api\n  method: get\n  operationId: searchCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory.api\n  method: get\n  operationId: listInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /inventory.api\n  method: post\n  operationId: createInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/{assetNum}.api\n  method: get\n  operationId: getInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/{assetNum}.api\n  method: put\n  operationId: updateInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/{assetNum}.api\n  method: delete\n  operationId: deleteInventory\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/{assetNum}/transfer_stock.api\n  method: post\n  operationId: transferInventoryStock\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stock_assets.api\n  method: get\n  operationId: listStockAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stock_assets.api\n  method: post\n  operationId: createStockAsset\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles.api\n  method: get\n  operationId: listBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles.api\n  method: post\n  operationId: createBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundleId}.api\n  method: get\n  operationId: getBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers.api\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers.api\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}.api\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}.api\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}.api\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses.api\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses.api\n  method: post\n  operationId: createBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.api\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts.api\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members.api\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members.api\n  method: post\n  operationId: createMember\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{userId}.api\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{userId}.api\n  method: patch\n  operationId: updateMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{userId}/checked_out_items.api\n  method: get\n  operationId: getMemberCheckedOutItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations.api\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations.api\n  method: post\n  operationId: createLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}.api\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}.api\n  method: patch\n  operationId: updateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/get_quantity_by_location.api\n  method: get\n  operationId: getQuantityByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetNum}/booked_dates.api\n  method: get\n  operationId: getAssetBookedDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/{assetNum}/booked_dates.api\n  method: get\n  operationId: getInventoryBookedDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_options.api\n  method: get\n\
  \  operationId: listPaymentOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing_coupons.api\n  method: get\n  operationId: listCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /baskets/{orderNum}/charge_pre_payment.api\n  method: patch\n  operationId: chargeOrderPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/charge_damages.api\n  method: patch\n  operationId: chargeOrderDamages\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{orderNum}/apply_taxes.api\n  method: patch\n  operationId: applyOrderTaxes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_orders.api\n  method: get\n  operationId: listPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_orders.api\n  method: post\n  operationId: createPurchaseOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_orders/{poId}.api\n  method: get\n  operationId: getPurchaseOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_orders/{poId}.api\n  method: patch\n  operationId: updatePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_orders/{poId}/receive_items.api\n\
  \  method: patch\n  operationId: receivePurchaseOrderItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendors.api\n  method: get\n  operationId: listVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendors.api\n  method: post\n  operationId: createVendor\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /services.api\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services.api\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{serviceId}/complete.api\n  method: patch\n  operationId: completeService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetNum}/maintenance.api\n  method: patch\n  operationId:\
  \ putAssetInMaintenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.api\n  method: post\n  operationId: createWorkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{taskId}.api\n  method: get\n  operationId: getWorkOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{taskId}/start.api\n  method: patch\n  operationId: startWorkOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{taskId}/end.api\n  method: patch\n  operationId: endWorkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/agentic-access/ezrentout-agentic-access.yml
summary_line: 71 operations · 40 acting
tags:
- Equipment Rental
- Rental Management
- Asset Tracking
- Inventory
- Order Management
- EZO
---
