---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 17
api_specs:
- filename: parcelone-closing-api-openapi.yml
  format: yaml
  label: ParcelOne Closing API
  slug: parcelone-closing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-closing-api-openapi.yml
- filename: parcelone-customer-api-openapi.yml
  format: yaml
  label: ParcelOne Customer API
  slug: parcelone-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customer-api-openapi.yml
- filename: parcelone-customs-api-openapi.yml
  format: yaml
  label: ParcelOne Customs API
  slug: parcelone-customs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customs-api-openapi.yml
- filename: parcelone-datetime-api-openapi.yml
  format: yaml
  label: ParcelOne Datetime API
  slug: parcelone-datetime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-datetime-api-openapi.yml
- filename: parcelone-mandator-api-openapi.yml
  format: yaml
  label: ParcelOne Mandator API
  slug: parcelone-mandator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mandator-api-openapi.yml
- filename: parcelone-mobilereturn-api-openapi.yml
  format: yaml
  label: ParcelOne Mobilereturn API
  slug: parcelone-mobilereturn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mobilereturn-api-openapi.yml
- filename: parcelone-profile-api-openapi.yml
  format: yaml
  label: ParcelOne Profile API
  slug: parcelone-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-profile-api-openapi.yml
- filename: parcelone-shipment-api-openapi.yml
  format: yaml
  label: ParcelOne Shipment API
  slug: parcelone-shipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-shipment-api-openapi.yml
consequence_counts:
  physical: 3
  read: 17
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parcelone Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /closing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shipment/{ShipmentRefField}/{ShipmentRefValue}
operation_count: 21
overview: 'ParcelOne exposes 21 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 1 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ParcelOne
provider_slug: parcelone
slug: parcelone-agentic-access
source_filename: parcelone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/parcelone-shipping-openapi.json, openapi/parcelone-tracklmc-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 17\n    acting: 4\n  by_consequence:\n    read: 17\n    physical: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /closing/closable/{mandator}/{consigner}/{cep}/{startdate}/{enddate}\n  method: get\n  operationId: getClosable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /closing/stamps/{mandator}/{consigner}/{cep}/{startdate}/{enddate}\n  method: get\n  operationId: getClosedStamps\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /closing/reprint/{closedStamp}\n  method: get\n  operationId: reprintClosingList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /closing\n  method: post\n  operationId: closeShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n  method: get\n  operationId: getCustomerStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customs/reprint/{ShipmentRefField}/{ShipmentRefValue}\n\
  \  method: get\n  operationId: reprintCustomsDocumentsForShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customs/reprint/{ShipmentRefField}/{ShipmentRefValue}/{PackageRefField}/{PackageRefValue}\n  method: get\n  operationId: reprintCustomsDocumentsShipmentPackageID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customs\n  method: post\n  operationId: registerCustomsData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datetime\n  method: get\n  operationId: getDateTime\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mandator\n  method: get\n  operationId: getmandatorStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobilereturn/{SearchCriteria}/{SearchValue}\n  method: get\n  operationId: getMobileReturnStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getAllCustomerProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{mandator}\n  method: get\n  operationId: getCEPSbyMandator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{mandator}/{cep}\n\
  \  method: get\n  operationId: getProductsbyMandatorandCep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{mandator}/{cep}/{product}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/{ShipmentRefField}/{ShipmentRefValue}\n  method: get\n  operationId: getShipmentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/{ShipmentRefField}/{ShipmentRefValue}\n  method: delete\n  operationId: cancelShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment/label/{ShipmentRefField}/{ShipmentRefValue}\n  method: get\n  operationId: reprintShipmentLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/document/{ShipmentRefField}/{ShipmentRefValue}\n  method: get\n  operationId: reprintShipmentDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment\n  method: post\n  operationId: registerShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /shipment/{trackno}\n  method: get\n  operationId: getTrackings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/parcelone/agentic-access/parcelone-agentic-access.yml
summary_line: 21 operations · 4 acting
tags:
- Logistics
- Shipping
- E-Commerce
- Fulfillment
- International
---
