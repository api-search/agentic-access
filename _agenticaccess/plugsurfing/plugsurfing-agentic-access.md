---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 30
api_specs:
- filename: plugsurfing-charging-key-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Key Orders API
  slug: plugsurfing-charging-key-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-charging-key-orders-api-openapi.yml
- filename: plugsurfing-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Keys API
  slug: plugsurfing-charging-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-charging-keys-api-openapi.yml
- filename: plugsurfing-drive-api-api-openapi.yml
  format: yaml
  label: Plugsurfing Drive API
  slug: plugsurfing-drive-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-drive-api-api-openapi.yml
- filename: plugsurfing-emp-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Charging Keys API
  slug: plugsurfing-emp-charging-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-emp-charging-keys-api-openapi.yml
- filename: plugsurfing-emp-fleets-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Fleets API
  slug: plugsurfing-emp-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-emp-fleets-api-openapi.yml
- filename: plugsurfing-emp-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Geosearch API
  slug: plugsurfing-emp-geosearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-emp-geosearch-api-openapi.yml
- filename: plugsurfing-emp-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Orders API
  slug: plugsurfing-emp-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-emp-orders-api-openapi.yml
- filename: plugsurfing-emp-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Sessions API
  slug: plugsurfing-emp-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-emp-sessions-api-openapi.yml
- filename: plugsurfing-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing Geosearch API
  slug: plugsurfing-geosearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-geosearch-api-openapi.yml
- filename: plugsurfing-payment-options-api-openapi.yml
  format: yaml
  label: Plugsurfing Payment Options API
  slug: plugsurfing-payment-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-payment-options-api-openapi.yml
- filename: plugsurfing-remote-charging-api-openapi.yml
  format: yaml
  label: Plugsurfing Remote Charging API
  slug: plugsurfing-remote-charging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-remote-charging-api-openapi.yml
- filename: plugsurfing-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing Sessions API
  slug: plugsurfing-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-sessions-api-openapi.yml
- filename: plugsurfing-user-groups-api-openapi.yml
  format: yaml
  label: Plugsurfing User Groups API
  slug: plugsurfing-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-user-groups-api-openapi.yml
- filename: plugsurfing-users-api-openapi.yml
  format: yaml
  label: Plugsurfing Users API
  slug: plugsurfing-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-users-api-openapi.yml
- filename: plugsurfing-vouchers-api-openapi.yml
  format: yaml
  label: Plugsurfing Vouchers API
  slug: plugsurfing-vouchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plugsurfing/openapi/plugsurfing-vouchers-api-openapi.yml
consequence_counts:
  physical: 10
  read: 30
  safety-critical: 3
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Plugsurfing Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /drive/v1/users/{userId}/sessions/{sessionId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /emp/v1/charging-keys/{keyIdentifier}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emp/v1/sessions/{sessionId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /drive/v1/users/{userId}/charging-keys/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /drive/v1/users/{userId}/charging-keys/plug-and-charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /drive/v1/users/{userId}/payment-options
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /drive/v1/users/{userId}/payment-options/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /drive/v1/users/{userId}/sessions/{sessionId}/payments/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /drive/v1/users/{userId}/user-groups/{groupId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /drive/v1/users/{userId}/user-groups/{groupId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /emp/v1/charging-keys/{keyIdentifier}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emp/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emp/v1/orders/{orderId}/assign
operation_count: 59
overview: 'Plugsurfing exposes 59 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 16 write, 10 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Plugsurfing
provider_slug: plugsurfing
slug: plugsurfing-agentic-access
source_filename: plugsurfing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/plugsurfing-charging-key-orders-api-openapi.yml, openapi/plugsurfing-charging-keys-api-openapi.yml,\n  openapi/plugsurfing-emp-charging-keys-api-openapi.yml, openapi/plugsurfing-emp-fleets-api-openapi.yml,\n  openapi/plugsurfing-emp-geosearch-api-openapi.yml, openapi/plugsurfing-emp-orders-api-openapi.yml,\n  openapi/plugsurfing-emp-sessions-api-openapi.yml, openapi/plugsurfing-geosearch-api-openapi.yml,\n  openapi/plugsurfing-payment-options-api-openapi.yml, openapi/plugsurfing-remote-charging-api-openapi.yml,\n  openapi/plugsurfing-sessions-api-openapi.yml, openapi/plugsurfing-user-groups-api-openapi.yml,\n  openapi/plugsurfing-users-api-openapi.yml, openapi/plugsurfing-vouchers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See\
  \ research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    acting: 29\n    connected: 30\n  by_consequence:\n    physical: 10\n    read: 30\n    write: 16\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /drive/v1/users/{userId}/charging-keys/orders\n  method: post\n  operationId: createChargingKeyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/charging-keys/orders\n  method: get\n  operationId: listChargingKeyOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/charging-keys/orders/{orderId}/receipt\n\
  \  method: get\n  operationId: getChargingKeyOrderReceiptUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/charging-keys/orders/configuration\n  method: get\n  operationId: getChargingKeyOrderConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/charging-keys/{referenceId}/activate\n  method: post\n  operationId: activateUserChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/charging-keys/{identifier}\n  method: patch\n  operationId: updateUserChargingKey\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/charging-keys\n  method: get\n  operationId: listUserChargingKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/charging-keys\n  method: post\n  operationId: createUserChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/charging-keys/plug-and-charge\n  method: post\n  operationId: createPncChargingKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/charging-keys/reservations\n  method: post\n  operationId: createChargingKeyReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/charging-keys\n  method: get\n  operationId: listEmpChargingKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/charging-keys\n  method: post\n  operationId:\
  \ createEmpChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/charging-keys/{keyIdentifier}/rename\n  method: put\n  operationId: renameEmpChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/charging-keys/{keyIdentifier}/enable\n  method: put\n  operationId: enableEmpChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/charging-keys/{keyIdentifier}/disable\n  method: put\n  operationId: disableEmpChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emp/v1/charging-keys/{keyIdentifier}/transfer\n  method: put\n  operationId: transferEmpChargingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/fleets\n  method: post\n  operationId: createFleet\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/fleets/{fleetId}/rename\n  method: put\n  operationId: renameFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/fleets/{fleetId}/invitation\n  method: get\n  operationId: getFleetInvitationCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/geosearch/radius\n  method: post\n  operationId: searchEmpLocationsByRadius\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/geosearch/rectangle\n  method: post\n  operationId: searchEmpLocationsByRectangle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/geosearch/route\n  method: post\n  operationId: searchEmpLocationsByRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/locations/{locationId}\n  method: get\n  operationId: getEmpLocationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/locations/{locationId}/live-data\n  method: get\n  operationId: getEmpLocationLiveData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/locations/batch\n  method: get\n  operationId: getEmpLocationsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/orders\n  method: get\n  operationId: listEmpChargingKeyOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/orders\n  method: post\n  operationId: createEmpChargingKeyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/orders/{orderId}/assign\n  method: post\n  operationId:\
  \ assignEmpChargingKeyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/products\n  method: get\n  operationId: getEmpProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/sessions/start\n  method: post\n  operationId: startRemoteSessionEmp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emp/v1/sessions/{sessionId}/stop\n  method: post\n\
  \  operationId: stopRemoteSessionEmp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emp/v1/sessions/{sessionId}/receipt\n  method: get\n  operationId: getSessionReceiptEmp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/sessions/{sessionId}\n  method: get\n  operationId: getSessionByIdEmp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/geosearch/radius\n  method: post\n  operationId: searchLocationsByRadius\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/geosearch/rectangle\n  method: post\n  operationId: searchLocationsByRectangle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/geosearch/route\n  method: post\n  operationId: searchLocationsByRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/locations/{locationId}\n  method: get\n  operationId: getLocationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/locations/{locationId}/live-data\n  method: get\n  operationId: getLocationLiveData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /drive/v1/locations/batch\n  method: get\n  operationId: getLocationsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/locations/operators\n  method: get\n  operationId: listOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/payment-options\n  method: get\n  operationId: listPaymentOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/payment-options\n  method: post\n  operationId: createPaymentOption\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/payment-options/stripe-setup-intent\n  method: get\n  operationId: createStripeSetupIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/payment-options/{id}\n  method: delete\n  operationId: deletePaymentOption\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/prepaid\n  method: get\n  operationId: listPrepaid\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emp/v1/payment-options/stripe/publishable-api-key\n  method: get\n  operationId: getStripePublishableApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/sessions/start\n  method: post\n  operationId: startRemoteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/sessions/{sessionId}/stop\n  method: post\n  operationId: stopRemoteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /drive/v1/users/{userId}/sessions/history\n  method: post\n  operationId: listSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/sessions/{sessionId}\n  method: get\n  operationId: getSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/sessions/{sessionId}/receipt\n  method: get\n  operationId: getSessionReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}/sessions/{sessionId}/payments/retry\n  method: post\n  operationId: retrySessionPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/user-groups/{groupId}\n  method: post\n  operationId: createUserGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/user-groups/{groupId}\n  method:\
  \ delete\n  operationId: deleteUserGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v1/users/{userId}\n  method: patch\n\
  \  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v1/users/{userId}/vouchers/{code}/redeem\n  method: post\n  operationId: redeem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/plugsurfing/agentic-access/plugsurfing-agentic-access.yml
summary_line: 59 operations · 29 acting · 3 human-in-the-loop
tags:
- Company
- EV Charging
- Roaming
- Europe
---
