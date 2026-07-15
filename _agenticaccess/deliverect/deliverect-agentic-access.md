---
acting_count: 71
action_class_counts:
  acting: 71
  connected: 33
api_specs:
- filename: deliverect-pos-api-openapi-original.yml
  format: yaml
  label: Deliverect POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pos-api-openapi-original.yml
- filename: deliverect-commerce-api-openapi-original.yml
  format: yaml
  label: Deliverect Commerce API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-commerce-api-openapi-original.yml
- filename: deliverect-channel-api-openapi-original.yml
  format: yaml
  label: Deliverect Channel API
  slug: channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-channel-api-openapi-original.yml
- filename: deliverect-dispatch-api-openapi-original.yml
  format: yaml
  label: Deliverect Dispatch API
  slug: dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-dispatch-api-openapi-original.yml
- filename: deliverect-store-api-openapi-original.yml
  format: yaml
  label: Deliverect Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-store-api-openapi-original.yml
- filename: deliverect-pay-api-openapi-original.yml
  format: yaml
  label: Deliverect Pay API
  slug: pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pay-api-openapi-original.yml
- filename: deliverect-crm-api-openapi-original.yml
  format: yaml
  label: Deliverect CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-crm-api-openapi-original.yml
- filename: deliverect-loyalty-api-openapi-original.yml
  format: yaml
  label: Deliverect Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-loyalty-api-openapi-original.yml
- filename: deliverect-kds-api-openapi-original.yml
  format: yaml
  label: Deliverect KDS API
  slug: kds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-kds-api-openapi-original.yml
- filename: deliverect-gift-cards-api-openapi-original.yml
  format: yaml
  label: Deliverect Gift Cards API
  slug: gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-gift-cards-api-openapi-original.yml
consequence_counts:
  physical: 23
  read: 33
  safety-critical: 5
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Deliverect Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/cancel_job
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/create_job
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/updateJob
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fulfillment/validate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /validate_job
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /channel/amendments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /channel/order_status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /channel/payment_update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /channel/prep_time
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /commerce/{accountId}/baskets/{basketId}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /commerce/{accountId}/v2/checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfillment/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfillment/generic/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /giftCards/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /kds/orderStatus/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /kds/order_status_update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /kds_order_notification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orderStatus/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pay/channel/{channelLinkId}/payments/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pay/channel/{channelLinkId}/payments/{paymentId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /register
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /unregister-profile
operation_count: 104
overview: 'Deliverect exposes 104 API operations that an AI agent could call, of which 71 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 43 write, 23 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deliverect
provider_slug: deliverect
slug: deliverect-agentic-access
source_filename: deliverect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deliverect-channel-api-openapi-original.yml, openapi/deliverect-commerce-api-openapi-original.yml,\n  openapi/deliverect-crm-api-openapi-original.yml, openapi/deliverect-dispatch-api-openapi-original.yml,\n  openapi/deliverect-gift-cards-api-openapi-original.yml, openapi/deliverect-kds-api-openapi-original.yml,\n  openapi/deliverect-loyalty-api-openapi-original.yml, openapi/deliverect-pay-api-openapi-original.yml,\n  openapi/deliverect-pos-api-openapi-original.yml, openapi/deliverect-store-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 104\n  by_action_class:\n    acting: 71\n    connected: 33\n  by_consequence:\n    physical: 23\n    write: 43\n    read: 33\n\
  \    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /{channelName}/order/{channelLinkId}\n  method: post\n  operationId: post_channelname_order_channellinkid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/order_status\n  method: post\n  operationId: channel_order_status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/menu_update/\n  method: post\n  operationId: channel_menu_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/snooze\n  method: post\n  operationId: channel_snooze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/busy_mode\n  method: post\n  operationId: channel_busy_mode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/courier_update\n\
  \  method: post\n  operationId: channel_courier_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/prep_time\n  method: post\n  operationId: channel_prep_time\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/register\n  method: post\n  operationId: channel_register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/amendments\n  method: post\n  operationId: channel_amendments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/payment_update\n  method: post\n  operationId: channel_payment_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/channels/{locationId}/holidays\n  method: get\n  operationId:\
  \ get_locations_channels_locationid_holidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channelLinks\n  method: get\n  operationId: get_channellinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allChannels\n  method: get\n  operationId: get_allchannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: get_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{channelName}/menuStatus/{_id}\n  method: post\n  operationId: post_channelname_menustatus_id\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{channelName}/updateStoreStatus/{channelLinkId}\n  method: post\n  operationId: post_channelname_updatestorestatus_channellinkid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{channelName}/updateRating\n  method: post\n  operationId: post_channelname_updaterating\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{channelName}/courierUpdate/{channelLinkId}\n  method: post\n  operationId: post_channelname_courierupdate_channellinkid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/recreate\n  method: post\n  operationId: post_commerce_accountid_baskets_recreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/stores/{channelLinkId}\n  method: get\n  operationId: commerce_channel_api_stores_get_store\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/{accountId}/menus\n  method: get\n  operationId: commerce_channel_api_menus_get_root_menus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/{accountId}/baskets\n  method: post\n  operationId: commerce_channel_api_baskets_create_basket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/{basketId}\n  method: get\n  operationId: commerce_channel_api_baskets_get_basket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /commerce/{accountId}/v2/checkouts\n  method: post\n  operationId: post_commerce_accountId_checkouts_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/v2/checkouts/{checkoutId}\n  method: get\n  operationId: get_commerce_accountId_checkouts_checkoutId_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/{accountId}/baskets/{basketId}/validate\n  method: post\n  operationId: post_commerce_accountid_baskets_basketid_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/{basketId}/items\n  method: patch\n  operationId: commerce_channel_api_baskets_update_basket_items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/{basketId}/customer\n  method: patch\n  operationId: commerce_channel_api_baskets_update_basket_customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /commerce/{accountId}/baskets/{basketId}/discounts\n  method: patch\n  operationId: commerce_channel_api_baskets_update_basket_discounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/{basketId}/payment\n  method: patch\n  operationId: patch_commerce_accountid_baskets_basketid_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/baskets/{basketId}/store\n  method: patch\n  operationId:\
  \ patch_commerce_accountid_baskets_basketid_store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/{accountId}/stores\n  method: get\n  operationId: commerce_channel_api_stores_get_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/{accountId}/stores/{channelLinkId}/menus\n  method: get\n  operationId: commerce_channel_api_stores_get_store_menus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coupons/channel/{channelLinkId}/coupons\n  method: get\n  operationId: get_couponsadmin_accountId_coupons_couponId_1\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upsell/channel/{channelLinkId}\n  method: post\n  operationId: getUpsellItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers\n  method: post\n  operationId: post_crm_accountid_customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/lookup\n  method: post\n  operationId: post_crm_accountid_customers_lookup\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/{crmProfileId}\n  method: get\n  operationId: get_crm_accountid_customers_crmprofileid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/{accountId}/customers/{crmProfileId}\n  method: patch\n  operationId: patch_crm_accountid_customers_crmprofileid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/{crmProfileId}/deliveryAddresses\n  method:\
  \ patch\n  operationId: patch_crm_accountid_customers_crmprofileid_deliveryaddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/{crmProfileId}/vehicles\n  method: patch\n  operationId: patch_crm_accountid_customers_crmprofileid_vehicles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/{crmProfileId}/favorites\n  method: patch\n  operationId: patch_crm_accountid_customers_crmprofileid_favorites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/{accountId}/customers/{crmProfileId}/orders\n  method: get\n  operationId: get_crm_accountid_customers_crmprofileid_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/{accountId}/orders/{crmOrderId}\n  method: get\n  operationId: get_crm_accountid_orders_crmorderid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/{accountId}/customers/{crmProfileId}/orders/favorites\n  method: get\n  operationId: get_crm_accountid_customers_crmprofileid_orders_favorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /validate_job\n  method: post\n  operationId: dispatch_validate_job\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/create_job\n  method: post\n  operationId: dispatch_create_job\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/updateJob\n  method: post\n  operationId: dispatch_updatejob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/cancel_job\n  method: post\n  operationId: dispatch_cancel_job\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fulfillment/validate\n  method: post\n  operationId: post_fulfillment_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /fulfillment/cancel\n  method: post\n  operationId: post_post_fulfillment_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/generic/events\n  method: post\n  operationId: post_post_fulfillment_generic_events\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /giftCards/channel/{channelLinkId}/profileLink/{giftCardProviderProfileLinkId}/applyGiftCard\n  method:\
  \ post\n  operationId: post_giftcards_channel_channellinkid_profilelink_giftcardproviderprofilelinkid_applygiftcard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /giftCards/channel/{channelLinkId}/profileLink/{giftCardProviderProfileLinkId}/getGiftCardBalance\n  method: post\n  operationId: post_giftcards_channel_channellinkid_profilelink_giftcardproviderprofilelinkid_getgiftcardbalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /giftCards/redeem\n  method: post\n  operationId: giftcards_redeem\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /giftCards/registerProfile\n  method: post\n  operationId: giftcards_registerprofile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /giftCards/reverse\n  method: post\n  operationId: giftcards_reverse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /giftCards/channel/{channelLinkId}/providerProfileLinks\n  method: get\n  operationId: get_giftcards_channel_channellinkid_providerprofilelinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kds_order_notification\n  method: post\n  operationId: kds_order_notification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kds/order_status_update\n  method: post\n  operationId: kds_order_status_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kds/productUpdate\n  method: post\n  operationId: kds_productupdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kds/register_kds\n  method: post\n  operationId: kds_register_kds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kds/orderStatus/{orderId}\n  method: post\n  operationId: post_post_kds_orderstatus_orderid\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loyalty/{channelLinkId}/customer\n  method: post\n  operationId: loyalty_channel_create_loyalty_customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loyalty/{channelLinkId}/customer\n  method: get\n  operationId: loyalty_channel_get_customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/{channelLinkId}/configuration\n\
  \  method: get\n  operationId: loyalty_channel_get_configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/{channelLinkId}/programs/retrieve\n  method: post\n  operationId: loyalty_channel_get_programs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loyalty/{channelLinkId}/compensationCards/validate\n  method: post\n  operationId: post_loyalty_channellinkid_compensationcards_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /loyalty/{channelLinkId}/programs/validate\n  method: post\n  operationId: post_new_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token\n  method: post\n  operationId: loyalty_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/channel/{channelLinkId}/gatewayProfiles\n  method: get\n  operationId: pay_endpoints_get_payment_gateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /pay/channel/{channelLinkId}/payments/request\n  method: post\n  operationId: pay_endpoints_request_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/channel/{channelLinkId}/payments/{paymentId}\n  method: get\n  operationId: pay_endpoints_get_payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/channel/{channelLinkId}/payments/{paymentId}/refund\n  method: post\n  operationId: pay_endpoints_refund_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request\n  method: post\n  operationId: payplatform_payments_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refund\n  method: post\n  operationId: payplatform_payments_refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /register\n  method: post\n  operationId: payplatform_payments_profile_register\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unregister-profile\n  method: post\n  operationId: payplatform_payments_unregister_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: post\n  operationId: pos_register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syncProducts\n  method: get\n  operationId: pos_syncproducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: pos_ordercancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /floors/locationId\n  method: get\n  operationId: pos_floors_locationid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /tables/locationId\n  method: get\n  operationId: pos_tables_locationid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/{locationId}/syncProducts\n  method: get\n  operationId: get_v2_locations_locationid_syncproducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productAndCategories\n  method: post\n  operationId: insertUpdateProductsAndCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product_sync_callback\n  method: post\n  operationId: pos_api_product_sync_callback\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/accounts/{accountId}/inventoryUploadUrl\n  method: post\n  operationId: inventory_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orderStatus/{orderId}\n  method: post\n  operationId: post_orderstatus_orderid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/location/{orderId}\n  method: get\n  operationId: order_delivery_update\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updatePreparationTime\n  method: post\n  operationId: post_updatepreparationtime\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations\n  method: get\n  operationId: get_get_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId:\
  \ get_products\n  x-agentic-access:\n    action-class: connec\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/agentic-access/deliverect-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/agentic-access/deliverect-agentic-access.yml
summary_line: 104 operations · 71 acting · 5 human-in-the-loop
tags:
- Restaurant
- Delivery
- Online Ordering
- Point of Sale
- Order Management
- Integration
---
