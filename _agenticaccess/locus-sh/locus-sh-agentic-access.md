---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 14
api_specs:
- filename: locus-oms-openapi.yml
  format: yaml
  label: Locus Order Management API
  slug: locus-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-oms-openapi.yml
- filename: locus-entities-openapi.yml
  format: yaml
  label: Locus Entity Management API
  slug: locus-entity-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-entities-openapi.yml
- filename: locus-platform-openapi.yml
  format: yaml
  label: Locus Platform Entities API
  slug: locus-platform-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/openapi/locus-platform-openapi.yml
consequence_counts:
  physical: 8
  read: 14
  safety-critical: 10
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Locus Sh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/lineitem/{lineItemId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/location/{locationId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/rider-persona/{riderPersonaId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/rider/{riderId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/roster/{rosterId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/service-type/{serviceTypeId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/shift-manager/{tagId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/transporter/{transporterId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/vehicle-model/{vehicleModelId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /client/{clientId}/vehicle/{vehicleId}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client/{clientId}/get-slots
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}/park
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client/{clientId}/order/{orderId}/reschedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client/{clientId}/order/{orderId}/verify-inventory
operation_count: 48
overview: 'Locus exposes 48 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 16 write, 8 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Locus
provider_slug: locus-sh
slug: locus-sh-agentic-access
source_filename: locus-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/locus-entities-openapi.yml, openapi/locus-oms-openapi.yml, openapi/locus-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 14\n    acting: 34\n  by_consequence:\n    read: 14\n    write: 16\n    safety-critical: 10\n    physical: 8\n  human_in_the_loop_required: 10\noperations:\n- path: /client/{clientId}/location/{locationId}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/location/{locationId}\n  method: put\n  operationId: createLocation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/location/{locationId}/disable\n  method: post\n  operationId: disableLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/lineitem/{lineItemId}\n  method: get\n  operationId: getLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/lineitem/{lineItemId}\n  method: put\n  operationId: createLineItem\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/lineitem/{lineItemId}/disable\n  method: post\n  operationId: disableLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/transporter/{transporterId}\n  method: get\n  operationId: getTransporter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/transporter/{transporterId}\n\
  \  method: put\n  operationId: createTransporter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/transporter/{transporterId}/disable\n  method: post\n  operationId: disableTransporter\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/rider/{riderId}\n  method: get\n  operationId: getRider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/rider/{riderId}\n\
  \  method: put\n  operationId: createRider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/rider/{riderId}/disable\n  method: post\n  operationId: disableRider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/vehicle/{vehicleId}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/vehicle/{vehicleId}\n\
  \  method: put\n  operationId: createVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/vehicle/{vehicleId}/disable\n  method: post\n  operationId: disableVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/vehicle-model/{vehicleModelId}\n  method: get\n  operationId: getVehicleModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /client/{clientId}/vehicle-model/{vehicleModelId}\n  method: put\n  operationId: createVehicleModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/vehicle-model/{vehicleModelId}/disable\n  method: post\n  operationId: disableVehicleModel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/rider-persona/{riderPersonaId}\n  method: get\n  operationId: getRiderPersona\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/rider-persona/{riderPersonaId}\n  method: put\n  operationId: createRiderPersona\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/rider-persona/{riderPersonaId}/disable\n  method: post\n  operationId: disableRiderPersona\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/roster/{rosterId}\n  method: get\n  operationId: getRoster\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/rosters-auto-create\n  method: post\n  operationId: createRostersApiRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/roster/{rosterId}/disable\n  method: post\n  operationId: disableRoster\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/homebase-master/{homebaseId}\n  method: get\n  operationId: getHomebase\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/homebase-master/{homebaseId}\n  method: put\n  operationId: createHomebase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/homebase-master/{homebaseId}/status\n  method: post\n  operationId: updateHomebaseStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/shift-manager/{tagId}\n  method: get\n  operationId:\
  \ getShiftTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/shift-manager/{tagId}\n  method: put\n  operationId: createShiftTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/shift-manager/{tagId}/disable\n  method: post\n  operationId: disableShiftTag\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/order\n  method: get\n\
  \  operationId: getOrderBySourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/order/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/order/{orderId}\n  method: put\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/park\n  method: put\n  operationId: parkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/cancel\n  method: put\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/open\n  method: put\n  operationId: openOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/complete\n  method: put\n  operationId: completeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/reschedule\n  method: post\n  operationId: rescheduleOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/order/{orderId}/verify-inventory\n\
  \  method: put\n  operationId: verifyInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/get-slots\n  method: post\n  operationId: getServiceableSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/service-type/{serviceTypeId}\n  method: get\n  operationId: getServiceType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/service-type/{serviceTypeId}\n  method: put\n  operationId: createServiceType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/service-type/{serviceTypeId}/disable\n  method: post\n  operationId: disableServiceType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /client/{clientId}/personnel-master/create-compact\n  method: post\n  operationId: createPersonnelCompact\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/personnel-master/{personnelId}/status\n  method: post\n  operationId: updatePersonnelStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/team-master/{teamId}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/team-master/{teamId}\n  method: put\n  operationId: createTeam\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/team-master/{teamId}/status\n  method: post\n  operationId: updateTeamStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locus-sh/refs/heads/main/agentic-access/locus-sh-agentic-access.yml
summary_line: 48 operations · 34 acting · 10 human-in-the-loop
tags:
- Logistics
- Last Mile Delivery
- Route Optimization
- Dispatch Planning
- Transportation Management
- Fleet Management
- Supply Chain
- Order Management
- Fulfillment
- Track and Trace
- Retail
- E-Commerce
- Artificial Intelligence
- India
---
