---
acting_count: 65
action_class_counts:
  acting: 65
  connected: 40
api_specs:
- filename: getcircuit-com-couriers-api-openapi.yml
  format: yaml
  label: Circuit Couriers API
  slug: getcircuit-com-couriers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-couriers-api-openapi.yml
- filename: getcircuit-com-depots-api-openapi.yml
  format: yaml
  label: Circuit Depots API
  slug: getcircuit-com-depots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-depots-api-openapi.yml
- filename: getcircuit-com-drivers-api-openapi.yml
  format: yaml
  label: Circuit Drivers API
  slug: getcircuit-com-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-drivers-api-openapi.yml
- filename: getcircuit-com-live-plans-api-openapi.yml
  format: yaml
  label: Circuit Live Plans API
  slug: getcircuit-com-live-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-live-plans-api-openapi.yml
- filename: getcircuit-com-live-stops-api-openapi.yml
  format: yaml
  label: Circuit Live Stops API
  slug: getcircuit-com-live-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-live-stops-api-openapi.yml
- filename: getcircuit-com-members-api-openapi.yml
  format: yaml
  label: Circuit Members API
  slug: getcircuit-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-members-api-openapi.yml
- filename: getcircuit-com-operations-api-openapi.yml
  format: yaml
  label: Circuit Operations API
  slug: getcircuit-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-operations-api-openapi.yml
- filename: getcircuit-com-orders-api-openapi.yml
  format: yaml
  label: Circuit Orders API
  slug: getcircuit-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-orders-api-openapi.yml
- filename: getcircuit-com-pickup-locations-api-openapi.yml
  format: yaml
  label: Circuit Pickup Locations API
  slug: getcircuit-com-pickup-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-pickup-locations-api-openapi.yml
- filename: getcircuit-com-plans-api-openapi.yml
  format: yaml
  label: Circuit Plans API
  slug: getcircuit-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-plans-api-openapi.yml
- filename: getcircuit-com-routes-api-openapi.yml
  format: yaml
  label: Circuit Routes API
  slug: getcircuit-com-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-routes-api-openapi.yml
- filename: getcircuit-com-stops-api-openapi.yml
  format: yaml
  label: Circuit Stops API
  slug: getcircuit-com-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-stops-api-openapi.yml
- filename: getcircuit-com-team-api-openapi.yml
  format: yaml
  label: Circuit Team API
  slug: getcircuit-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-team-api-openapi.yml
- filename: getcircuit-com-unassigned-stops-api-openapi.yml
  format: yaml
  label: Circuit Unassigned Stops API
  slug: getcircuit-com-unassigned-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-unassigned-stops-api-openapi.yml
consequence_counts:
  physical: 6
  read: 40
  safety-critical: 24
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 24
kind: agentic-access
layout: agentic-access
method: generated
name: Getcircuit Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /plans/{planId}/stops/{stopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /plans/{planId}/stops/{stopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /plans/{planId}/stops/{stopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /plans/{planId}/stops/{stopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops/{stopId}:liveDelete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops/{stopId}:liveDelete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops/{stopId}:liveUpdate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops/{stopId}:liveUpdate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:import
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:import
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:liveCreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:liveCreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:liveImport
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /plans/{planId}/stops:liveImport
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /unassignedStops
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /unassignedStops
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /unassignedStops/{unassignedStopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /unassignedStops/{unassignedStopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /unassignedStops/{unassignedStopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /unassignedStops/{unassignedStopId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /unassignedStops:import
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /unassignedStops:import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 105
overview: 'Circuit exposes 105 API operations that an AI agent could call, of which 65 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 35 write, 6 physical, and 24 safety-critical.


  24 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Circuit
provider_slug: getcircuit-com
slug: getcircuit-com-agentic-access
source_filename: getcircuit-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/openapi-connect-v1.json, openapi/openapi-v0.2b.json, openapi/openapi-v1.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 105\n  by_action_class:\n    connected: 40\n    acting: 65\n  by_consequence:\n    read: 40\n    physical: 6\n    write: 35\n    safety-critical: 24\n  human_in_the_loop_required: 24\noperations:\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders:import\n  method: post\n  operationId: importOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders:submit\n  method: post\n  operationId: submitOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /orders:withdraw\n  method: post\n  operationId: withdrawOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /orders/{id}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/shippingLabels\n  method: get\n  operationId: getOrderShippingLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /couriers\n  method: get\n  operationId: listCouriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /couriers/{id}\n  method: get\n  operationId: getCourier\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickupLocations\n  method: get\n  operationId: listPickupLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickupLocations/{id}\n  method: get\n  operationId: getPickupLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}\n  method: patch\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:optimize\n\
  \  method: post\n  operationId: optimizePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:distribute\n  method: post\n  operationId: distributePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:reoptimize\n  method: post\n  operationId: reoptimizePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /plans/{planId}:redistribute\n  method: post\n  operationId: redistributePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:save\n  method: post\n  operationId: savePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}/stops\n  method: post\n  operationId: createStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops\n  method: get\n  operationId: listStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}/stops:import\n  method: post\n  operationId: importStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}\n  method: patch\n  operationId: updateStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n \
  \     exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}\n  method: get\n  operationId: getStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}/stops/{stopId}\n  method: delete\n  operationId: deleteStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops:liveCreate\n  method: post\n  operationId: createLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}:liveUpdate\n  method: post\n  operationId: updateLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops:liveImport\n  method: post\n  operationId: importLiveStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /plans/{planId}/stops/{stopId}:liveDelete\n  method: post\n  operationId: deleteLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /drivers\n  method: get\n  operationId: listDrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drivers\n  method: post\n  operationId: createDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers/{driverId}\n  method: get\n  operationId:\
  \ getDriver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drivers/{driverId}\n  method: delete\n  operationId: deleteDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers/{driverId}\n  method: patch\n  operationId: updateDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers:import\n  method: post\n  operationId: importDrivers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots\n  method: get\n  operationId: listDepots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depots/{depotId}\n  method: get\n  operationId: getDepot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{routeId}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/{operationId}:cancel\n  method: post\n  operationId: cancelOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operations/{operationId}\n  method: get\n  operationId: getOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations\n  method: get\n  operationId: listOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops/{unassignedStopId}\n  method: get\n  operationId: getUnassignedStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops/{unassignedStopId}\n  method: delete\n  operationId: deleteUnassignedStop\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops/{unassignedStopId}\n  method: patch\n  operationId: updateUnassignedStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops\n  method: get\n  operationId: listUnassignedStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops\n  method: post\n  operationId: createUnassignedStop\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops:import\n  method: post\n  operationId: importUnassignedStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /team/customStopProperties\n  method: get\n  operationId: listCustomStopProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/customStopProperties/{customStopPropertyId}\n\
  \  method: get\n  operationId: getCustomStopProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}\n  method: patch\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:optimize\n  method: post\n  operationId: optimizePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:distribute\n\
  \  method: post\n  operationId: distributePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:reoptimize\n  method: post\n  operationId: reoptimizePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}:redistribute\n  method: post\n  operationId: redistributePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /plans/{planId}:save\n  method: post\n  operationId: savePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}/stops\n  method: post\n  operationId: createStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops\n  method: get\n  operationId: listPlanStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /plans/{planId}/stops:import\n  method: post\n  operationId: importStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}\n  method: patch\n  operationId: updateStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}\n  method: get\n  operationId: getStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /plans/{planId}/stops/{stopId}\n  method: delete\n  operationId: deleteStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops:liveCreate\n  method: post\n  operationId: createLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}:liveUpdate\n  method: post\n  operationId: updateLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops:liveImport\n  method: post\n  operationId: importLiveStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans/{planId}/stops/{stopId}:liveDelete\n  method: post\n  operationId: deleteLiveStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n     \
  \ human-in-the-loop: required\n    audit: required\n- path: /drivers\n  method: get\n  operationId: listDrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drivers\n  method: post\n  operationId: createDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers/{driverId}\n  method: get\n  operationId: getDriver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drivers/{driverId}\n  method: delete\n  operationId: deleteDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers/{driverId}\n  method: patch\n  operationId: updateDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drivers:import\n  method: post\n  operationId: importDrivers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots\n  method: post\n  operationId: createDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots\n  method: get\n  operationId: listDepots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depots/{depotId}\n  method: get\n  operationId: getDepot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depots/{depotId}\n  method: delete\n  operationId: deleteDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots/{depotId}\n\
  \  method: patch\n  operationId: updateDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots:import\n  method: post\n  operationId: importDepots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depots/{depotId}:setMain\n  method: post\n  operationId: setMainDepot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /routes/{routeId}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{routeId}/stops\n  method: get\n  operationId: listRouteStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/{operationId}:cancel\n  method: post\n  operationId: cancelOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /operations/{operationId}\n  method: get\n  operationId: getOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations\n  method: get\n  operationId: listOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops/{unassignedStopId}\n  method: get\n  operationId: getUnassignedStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops/{unassignedStopId}\n  method: delete\n  operationId: deleteUnassignedStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops/{unassignedStopId}\n  method: patch\n  operationId: updateUnassignedStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops\n  method: get\n  operationId: listUnassignedStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unassignedStops\n  method: post\n  operationId: createUnassignedStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unassignedStops:import\n  method: post\n  operationId: importUnassignedStops\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /team/customStopProperties\n  method: get\n  operationId: listCustomStopProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/customStopProperties/{customStopPropertyId}\n  method: get\n  operationId: getCustomStopProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /members\n  method: post\n  operationId: createMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}\n  method: patch\n  operationId: updateMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}\n  method: delete\n  operationId: deleteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members:import\n  method: post\n  operationId: importMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stops:search\n  method: get\n  operationId: searchStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/getcircuit-com/agentic-access/getcircuit-com-agentic-access.yml
summary_line: 105 operations · 65 acting · 24 human-in-the-loop
tags:
- Company
- Logistics
- Delivery
- Platform
---
