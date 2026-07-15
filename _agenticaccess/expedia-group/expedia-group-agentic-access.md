---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 27
api_specs:
- filename: expedia-rapid-openapi-original.yml
  format: yaml
  label: Expedia Rapid API
  slug: rapid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-rapid-openapi-original.yml
- filename: expedia-fraud-protection-openapi-original.yml
  format: yaml
  label: Expedia Fraud Protection API
  slug: fraud-protection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-fraud-protection-openapi-original.yml
- filename: expedia-lodging-product-openapi-original.yml
  format: yaml
  label: Expedia Lodging API
  slug: lodging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-lodging-product-openapi-original.yml
- filename: expedia-deposit-openapi-original.yml
  format: yaml
  label: Expedia EPS Deposit API
  slug: deposit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-deposit-openapi-original.yml
- filename: expedia-loyalty-openapi-original.yml
  format: yaml
  label: Expedia Loyalty Earn API
  slug: loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-loyalty-openapi-original.yml
consequence_counts:
  physical: 7
  read: 27
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Expedia Group Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /itineraries/{itinerary_id}/payment-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /itineraries/{itinerary_id}/rooms/{room_id}/pricing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/purchase/screen
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/purchase/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /properties/{propertyId}/depositPolicy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /properties/{propertyId}/depositPolicy
operation_count: 49
overview: 'Expedia Group exposes 49 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 15 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Expedia Group
provider_slug: expedia-group
slug: expedia-group-agentic-access
source_filename: expedia-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/expedia-deposit-openapi-original.yml, openapi/expedia-fraud-protection-openapi-original.yml,\n  openapi/expedia-lodging-product-openapi-original.yml, openapi/expedia-loyalty-openapi-original.yml,\n  openapi/expedia-rapid-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 27\n    acting: 22\n  by_consequence:\n    read: 27\n    physical: 7\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /properties/{propertyId}/depositPolicy\n  method: get\n  operationId: getDepositPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /properties/{propertyId}/depositPolicy\n  method: put\n  operationId: setDepositPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/depositPolicy\n  method: delete\n  operationId: deleteDepositPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/purchase/screen\n  method: post\n  operationId: screen\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - fraudandrisk.fraud.order-purchase-screen\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/purchase/update\n  method: post\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - fraudandrisk.fraud.order-purchase-update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/properties\n  method: get\n  operationId: getProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /products/properties/{propertyId}\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes\n  method: get\n  operationId: getRoomTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes\n  method: post\n  operationId: createRoomType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}\n  method: get\n  operationId: getRoomType\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}\n  method: put\n  operationId: updateRoomType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}\n  method: patch\n  operationId: patchRoomType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/amenities\n  method: get\n  operationId: getRoomTypeAmenities\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/amenities\n  method: put\n  operationId: setRoomTypeAmenities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans\n  method: get\n  operationId: getRatePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans\n  method: post\n  operationId: createRatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans/{ratePlanId}\n  method: get\n  operationId: getRatePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans/{ratePlanId}\n  method: put\n  operationId: updateRatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans/{ratePlanId}\n  method: delete\n  operationId: deleteRatePlan\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/ratePlans/{ratePlanId}\n  method: patch\n  operationId: patchRatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/roomTypes/{roomTypeId}/rateThresholds\n  method: get\n  operationId: getRateVerificationThresholds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/earn/transactions\n  method: get\n  operationId: loyaltyTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/earn/last_update\n  method: get\n  operationId: loyaltyLastUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/content\n  method: get\n  operationId: getPropertyContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/inactive\n  method: get\n  operationId: getInactiveProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property_id}/guest-reviews\n  method: get\n  operationId: getPropertyGuestReviews\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/properties/catalog\n  method: get\n  operationId: getPropertyCatalogFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/properties/content\n  method: get\n  operationId: getPropertyContentFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions\n  method: get\n  operationId: getRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{region_id}\n  method: get\n  operationId: getRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/geography\n\
  \  method: post\n  operationId: postGeography\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/availability\n  method: get\n  operationId: getAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property_id}/availability\n  method: get\n  operationId: getAdditionalAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property_id}/rooms/{room_id}/rates/{rate_id}\n  method: get\n  operationId: priceCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property_id}/payment-options\n  method: get\n  operationId: getPaymentOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/availability\n  method: get\n  operationId: getCalendarAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-sessions\n  method: post\n  operationId: postPaymentSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries\n  method: get\n  operationId: getReservation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /itineraries\n  method: post\n  operationId: postItinerary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}\n  method: get\n  operationId: getReservationByItineraryId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /itineraries/{itinerary_id}\n  method: put\n  operationId: putResumeBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}\n  method: delete\n  operationId: deleteHeldBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}/payment-sessions\n  method: put\n  operationId: putCompletePaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}/rooms/{room_id}\n  method: put\n  operationId: changeRoomDetails\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}/rooms/{room_id}\n  method: delete\n  operationId: deleteRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /itineraries/{itinerary_id}/rooms/{room_id}/pricing\n  method: put\n  operationId: commitChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chains\n  method: get\n  operationId: getChainReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  operationId: requestUndeliveredNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: post\n  operationId: requestTestNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/agentic-access/expedia-group-agentic-access.yml
summary_line: 49 operations · 22 acting
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
---
