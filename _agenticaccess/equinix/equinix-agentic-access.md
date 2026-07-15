---
acting_count: 119
action_class_counts:
  acting: 119
  connected: 134
api_specs:
- filename: fabric-openapi-original.yml
  format: yaml
  label: Equinix Fabric API
  slug: fabric
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/fabric-openapi-original.yml
- filename: metal-openapi-original.yml
  format: yaml
  label: Equinix Metal API
  slug: metal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/metal-openapi-original.yml
- filename: eia-openapi-original.yml
  format: yaml
  label: Equinix Internet Access API
  slug: internet-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/eia-openapi-original.yml
- filename: lookup-openapi-original.yml
  format: yaml
  label: Equinix Lookup API
  slug: lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/lookup-openapi-original.yml
- filename: orders-openapi-original.yml
  format: yaml
  label: Equinix Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orders-openapi-original.yml
- filename: orderhistory-openapi-original.yml
  format: yaml
  label: Equinix Order History API
  slug: order-history
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orderhistory-openapi-original.yml
- filename: securecabinet-openapi-original.yml
  format: yaml
  label: Equinix Secure Cabinet API
  slug: secure-cabinet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/securecabinet-openapi-original.yml
- filename: smarthands-openapi-original.yml
  format: yaml
  label: Equinix Smart Hands API
  slug: smart-hands
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/smarthands-openapi-original.yml
- filename: accesstoken-openapi-original.yml
  format: yaml
  label: Equinix API Authentication
  slug: access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/accesstoken-openapi-original.yml
- filename: sts-openapi-original.yml
  format: yaml
  label: Equinix Security Token Service
  slug: sts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/sts-openapi-original.yml
consequence_counts:
  physical: 25
  read: 134
  safety-critical: 4
  write: 90
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Equinix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/otp/app
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/otp/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /colocations/v2/orders/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /colocations/v2/orders/{orderId}/negotiations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /colocations/v2/orders/{orderId}/notes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizations/{id}/payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{id}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /securecabinet/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /transfers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /transfers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/cableRequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/cageCleanup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/cageEscort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/equipmentInstall
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/locatePackage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/moveJumperCable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/other
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/patchCableInstall
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/smarthands/patchCableRemoval
operation_count: 253
overview: 'Equinix exposes 253 API operations that an AI agent could call, of which 119 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 134 read, 90 write, 25 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Equinix
provider_slug: equinix
slug: equinix-agentic-access
source_filename: equinix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/accesstoken-openapi-original.yml, openapi/eia-openapi-original.yml, openapi/lookup-openapi-original.yml,\n  openapi/metal-openapi-original.yml, openapi/orderhistory-openapi-original.yml, openapi/orders-openapi-original.yml,\n  openapi/securecabinet-openapi-original.yml, openapi/smarthands-openapi-original.yml, openapi/sts-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 253\n  by_action_class:\n    acting: 119\n    connected: 134\n  by_consequence:\n    write: 90\n    read: 134\n    physical: 25\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /oauth2/v1/refreshaccesstoken\n  method: post\n  operationId: RefreshOAuth2AccessToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/v1/token\n  method: post\n  operationId: GetOAuth2AccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internetAccess/v2/services\n  method: post\n  operationId: createEquinixInternetAccessv2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /colocations/v2/locations\n\
  \  method: get\n  operationId: Get Locations by permission code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /colocations/v2/patchPanels\n  method: get\n  operationId: Retrieve all patch panels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /colocations/v2/patchPanels/{patchPanelId}\n  method: get\n  operationId: Retrieve patch panel details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /colocations/v2/providers\n  method: get\n  operationId: Retrieve list of providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /colocations/v2/connectionServices\n  method:\
  \ get\n  operationId: Retrieve list of connection services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{id}\n  method: delete\n  operationId: deleteAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches/{id}\n  method: delete\n  operationId: deleteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches/{id}\n  method: get\n  operationId: findBatchById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bgp/sessions/{id}\n  method: delete\n  operationId: deleteBgpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bgp/sessions/{id}\n  method: get\n  operationId: findBgpSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bgp/sessions/{id}\n  method: put\n  operationId: updateBgpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /bgp-dynamic-neighbors/{id}\n  method: delete\n  operationId: deleteBgpDynamicNeighborById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bgp-dynamic-neighbors/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capacity\n  method: get\n  operationId: findCapacityForFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capacity\n  method: post\n  operationId: checkCapacityForFacility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capacity/metros\n  method: get\n  operationId: findCapacityForMetro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capacity/metros\n  method: post\n  operationId: checkCapacityForMetro\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{connection_id}\n  method: delete\n  operationId: deleteInterconnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{connection_id}\n  method: get\n  operationId: getInterconnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}\n  method: put\n  operationId: updateInterconnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{connection_id}/events\n  method: get\n  operationId: findInterconnectionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/ports\n\
  \  method: get\n  operationId: listInterconnectionPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/virtual-circuits\n  method: get\n  operationId: listInterconnectionVirtualCircuits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/ports/{id}\n  method: get\n  operationId: getInterconnectionPort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/ports/{id}/events\n  method: get\n  operationId: findInterconnectionPortEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/ports/{port_id}/virtual-circuits\n\
  \  method: get\n  operationId: listInterconnectionPortVirtualCircuits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connection_id}/ports/{port_id}/virtual-circuits\n  method: post\n  operationId: createInterconnectionPortVirtualCircuit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}\n  method: delete\n  operationId: deleteDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}\n\
  \  method: get\n  operationId: findDeviceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}\n  method: put\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}/actions\n  method: post\n  operationId: performAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}/bandwidth\n  method: get\n  operationId: findInstanceBandwidth\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/bgp/neighbors\n  method: get\n  operationId: getBgpNeighborData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/bgp/sessions\n  method: get\n  operationId: findBgpSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/bgp/sessions\n  method: post\n  operationId: createBgpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}/customdata\n  method: get\n \
  \ operationId: findDeviceCustomdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/diagnostics/screenshot\n  method: get\n  operationId: captureScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/diagnostics/health/rollup\n  method: get\n  operationId: getDeviceHealthRollup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/events\n  method: get\n  operationId: findDeviceEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/firmware-sets\n  method: get\n  operationId: getDeviceFirmwareSets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/ips\n  method: get\n  operationId: findIPAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/ips\n  method: post\n  operationId: createIPAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{id}/metadata\n  method: get\n  operationId: findDeviceMetadataByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/ssh-keys\n  method: get\n  operationId: findDeviceSSHKeys\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/traffic\n  method: get\n  operationId: findTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/usages\n  method: get\n  operationId: findDeviceUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{id}/userdata\n  method: get\n  operationId: findDeviceUserdataByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{instance_id}/ips/{id}/customdata\n  method: get\n  operationId: findIPAssignmentCustomdata\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails\n  method: post\n  operationId: createEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}\n  method: delete\n  operationId: deleteEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}\n  method: get\n  operationId: findEmailById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}\n\
  \  method: put\n  operationId: updateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: findEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: findEventById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facilities\n  method: get\n  operationId: findFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hardware-reservations/{id}\n  method: get\n\
  \  operationId: findHardwareReservationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hardware-reservations/{id}/activate\n  method: post\n  operationId: activateHardwareReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hardware-reservations/{id}/move\n  method: post\n  operationId: moveHardwareReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents\n  method: get\n  operationId: findIncidents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: get\n  operationId: findInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations/{id}\n  method: delete\n  operationId: declineInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invitations/{id}\n  method: get\n  operationId: findInvitationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations/{id}\n  method: put\n  operationId: acceptInvitation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{id}\n  method: get\n  operationId: getInvoiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ips/{id}\n  method: delete\n  operationId: deleteIPAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ips/{id}\n  method: get\n  operationId: findIPAddressById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ips/{id}\n  method: patch\n  operationId: updateIPAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ips/{id}/available\n  method: get\n  operationId: findIPAvailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ips/{id}/customdata\n  method: get\n  operationId: findIPAddressCustomdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/{id}\n  method: delete\n  operationId: deleteLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /licenses/{id}\n  method: get\n  operationId: findLicenseById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/{id}\n  method: put\n  operationId: updateLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/metros\n  method: get\n  operationId: findMetros\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/metros/{id}\n\
  \  method: get\n  operationId: getMetro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/spot/prices\n  method: get\n  operationId: findSpotMarketPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/spot/prices/history\n  method: get\n  operationId: findSpotMarketPricesHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/spot/prices/metros\n  method: get\n  operationId: findMetroSpotMarketPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships/{id}\n  method: delete\n  operationId: deleteMembership\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memberships/{id}\n  method: get\n  operationId: findMembershipById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships/{id}\n  method: put\n  operationId: updateMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metal-gateways/{id}\n  method: delete\n  operationId: deleteMetalGateway\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metal-gateways/{id}\n  method: get\n  operationId: findMetalGatewayById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metal-gateways/{id}/bgp-dynamic-neighbors\n  method: get\n  operationId: getBgpDynamicNeighbors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metal-gateways/{id}/bgp-dynamic-neighbors\n  method: post\n  operationId: createBgpDynamicNeighbor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metal-gateways/{id}/ips\n  method: get\n  operationId: getMetalGatewayElasticIps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metal-gateways/{id}/ips\n  method: post\n  operationId: createMetalGatewayElasticIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operating-system-versions\n  method: get\n  operationId: findOperatingSystemVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operating-systems\n\
  \  method: get\n  operationId: findOperatingSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: findOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: get\n  operationId: findOrganizationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}\n  method: put\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/capacity\n  method: get\n  operationId: findOrganizationCapacityPerFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/capacity/metros\n\
  \  method: get\n  operationId: findOrganizationCapacityPerMetro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/customdata\n  method: get\n  operationId: findOrganizationCustomdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/devices\n  method: get\n  operationId: findOrganizationDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/events\n  method: get\n  operationId: findOrganizationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/facilities\n  method: get\n  operationId: findFacilitiesByOrganization\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/firmware-sets\n  method: get\n  operationId: getOrganizationFirmwareSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/invitations\n  method: get\n  operationId: findOrganizationInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/invitations\n  method: post\n  operationId: createOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /organizations/{id}/invoices\n  method: get\n  operationId: findOrganizationInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/operating-systems\n  method: get\n  operationId: findOperatingSystemsByOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/payment-methods\n  method: get\n  operationId: findOrganizationPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/payment-methods\n  method: post\n  operationId: createPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/plans\n  method: get\n  operationId: findPlansByOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/projects\n  method: get\n  operationId: findOrganizationProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/projects\n  method: post\n  operationId: createOrganizationProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/transfers\n  method: get\n  operationId: findOrganizationTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/connections\n  method: get\n  operationId: organizationListInterconnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/connections\n  method: post\n  operationId: createOrganizationInterconnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods/{id}\n  method: delete\n\
  \  operationId: deletePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods/{id}\n  method: get\n  operationId: findPaymentMethodById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-methods/{id}\n  method: put\n  operationId: updatePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \n\n# --- truncated at 32\
  \ KB (71 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/agentic-access/equinix-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/agentic-access/equinix-agentic-access.yml
summary_line: 253 operations · 119 acting · 4 human-in-the-loop
tags:
- Fortune 1000
- Data Centers
- Interconnection
- Colocation
- Bare Metal
- Cloud Infrastructure
- Networking
---
