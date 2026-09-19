---
acting_count: 56
action_class_counts:
  acting: 56
  connected: 35
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: grubhub-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: grubhub-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: grubhub-merchant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: grubhub-merchant-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-busy-intervals-openapi.yml
  format: yaml
  label: Grubhub Busy Intervals API
  slug: grubhub-busy-intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-busy-intervals-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: grubhub-deliveries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-connect-endpoints-openapi.yml
  format: yaml
  label: Grubhub Connect (Delivery as a Service) API
  slug: grubhub-connect-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-endpoints-openapi.yml
- filename: grubhub-connect-webhooks-openapi.yml
  format: yaml
  label: Grubhub Connect Webhooks
  slug: grubhub-connect-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-webhooks-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: grubhub-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
- filename: grubhub-reporting-endpoints-openapi.yml
  format: yaml
  label: Grubhub Merchant Reporting API
  slug: grubhub-reporting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-endpoints-openapi.yml
- filename: grubhub-reporting-webhooks-openapi.yml
  format: yaml
  label: Grubhub Reporting Webhooks
  slug: grubhub-reporting-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-webhooks-openapi.yml
- filename: grubhub-testing-openapi.yml
  format: yaml
  label: Grubhub Testing API
  slug: grubhub-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-testing-openapi.yml
consequence_counts:
  physical: 16
  read: 35
  safety-critical: 5
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Grubhub Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/external
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pos/v1/merchant/{merchant_id}/schedules/closenow
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pos/v1/merchant/{merchant_id}/schedules/overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /pos/v1/merchant/{merchant_id}/schedules/overrides
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/daas/v1/test/webhook/emulateRefundUpdateWebhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/daas/v1/test/{deliveryId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/daas/v1/{deliveryId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/fulfillment/deliveryboundaries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/fulfillment/estimates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/fulfillment/{delivery_area_id}/deliveryfee
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_id}/orders/{order_uuid}/addpickupinstructions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/preorderwindow
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/scheduledorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_id}/schedules/opennow
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/changerequests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_long_id}/test/jitevent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_long_id}/test/transmission
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v2/merchant/pos-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v2/merchant/{merchant_id}/pos-status
operation_count: 91
overview: 'Grubhub exposes 91 API operations that an AI agent could call, of which 56 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 35 write, 16 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Grubhub
provider_slug: grubhub
slug: grubhub-agentic-access
source_filename: grubhub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/grubhub-busy-intervals-openapi.yml, openapi/grubhub-connect-endpoints-openapi.yml,\n  openapi/grubhub-deliveries-openapi.yml, openapi/grubhub-menu-openapi.yml, openapi/grubhub-merchant-data-openapi.yml,\n  openapi/grubhub-merchant-schedules-openapi.yml, openapi/grubhub-onboarding-openapi.yml, openapi/grubhub-orders-openapi.yml,\n  openapi/grubhub-reporting-endpoints-openapi.yml, openapi/grubhub-testing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 91\n  by_action_class:\n    acting: 56\n    connected: 35\n  by_consequence:\n    write: 35\n    read: 35\n    physical: 16\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /pos/v1/merchant/{merchant_id}/busy/{busy_interval_id}\n\
  \  method: put\n  operationId: updateBusyMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/busy\n  method: get\n  operationId: getBusyMode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/busy\n  method: post\n  operationId: setBusyMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/busy\n  method: delete\n  operationId:\
  \ deleteActiveBusyMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/tip\n  method: post\n  operationId: updateCourierTip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/refund\n  method: post\n  operationId: requestRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/proxy\n  method: post\n  operationId: createProxyPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/pickupVerification\n  method: post\n  operationId: updatePickupVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/pickupReady\n  method: post\n  operationId: pickupReady\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/dropoff\n  method: post\n  operationId: updateDeliveryDropoffLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}/cancel\n  method: post\n  operationId: cancelDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/test/{deliveryId}/refund\n\
  \  method: post\n  operationId: progressRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/test/{deliveryId}/deliveryState\n  method: post\n  operationId: progressDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/test/webhook/emulateStatusUpdateWebhook\n  method: post\n  operationId: emulateStatusUpdateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/test/webhook/emulateRefundUpdateWebhook\n  method: post\n  operationId: emulateRefundUpdateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/quote/{quoteId}/accept\n  method: post\n  operationId: acceptDeliveryQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /delivery/daas/v1/quote\n  method: post\n  operationId: requestDeliveryQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/daas/v1/{deliveryId}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery/daas/v1/servicearea\n  method: get\n  operationId: getServiceAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/delivery\n  method: get\n  operationId: getExternalDeliveryByOrderUuid\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/deliveries/{delivery_id}\n  method: get\n  operationId: getExternalDeliveryByDeliveryId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/menu/ingestion/validate\n  method: post\n  operationId: validatePosMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/menu/ingestion\n  method: post\n  operationId: addOrUpdatePosFullMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/external\n  method: patch\n  operationId: bulkAddOrUpdateSchedulesOverridesByExternalIds\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides\n  method: get\n  operationId: getSchedulesOverridesForMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides\n  method: patch\n  operationId: bulkAddOrUpdateSchedulesOverridesByInternalIds\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/menu/entities/tags/alcohol\n  method: patch\n  operationId: tagProductsAsAlcoholic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/{job_id}/status\n  method: get\n  operationId: getBulkScheduleOverrideStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/menu/normalized\n\
  \  method: get\n  operationId: findNormalizedMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/menu/entities/tags/{job_id}/status\n  method: get\n  operationId: getBulkSupplementalTagStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/menu/ingestion/jobs/{job_id}\n  method: get\n  operationId: getMenuIngestionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v2/merchant/{merchant_id}/pos-status\n  method: put\n  operationId: updateMerchantStatusByOrderType\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v2/merchant/pos-status\n  method: put\n  operationId: updateMerchantStatusByOrderTypeBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/taxrate\n  method: get\n  operationId: getMerchantTaxRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/taxrate\n  method: put\n  operationId: updateMerchantTaxRate\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/scheduledorders\n  method: put\n  operationId: updateOptInOrOutScheduledOrdersByLegacyId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/preorderwindow\n  method: put\n  operationId: updateMerchantPreOrderInMinutes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/pos-status\n  method: put\n  operationId: heartbeatStatusChangeTriggered\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/{delivery_area_id}/deliveryfee\n  method: get\n  operationId: getMerchantDeliveryAreaFeeByLegacyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/{delivery_area_id}/deliveryfee\n  method: put\n  operationId: updateMerchantDeliveryAreaFeeByLegacyId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/estimates\n  method: get\n  operationId: getFulfillmentEstimatesByLegacyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/estimates\n  method: put\n  operationId: updateFulfillmentEstimatesByLegacyId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/deliveryboundaries\n  method: get\n  operationId: getDeliveryBoundaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/fulfillment/deliveryboundaries\n  method: put\n  operationId: updateDeliveryBoundaries\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/deliveryminimum\n  method: get\n  operationId: getDeliveryMinimumForMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/deliveryminimum\n  method: put\n  operationId: updateDeliveryMinimumForMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/properties\n  method: put\n  operationId: updateMerchantProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/pos-status\n  method: put\n  operationId: heartbeatStatusChangeTriggeredBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/integrationlive\n  method: put\n  operationId: updatePosMerchantIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v2/merchant/pos-status/{batch_id}/status\n  method: get\n  operationId: getMerchantStatusByOrderTypeBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{partner_id}/idmappings\n  method: get\n  operationId: getIdMappingsByPartnerAndExternalIds\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/fulfillment\n  method: get\n  operationId: getFulfillmentInfoByLegacyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}\n  method: get\n  operationId: getMerchantByLegacyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/properties/{batch_id}/status\n  method: get\n  operationId: getMerchantPropertiesBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/pos-status/{batch_id}/status\n  method: get\n  operationId: getHeartbeatStatusChangeTriggeredBatchStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/integrationlive/{batch_id}/status\n  method: get\n  operationId: getPosMerchantIntegrationBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/config/groups/{group_key}\n  method: get\n  operationId: getMerchantsByGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/repeating\n  method: get\n  operationId: getRepeatingSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/repeating\n  method: put\n  operationId: putRepeatingSchedule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/pickup/{schedule_version}\n  method: put\n  operationId: updatePickupSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/delivery/{schedule_version}\n  method: put\n  operationId: updateDeliverySchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/catering/{schedule_version}\n  method: put\n  operationId: updateCateringSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/overrides\n  method: get\n  operationId: getScheduledOverrides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/overrides\n  method: post\n  operationId: overrideSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/overrides\n  method: delete\n  operationId: deleteScheduleOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/opennow\n  method: post\n  operationId: openNow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/closenow\n  method: post\n  operationId: closeNow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/pickup\n  method: get\n  operationId: getPickupSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/delivery\n  method: get\n  operationId: getDeliverySchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/catering\n\
  \  method: get\n  operationId: getCateringSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/onboarding/v1/triage\n  method: post\n  operationId: triage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/referral\n  method: post\n  operationId: referralSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/partner/deactivate\n  method: post\n  operationId:\
  \ partnerDeactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/partner/activate\n  method: post\n  operationId: partnerActivateMerchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/deactivate\n  method: post\n  operationId: deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/associate\n  method: post\n  operationId: associateMerchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/activate\n  method: post\n  operationId: activateMerchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/onboarding/v1/merchants\n  method: get\n  operationId: getEligibleMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/status\n  method: put\n  operationId: updateExternalOrderStatusByOrderUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/changerequests\n  method: get\n  operationId: getChangeRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/changerequests\n  method: post\n  operationId: changeExternalOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/orders/{order_uuid}/addpickupinstructions\n  method: post\n  operationId: addPickupInstructionsToOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}\n  method: get\n  operationId: getPosOrderByOrderUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders\n\
  \  method: get\n  operationId: getPosOrdersByMerchantStatusDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/group/{group_key}/orders\n  method: get\n  operationId: getPosOrdersByGroupStatusDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/reporting/v1/reports\n  method: post\n  operationId: createExportReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/reporting/v1/reports/{reportUuid}\n  method: get\n  operationId: getDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/reporting/v1/merchants\n  method: get\n  operationId: getEnabledMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/test/transmission\n  method: post\n  operationId: postTestOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/test/jitevent\n  method: post\n  operationId: simulateJitOrderEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/test/delivery\n  method: post\n  operationId: postTestDeliveryRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/agentic-access/grubhub-agentic-access.yml
summary_line: 91 operations · 56 acting · 5 human-in-the-loop
tags:
- Food Delivery
- Restaurant
- Marketplace
- Online Ordering
- Point-of-Sale
- Logistics
- Last Mile Delivery
- Menu Management
- Hospitality
- Local Commerce
---
