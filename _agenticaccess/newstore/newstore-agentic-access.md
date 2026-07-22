---
acting_count: 79
action_class_counts:
  acting: 79
  connected: 71
api_specs:
- filename: newstore-api-openapi-original.json
  format: json
  label: NewStore Omnichannel API
  slug: newstore-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/openapi/newstore-api-openapi-original.json
consequence_counts:
  physical: 31
  read: 71
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Newstore Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/carts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /checkout/carts/{cartId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/carts/{cartId}/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /checkout/carts/{cartId}/items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /checkout/carts/{cartId}/items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/carts/{cartId}/items/{lineItemId}/add-ons
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /fulfillment/adapters/config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /fulfillment/adapters/config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfillment/configurations/shipments/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfillment/package-types
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /fulfillment/package-types/{package_type_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /fulfillment/package-types/{package_type_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /fulfillment/provider-rate-priorities
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /fulfillment/provider-rates/{provider_rate_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /fulfillment/provider-rates/{provider_rate_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment/providers/{newstore}/locations/{location}/mappings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment/providers/{newstore}/locations/{location}/mappings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /taxes/transactions/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/config/routing/can_update_ffr_processed_externally
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/config/routing/reroute_to_rejected_fulfillment_nodes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/config/routing/skip_shipping_offer_update_for_dc_orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/d/fulfill_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/fulfillment_request/{ffr_uuid}/set_items_states
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/orders/{id}/_extend_grace_period
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/orders/{id}/cancel
operation_count: 150
overview: 'Newstore exposes 150 API operations that an AI agent could call, of which 79 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 71 read, 48 write, and 31 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Newstore
provider_slug: newstore
slug: newstore-agentic-access
source_filename: newstore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/newstore-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 150\n  by_action_class:\n    acting: 79\n    connected: 71\n  by_consequence:\n    write: 48\n    read: 71\n    physical: 31\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog/import-schemas\n  method: post\n  operationId: createImportSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:import-schemas:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/import-schemas/{id}\n\
  \  method: delete\n  operationId: destroyImportSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:import-schemas:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/import-schemas/{id}\n  method: get\n  operationId: showImportSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:import-schemas:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/import-schemas/{id}\n  method: patch\n  operationId: updateImportSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:import-schemas:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/exports/catalogs/{catalog}/pricebooks/{pricebook}\n  method: get\n  operationId: showPricebookExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:pricebook-export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/catalogs/{catalog}/offlineproducts\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:product-export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/carts\n  method: post\n  operationId: createCart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout:carts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/carts/{cartId}\n  method: get\n  operationId: showCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout:carts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/carts/{cartId}\n  method: patch\n  operationId: updateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout:carts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/carts/{cartId}/items\n  method: post\n  operationId: createLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - checkout:carts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/carts/{cartId}/items/{lineItemId}\n  method: delete\n  operationId: destroyLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout:carts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/carts/{cartId}/items/{lineItemId}\n  method: patch\n  operationId: updateLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout:carts:write\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/carts/{cartId}/items/{lineItemId}/add-ons\n  method: post\n  operationId: createAddOnLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout:carts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clienteling/profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - clienteling:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clienteling/profiles/{customer_id}\n\
  \  method: get\n  operationId: showProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - clienteling:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/profiles/lookup-bulk-emails\n  method: post\n  operationId: createRetrievalBulkEmailProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/data\n  method: post\n  operationId: createData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /customer/data/{data_id}\n  method: delete\n  operationId: destroyData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/data/{data_id}\n  method: get\n  operationId: showData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/tokens\n  method: post\n  operationId: createTokensOperations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:read\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/profiles\n  method: get\n  operationId: GetlistProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/profiles\n  method: post\n  operationId: createOrShowProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/profiles/{profile_id}\n  method: get\n  operationId: GetshowProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer:profile:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/profiles/{profile_id}\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/profiles/{profile_id}\n  method: post\n  operationId: createProfileDeletionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/profiles/{profile_id}/addresses\n  method: get\n  operationId: listAddresses\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/profiles/{profile_id}/addresses\n  method: post\n  operationId: createOrShowAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/profiles/{profile_id}/addresses/{address_id}\n  method: delete\n  operationId: destroyAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /customer/profiles/{profile_id}/addresses/{address_id}\n  method: get\n  operationId: showAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer:profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/profiles/{profile_id}/addresses/{address_id}\n  method: patch\n  operationId: updateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer:profile:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/config\n  method: get\n  operationId: showConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /customer/config\n  method: patch\n  operationId: updateConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}\n  method: get\n  operationId: showStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}\n  method: patch\n  operationId: updateStore\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{storeId}/cashboxes\n  method: get\n  operationId: listCashboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}/cashboxes\n  method: post\n  operationId: createCashbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{storeId}/cashboxes/{cashboxId}\n\
  \  method: get\n  operationId: showCashbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}/cashboxes/{cashboxId}/release\n  method: post\n  operationId: createCashboxRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: showOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - fiscalization:orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/returns/{returnId}\n  method: get\n  operationId:\
  \ showReturn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - fiscalization:orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: showTenantConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/offline-mode\n  method: get\n  operationId: showTenantOfflineModeConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/offline-mode\n  method: patch\n  operationId: updateTenantOfflineModeConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/adapters/config\n  method: delete\n  operationId: destroyEasypostAdapterConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/adapters/config\n  method: get\n  operationId: showEasypostAdapterConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/adapters/config\n  method: put\n  operationId:\
  \ replaceEasypostAdapterConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/configurations/shipments/{name}\n  method: get\n  operationId: showConfigurationByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/configurations/shipments/{name}\n  method: post\n  operationId: createConfigurationByName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/configurations/shipments/checks\n  method: get\n  operationId: showConfigurationsChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/provider-rate-priorities\n  method: get\n  operationId: showProviderRatePriorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/provider-rate-priorities\n  method: put\n  operationId: replaceProviderRatePriorities\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/provider-rates\n  method: get\n  operationId: listProviderRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/provider-rates/{provider_rate_id}\n  method: delete\n  operationId: destroyProviderRate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/provider-rates/{provider_rate_id}\n  method: get\n  operationId: showProviderRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/provider-rates/{provider_rate_id}\n  method: put\n  operationId: replaceProviderRate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/shipping-audits\n  method: get\n  operationId: listShippingOptionAudits\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - shipments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/shipping-audits/{audit_id}\n  method: get\n  operationId: showShippingOptionAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - shipments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/shipping-labels/{public_key}\n  method: get\n  operationId: showShippingLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/package-types\n  method: get\n  operationId: listPackageTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/package-types\n  method: post\n  operationId: createPackageType\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/package-types/{package_type_id}\n  method: delete\n  operationId: destroyPackageType\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillment/package-types/{package_type_id}\n  method: get\n  operationId: showPackageType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillment/package-types/{package_type_id}\n\
  \  method: patch\n  operationId: updatePackageType\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:providers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:providers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /iam/providers/{alias}\n  method: delete\n  operationId: destroyProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:providers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/providers/{alias}\n  method: get\n  operationId: showProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:providers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/providers/{alias}\n  method: patch\n  operationId: updateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:providers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/supported-providers\n  method: get\n  operationId: listSupportedProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:providers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/users/{id}\n  method:\
  \ delete\n  operationId: destroyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/users/{id}\n  method: get\n  operationId: showUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/users/{id}\n  method: put\n  operationId: replaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/permissions\n\
  \  method: get\n  operationId: listPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:roles:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:roles:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/roles\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:roles:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/roles/{id}\n  method: delete\n  operationId: destroyRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - iam:roles:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/roles/{id}\n  method: get\n  operationId: showRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - iam:roles:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/roles/{id}\n  method: put\n  operationId: replaceRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - iam:roles:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/roles/{id}/users\n  method: get\n  operationId: listUsersByRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - iam:roles:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/config\n  method: get\n  operationId: showInventoryConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/config\n  method: put\n  operationId: replaceInventoryConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/config/reservations\n  method: get\n  operationId: showReservationConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - newstore:configuration:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/config/reservations\n  method: patch\n  operationId: updateReservationConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - newstore:configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inventory:reservations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/reservations\n  method: post\n  operationId: createReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - inventory:reservations:write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/reservations/{reservation_id}\n  method: get\n  operationId: showReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inventory:reservations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/reservations/{reservation_id}\n  method: patch\n  operationId: updateReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - inventory:reservations:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/reservations/{reservation_id}/items\n  method: patch\n  operationId: updateReservationItems\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - inventory:reservations:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/orders\n  method: get\n  operationId: showOrderHistoryForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/orders/{id}\n  method: get\n  operationId: showSalesOrderByIdAndIdType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/orders/{id}/_extend_grace_period\n  method: post\n  operationId: createGracePeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/orders/{id}/cancel\n  method: get\n  operationId: showCancellationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/orders/{id}/cancel\n  method: post\n  operationId: createCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/orders/{id}/items/{item_uuid}/cancel\n  method: post\n  operationId: createLineItemCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-\n\n# --- truncated at 32 KB (49 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/agentic-access/newstore-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/agentic-access/newstore-agentic-access.yml
summary_line: 150 operations · 79 acting
tags:
- Company
- Retail
- Omnichannel
- Order Management
- Point of Sale
- Ecommerce
- Fulfillment
- Inventory
- Store Operations
- REST
---
