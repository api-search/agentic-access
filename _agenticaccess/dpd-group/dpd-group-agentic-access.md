---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: dpd-group-countries-api-openapi.yml
  format: yaml
  label: DPD Geo Countries API
  slug: geoapi-countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-countries-api-openapi.yml
- filename: dpd-group-customers-api-openapi.yml
  format: yaml
  label: DPD Geo Customers API
  slug: geoapi-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-customers-api-openapi.yml
- filename: dpd-group-me-api-openapi.yml
  format: yaml
  label: DPD Geo Me API
  slug: geoapi-me
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-me-api-openapi.yml
- filename: dpd-group-parcels-api-openapi.yml
  format: yaml
  label: DPD Geo Parcels API
  slug: geoapi-parcels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-parcels-api-openapi.yml
- filename: dpd-group-pickup-orders-api-openapi.yml
  format: yaml
  label: DPD Geo Pickup Orders API
  slug: geoapi-pickup-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-pickup-orders-api-openapi.yml
- filename: dpd-group-shipments-api-openapi.yml
  format: yaml
  label: DPD Geo Shipments API
  slug: geoapi-shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipments-api-openapi.yml
- filename: dpd-group-shipping-services-api-openapi.yml
  format: yaml
  label: DPD Geo Shipping Services API
  slug: geoapi-shipping-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-services-api-openapi.yml
- filename: dpd-group-shipping-api-openapi.yml
  format: yaml
  label: DPD META-API Shipment
  slug: meta-api-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-api-openapi.yml
consequence_counts:
  physical: 11
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dpd Group Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pickup-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pickup-orders/{pickupOrderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v1/colreq
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v1/label
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v1/login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v1/pickupscheduling
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v1/shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v2/colreq
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v2/pickupscheduling
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/v2/shipment
operation_count: 23
overview: 'DPD Group exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 2 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DPD Group
provider_slug: dpd-group
slug: dpd-group-agentic-access
source_filename: dpd-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/dpd-group-countries-api-openapi.yml, openapi/dpd-group-customers-api-openapi.yml,\n  openapi/dpd-group-me-api-openapi.yml, openapi/dpd-group-parcels-api-openapi.yml, openapi/dpd-group-pickup-orders-api-openapi.yml,\n  openapi/dpd-group-shipments-api-openapi.yml, openapi/dpd-group-shipping-api-openapi.yml, openapi/dpd-group-shipping-services-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 10\n    acting: 13\n  by_consequence:\n    read: 10\n    write: 2\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerDSW}/addresses\n  method: get\n  operationId: getCustomersByCustomerDSWAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels\n  method: get\n  operationId: getParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels/labels\n  method:\
  \ post\n  operationId: postParcelsLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parcels/{parcelIdent}/labels\n  method: post\n  operationId: postParcelsByParcelIdentLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parcels/tracking\n  method: post\n  operationId: postParcelsTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels/{parcelIdent}/tracking\n  method: get\n  operationId: getParcelsByParcelIdentTracking\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels/{parcelIdent}/drop-off-codes\n  method: post\n  operationId: postParcelsByParcelIdentDropOffCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickup-orders\n  method: post\n  operationId: postPickupOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickup-orders/{pickupOrderId}\n  method: delete\n  operationId: deletePickupOrdersByPickupOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickup-orders/{pickupOrderId}\n  method: get\n  operationId: getPickupOrdersByPickupOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: post\n  operationId: postShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v2/shipment\n  method: post\n  operationId: shippingV2ShipmentPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v2/pickupscheduling\n  method: post\n  operationId: shippingV2PickupschedulingPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v2/colreq\n  method: post\n  operationId: shippingV2ColreqPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v1/shipment\n  method: post\n  operationId: shippingV1ShipmentPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v1/pickupscheduling\n  method: post\n  operationId: shippingV1PickupschedulingPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /shipping/v1/login\n  method: post\n  operationId: shippingV1LoginPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v1/label\n  method: post\n  operationId: shippingV1LabelPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/v1/colreq\n  method: post\n  operationId: shippingV1ColreqPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping-services\n  method: get\n  operationId: getShippingServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/agentic-access/dpd-group-agentic-access.yml
summary_line: 23 operations · 13 acting
tags:
- Logistics
- Parcel
- Shipping
- Tracking
- Carrier
---
