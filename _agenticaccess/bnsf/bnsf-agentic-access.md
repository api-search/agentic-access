---
acting_count: 0
action_class_counts:
  connected: 59
api_specs:
- filename: bnsf-trace-openapi.yml
  format: yaml
  label: BNSF Tracing API
  slug: bnsf-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-trace-openapi.yml
- filename: bnsf-intermodal-hub-operations-openapi.yml
  format: yaml
  label: BNSF Intermodal Hub Operations API
  slug: bnsf-hub-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-intermodal-hub-operations-openapi.yml
- filename: bnsf-automotive-hub-operations-openapi.yml
  format: yaml
  label: BNSF Automotive Hub Operations API
  slug: bnsf-automotive-hub-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-automotive-hub-operations-openapi.yml
- filename: bnsf-prices-openapi.yml
  format: yaml
  label: BNSF Prices and Rates API
  slug: bnsf-pricing-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-prices-openapi.yml
- filename: bnsf-schedules-openapi.yml
  format: yaml
  label: BNSF Schedules API
  slug: bnsf-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-schedules-openapi.yml
- filename: bnsf-waybill-openapi.yml
  format: yaml
  label: BNSF Waybill Management API
  slug: bnsf-waybill-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-waybill-openapi.yml
- filename: bnsf-reference-files-openapi.yml
  format: yaml
  label: BNSF Reference Files API
  slug: bnsf-reference-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-reference-files-openapi.yml
- filename: bnsf-diagnostics-openapi.yml
  format: yaml
  label: BNSF Diagnostics API
  slug: bnsf-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/openapi/bnsf-diagnostics-openapi.yml
consequence_counts:
  delete: 3
  read: 23
  write: 33
description: 'Recommended x-agentic-access execution contracts for the BNSF Customer API, classified from the published contracts. subject: required marks the 27 Restricted Services, which BNSF gates on a separately authorised certificate. human-in-the-loop: required marks the writes with no published reversal and no idempotency key — an agent that fires one of these cannot undo it and cannot safely retry it. A governance starting point; review and bind audience per deployment.'
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Bnsf Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 59
overview: 'BNSF exposes 59 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 33 write.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BNSF
provider_slug: bnsf
slug: bnsf-agentic-access
source_filename: bnsf-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: generated\nsource: the eight BNSF OpenAPI documents in openapi/, harvested 2026-09-06\ndescription: 'Recommended x-agentic-access execution contracts for the BNSF Customer API, classified from the published\n  contracts. subject: required marks the 27 Restricted Services, which BNSF gates on a separately authorised certificate.\n  human-in-the-loop: required marks the writes with no published reversal and no idempotency key — an agent that\n  fires one of these cannot undo it and cannot safely retry it. A governance starting point; review and bind audience\n  per deployment.'\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 59\n  by_consequence:\n    write: 33\n    read: 23\n    delete: 3\n  human_in_the_loop_required: 8\n  restricted_subject_required: 27\noperations:\n- path: /v1/pregate/automotive/haulaway-entry\n  method: post\n  operationId: postV1PregateAutomotiveHaulawayEntry\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/vehicles/addHold\n  method: post\n  operationId: postV1VehiclesAddhold\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: true\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/vehicles/releaseHold\n  method: post\n  operationId: postV1VehiclesReleasehold\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/gate-pass/ramp/{aarRampCode}/vehicle/{vin}\n  method: get\n  operationId: getV1GatePassRampByAarRampCodeVehicleByVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop:\
  \ not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gate-pass/ramp/{aarRampCode}/gate-pass/{gatePassCode}\n  method: get\n  operationId: getV1GatePassRampByAarRampCodeGatePassByGatePassCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exit-request\n  method: post\n  operationId: postV1ExitRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pre-outgate\n  method: post\n  operationId: postV1PreOutgate\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /healthcheck\n\
  \  method: get\n  operationId: getHealthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytic-event\n  method: post\n  operationId: postV1AnalyticEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/dray-booking/open\n  method: get\n  operationId: getV1DrayBookingOpen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dray-plan/list-units\n  method: post\n  operationId: postV1DrayPlanListUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject:\
  \ required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/dray-plan/initial/{equipmentInitial}/number/{equipmentNumber}\n  method: delete\n  operationId: deleteV1DrayPlanInitialByEquipmentInitialNumberByEquipmentNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: delete\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/dray-plan/units\n  method: get\n  operationId: getV1DrayPlanUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dray-plan/units\n  method: post\n  operationId: postV1DrayPlanUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: true\n    human-in-the-loop:\
  \ not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v2/dvir\n  method: post\n  operationId: postV2Dvir\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/flips\n  method: post\n  operationId: postV1Flips\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/hub\n  method: get\n  operationId: getV1Hub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ingate\n  method: post\n  operationId: postV2Ingate\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n\
  \    subject: required\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/ingate-management/current\n  method: get\n  operationId: getV1IngateManagementCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ingate/validate\n  method: post\n  operationId: postV2IngateValidate\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/j1-receipts\n  method: post\n  operationId: postV1J1Receipts\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n\
  - path: /v2/outgate\n  method: post\n  operationId: postV2Outgate\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v2/outgate/validate\n  method: post\n  operationId: postV2OutgateValidate\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pickup-number\n  method: post\n  operationId: postV1PickupNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pregate/in\n  method: post\n  operationId: postV1PregateIn\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject:\
  \ required\n    reversible: true\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pregate/in\n  method: delete\n  operationId: deleteV1PregateIn\n  x-agentic-access:\n    action-class: connected\n    consequence: delete\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pregate/out\n  method: post\n  operationId: postV1PregateOut\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: true\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/pregate/out\n  method: delete\n  operationId: deleteV1PregateOut\n  x-agentic-access:\n    action-class: connected\n    consequence: delete\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v2/street-en-route\n\
  \  method: post\n  operationId: postV2StreetEnRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v3/unit-details\n  method: post\n  operationId: postV3UnitDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v3/unit-details/domestic-empties\n  method: get\n  operationId: getV3UnitDetailsDomesticEmpties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/update-parking\n  method: post\n  operationId: postV1UpdateParking\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ write\n    subject: required\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/carload-rates\n  method: post\n  operationId: postV1CarloadRates\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/intermodal-rates\n  method: post\n  operationId: postV1IntermodalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/invoices\n  method: post\n  operationId: postV1Invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/rail-miles\n\
  \  method: post\n  operationId: postV1RailMiles\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/event-codes\n  method: get\n  operationId: getV1EventCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stations\n  method: get\n  operationId: getV1Stations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stcc\n  method: get\n  operationId: getV1Stcc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop:\
  \ not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stcc/hazardous\n  method: get\n  operationId: getV1StccHazardous\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/umler\n  method: post\n  operationId: postV1Umler\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/intermodal-schedules\n  method: get\n  operationId: getV1IntermodalSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trip-plan-automotive\n  method: get\n  operationId: getV1TripPlanAutomotive\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vins\n  method: post\n  operationId: postV1Vins\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/vin-details\n  method: get\n  operationId: getV1VinDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vin-inspections\n  method: get\n  operationId: getV1VinInspections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/cars\n  method: get\n  operationId: getV1Cars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cars\n  method: post\n  operationId: postV1Cars\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/carload-consist\n  method: get\n  operationId: getV1CarloadConsist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trip-plan-carload\n  method: get\n  operationId: getV1TripPlanCarload\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trip-plan-intermodal\n  method: get\n  operationId: getV1TripPlanIntermodal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/units\n  method: get\n  operationId: getV1Units\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/units\n  method: post\n  operationId: postV1Units\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/trains\n  method:\
  \ get\n  operationId: getV1Trains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ag-trains\n  method: post\n  operationId: postV1AgTrains\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/coal-trains\n  method: post\n  operationId: postV1CoalTrains\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/ip-trains\n  method: post\n  operationId: postV1IpTrains\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    reversible: false\n    human-in-the-loop:\
  \ not-required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/bol\n  method: post\n  operationId: postV1Bol\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    reversible: false\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n- path: /v1/waybill\n  method: get\n  operationId: getV1Waybill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    reversible: false\n    human-in-the-loop: not-required\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/agentic-access/bnsf-agentic-access.yml
summary_line: 59 operations · 8 human-in-the-loop
tags:
- Freight
- Railroad
- Shipping
- Trains
- Intermodal
- Logistics
- Supply Chain
- Transportation
---
