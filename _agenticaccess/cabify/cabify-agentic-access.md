---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 26
api_specs:
- filename: cabify-delivery-api-openapi.yml
  format: yaml
  label: Cabify Delivery API
  slug: cabify-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-delivery-api-openapi.yml
- filename: cabify-estimates-api-openapi.yml
  format: yaml
  label: Cabify Estimates API
  slug: cabify-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-estimates-api-openapi.yml
- filename: cabify-hubs-api-openapi.yml
  format: yaml
  label: Cabify Hubs API
  slug: cabify-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-hubs-api-openapi.yml
- filename: cabify-journeys-api-openapi.yml
  format: yaml
  label: Cabify Journeys API
  slug: cabify-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-journeys-api-openapi.yml
- filename: cabify-label-api-openapi.yml
  format: yaml
  label: Cabify Label API
  slug: cabify-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-label-api-openapi.yml
- filename: cabify-labels-api-openapi.yml
  format: yaml
  label: Cabify Labels API
  slug: cabify-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-labels-api-openapi.yml
- filename: cabify-parcels-api-openapi.yml
  format: yaml
  label: Cabify Parcels API
  slug: cabify-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-parcels-api-openapi.yml
- filename: cabify-sales-api-openapi.yml
  format: yaml
  label: Cabify Sales API
  slug: cabify-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-sales-api-openapi.yml
- filename: cabify-shipment-api-openapi.yml
  format: yaml
  label: Cabify Shipment API
  slug: cabify-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-shipment-api-openapi.yml
- filename: cabify-shipping-types-api-openapi.yml
  format: yaml
  label: Cabify Shipping Types API
  slug: cabify-shipping-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-shipping-types-api-openapi.yml
- filename: cabify-status-api-openapi.yml
  format: yaml
  label: Cabify Status API
  slug: cabify-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-status-api-openapi.yml
- filename: cabify-users-api-openapi.yml
  format: yaml
  label: Cabify Users API
  slug: cabify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-users-api-openapi.yml
- filename: cabify-webhooks-api-openapi.yml
  format: yaml
  label: Cabify Webhooks API
  slug: cabify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 26
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cabify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/parcels/ship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/parcels/estimate
operation_count: 46
overview: 'Cabify exposes 46 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 18 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cabify
provider_slug: cabify
slug: cabify-agentic-access
source_filename: cabify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cabify-delivery-api-openapi.yml, openapi/cabify-estimates-api-openapi.yml, openapi/cabify-hubs-api-openapi.yml,\n  openapi/cabify-journeys-api-openapi.yml, openapi/cabify-label-api-openapi.yml, openapi/cabify-labels-api-openapi.yml,\n  openapi/cabify-parcels-api-openapi.yml, openapi/cabify-sales-api-openapi.yml, openapi/cabify-shipment-api-openapi.yml,\n  openapi/cabify-shipping-types-api-openapi.yml, openapi/cabify-status-api-openapi.yml, openapi/cabify-users-api-openapi.yml,\n  openapi/cabify-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 20\n    connected: 26\n  by_consequence:\n    write: 18\n    read: 26\n    physical:\
  \ 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/parcels/deliver/cancel\n  method: post\n  operationId: cancelParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/deliver/pickup\n  method: get\n  operationId: deliverPickup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/estimates\n  method: post\n  operationId: getEstimation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hubs\n  method: get\n  operationId: getV1Hubs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hubs\n  method: post\n  operationId: postV1Hubs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hubs/none/{hub_external_id}\n  method: get\n  operationId: getV1HubsNoneByHubExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hubs/none/{hub_external_id}\n  method: put\n  operationId: putV1HubsNoneByHubExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v4/hub\n  method: get\n  operationId: getHub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/journey/{id}/state\n  method: post\n  operationId: cancelJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/journey/{id}/state\n  method: get\n  operationId: getJourneyState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/journey\n  method: post\n  operationId: createJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/journey/{journey_id}\n  method: get\n  operationId: getJourney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/journey/{id}/keep_searching\n  method: post\n  operationId: keepSearching\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{parcel_id}/warehouse/label\n  method: get\n  operationId: warehouseLabelParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v4/labels\n  method: post\n  operationId: createLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/labels\n  method: get\n  operationId: getLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/labels\n  method: patch\n  operationId: updateLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/labels/{id}\n  method: get\n  operationId: getLabelById\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels\n  method: post\n  operationId: addParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels\n  method: get\n  operationId: getParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}/proof_configuration\n  method: post\n  operationId: createProofConfigurationParcel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{parcel_id}/proof_configuration\n  method: get\n  operationId: proofConfigurationParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/delete\n  method: post\n  operationId: deleteParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{parcel_id}\n  method: get\n  operationId: getParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}\n  method: put\n  operationId: updateParcel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{parcel_id}/tip\n  method: get\n  operationId: getTipParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}/tip\n  method: post\n  operationId: tipParcel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{parcel_id}/label\n  method: get\n  operationId: labelParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}/notify\n  method: post\n  operationId: notifyParcel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/journey/{journey_id}/sales\n  method: get\n  operationId: getJourneySales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/sales\n  method: get\n  operationId: getSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/user/{user_id}/sales\n  method: get\n  operationId: getUserSales\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/parcels/estimate\n  method: post\n  operationId: EstimateShipParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/ship\n  method: post\n  operationId: shipParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipping_types/available\n  method: get\n  operationId: shippingTypesAvailable\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}/status\n  method: get\n  operationId: statusParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/{parcel_id}/timeline\n  method: get\n  operationId: timelineParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/users\n  method: post\n  operationId: createUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/users\n  method: patch\n  operationId: updateUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/users/email/{email}\n  method: get\n  operationId: getUserByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/users/{id}\n  method: get\n  operationId: getUserById\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{hook}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/agentic-access/cabify-agentic-access.yml
summary_line: 46 operations · 20 acting
tags:
- Company
- Transportation
- Ride Hailing
- Mobility
- Logistics
- Delivery
- Last Mile Delivery
- Webhook
- Authentication
---
