---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 17
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: merchant-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: merchant-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
consequence_counts:
  physical: 3
  read: 17
  safety-critical: 3
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Grubhub Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/external
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
  path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/delivery/proxy-phone
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/status
operation_count: 35
overview: 'grubhub exposes 35 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 12 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: grubhub
provider_slug: grubhub
slug: grubhub-agentic-access
source_filename: grubhub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/grubhub-deliveries-openapi.yml, openapi/grubhub-menu-openapi.yml, openapi/grubhub-merchant-data-openapi.yml,\n  openapi/grubhub-merchant-schedules-openapi.yml, openapi/grubhub-onboarding-openapi.yml, openapi/grubhub-orders-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 17\n    acting: 18\n  by_consequence:\n    read: 17\n    physical: 3\n    write: 12\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/delivery\n  method: get\n  operationId: getDeliveryStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/delivery/proxy-phone\n  method: post\n  operationId: createProxyCourierPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/menu/ingestion\n  method: post\n  operationId: ingestMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/menu/ingestion/jobs/{job_id}\n  method: get\n  operationId: getMenuIngestionStatus\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/ingestion/menu\n  method: get\n  operationId: getMerchantMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/external\n  method: put\n  operationId: updateMenuScheduleOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/menu/schedules/overrides/{job_id}/status\n  method: get\n  operationId: getMenuScheduleOverrideStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchants\n  method: get\n  operationId: listMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}\n  method: get\n  operationId: getMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/fulfillment\n  method: get\n  operationId: getMerchantFulfillment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchants/status\n  method: put\n  operationId: updateMerchantStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchants/status/{batch_id}\n  method: get\n  operationId: getMerchantStatusBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchants/properties\n  method: put\n  operationId: updateMerchantProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchants/properties/{batch_id}\n  method: get\n  operationId: getMerchantPropertiesBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/delivery\n  method: get\n  operationId: getDeliverySchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/delivery\n  method: put\n  operationId: updateDeliverySchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/pickup\n  method: get\n  operationId: getPickupSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/pickup\n  method:\
  \ put\n  operationId: updatePickupSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/catering\n  method: get\n  operationId: getCateringSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_id}/schedules/catering\n  method: put\n  operationId: updateCateringSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/overrides\n\
  \  method: post\n  operationId: createScheduleOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/merchant/{merchant_id}/schedules/overrides\n  method: delete\n  operationId: cancelScheduleOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pos/v1/onboarding/referral\n  method: post\n  operationId: createMerchantReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/onboarding/activate\n  method: post\n  operationId: activateMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/onboarding/deactivate\n  method: post\n  operationId: deactivateMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/onboarding/deactivate/partner\n  method: post\n  operationId: deactivateMerchantPartner\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/onboarding/associate\n  method: post\n  operationId: associateMerchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/onboarding/eligibility/{merchant_id}\n  method: get\n  operationId: getMerchantEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/onboarding/issue\n  method: post\n  operationId: reportOnboardingIssue\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders\n  method: get\n  operationId: listMerchantOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/orders/poll\n  method: get\n  operationId: pollOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/confirm\n\
  \  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/status\n  method: put\n  operationId: updateOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/v1/merchant/{merchant_long_id}/orders/{order_uuid}/changerequests\n  method: get\n  operationId: getOrderChangeRequests\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/agentic-access/grubhub-agentic-access.yml
summary_line: 35 operations · 18 acting · 3 human-in-the-loop
tags: []
---
