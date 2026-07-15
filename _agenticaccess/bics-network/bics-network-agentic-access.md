---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 38
api_specs:
- filename: bics-sms-openapi.json
  format: json
  label: BICS SMS API
  slug: bics-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-sms-openapi.json
- filename: bics-mynumbers-openapi.json
  format: json
  label: BICS MyNumbers API
  slug: bics-mynumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-openapi.json
- filename: bics-mynumbers-porting-openapi.json
  format: json
  label: BICS MyNumbers Number Porting API
  slug: bics-mynumbers-number-porting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-porting-openapi.json
- filename: bics-mynumbers-cdr-openapi.json
  format: json
  label: BICS MyNumbers CDR API
  slug: bics-mynumbers-cdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-cdr-openapi.json
- filename: bics-mynumbers-address-management-openapi.json
  format: json
  label: BICS MyNumbers Address Management API
  slug: bics-mynumbers-address-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-address-management-openapi.json
- filename: bics-mynumbers-disconnection-openapi.json
  format: json
  label: BICS MyNumbers Disconnection API
  slug: bics-mynumbers-disconnection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-disconnection-openapi.json
- filename: bics-mynumbers-emergency-services-openapi.json
  format: json
  label: BICS MyNumbers Emergency Services API
  slug: bics-mynumbers-emergency-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-emergency-services-openapi.json
- filename: bics-connect-openapi.json
  format: json
  label: BICS Connect API
  slug: bics-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-connect-openapi.json
consequence_counts:
  physical: 8
  read: 38
  safety-critical: 7
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Bics Network Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emergencyservices/orders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /emergencyservices/orders/{orderId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /emergencyservices/orders/{orderId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emergencyservices/orders/{orderId}/orderitems
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /emergencyservices/orders/{orderId}/orderitems/{orderItemId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /emergencyservices/orders/{orderId}/orderitems/{orderItemId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emergencyservices/orders/{orderId}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /disconnections/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /disconnections/orders/{orderId}/orderitems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /disconnections/orders/{orderId}/orderitems/{orderItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /disconnections/orders/{orderId}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /order/{orderReference}/orderItem/{orderItemReference}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outbound/{senderAddress}/requests
operation_count: 76
overview: 'BICS exposes 76 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 23 write, 8 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BICS
provider_slug: bics-network
slug: bics-network-agentic-access
source_filename: bics-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bics-connect-openapi.json, openapi/bics-mynumbers-address-management-openapi.json,\n  openapi/bics-mynumbers-cdr-openapi.json, openapi/bics-mynumbers-disconnection-openapi.json,\n  openapi/bics-mynumbers-emergency-services-openapi.json, openapi/bics-mynumbers-openapi.json,\n  openapi/bics-mynumbers-porting-openapi.json, openapi/bics-sms-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 38\n    acting: 38\n  by_consequence:\n    read: 38\n    write: 23\n    physical: 8\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /connections/{connectionId}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{connectionId}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{connectionId}/modify\n  method: post\n  operationId: modifyConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata\n  method: get\n  operationId: getRefData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: get\n  operationId: getConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interconnects\n  method: get\n  operationId: getInterconnects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{reference}\n  method: get\n  operationId: Get Address By Reference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{reference}\n  method: put\n  operationId: Update Address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{reference}\n  method: delete\n  operationId: Delete Address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{reference}/documents/{documentReference}\n  method: delete\n  operationId: Delete Document By Reference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{reference}/documentTypeCode/{code}\n  method: delete\n  operationId: Delete Document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{reference}/documents\n  method: post\n  operationId: Add Document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses\n  method: get\n  operationId: Get Addresses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: post\n  operationId: Create Address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdrs/{id}/download/{format}\n  method: get\n  operationId: Download CDR Request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdrs/{id}/status\n  method: get\n  operationId: Get status of CDR Request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdrs/availableDates\n  method: get\n  operationId: Get\
  \ available CDR dates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdrs\n  method: post\n  operationId: Request CDRs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disconnections/orders/{orderId}/submit\n  method: post\n  operationId: submit Disconnection Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disconnections/orders/{orderId}/orderitems/{orderItemId}\n\
  \  method: delete\n  operationId: delete Disconnection Order Item\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disconnections/orders\n  method: post\n  operationId: create Disconnection Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disconnections/orders/{orderId}/orderitems\n  method: post\n  operationId: add Disconnection Order Item\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emergencyservices/requirements/{country}\n  method: get\n  operationId: get Emergency Service Country Specific Fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emergencyservices/orders\n  method: get\n  operationId: get Emergency Services Orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emergencyservices/orders\n  method: post\n  operationId: create Emergency Services Order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}\n  method: get\n  operationId: get Emergency Service Order Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emergencyservices/orders/{orderId}\n  method: delete\n  operationId: cancel Emergency Service Order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}\n  method: patch\n  operationId: update Emergency Service Order\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}/orderitems\n  method: post\n  operationId: create Emergency Service Order Item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}/orderitems/{orderItemId}\n  method: delete\n  operationId: delete Emergency Service Order Item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}/orderitems/{orderItemId}\n  method: patch\n  operationId: update Emergency Service Order Item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emergencyservices/orders/{orderId}/submit\n  method: post\n  operationId: submit Emergency Service Order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n  \
  \  escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stock/product/{product}/country/{country}/quantity/{quantity}\n  method: get\n  operationId: Check Available Stock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/languages\n  method: get\n  operationId: Get Languages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers\n  method: get\n  operationId: get Inventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/locations/country/{country}\n  method: get\n  operationId: get Locations By Country\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /numbers/{number}/services\n  method: get\n  operationId: get number services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/bulk\n  method: post\n  operationId: Order Numbers In Bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/locations\n  method: get\n  operationId: get Locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/{orderId}\n  method: get\n  operationId: Get Order Details\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/calendar\n  method: get\n  operationId: get Calendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/{number}\n  method: get\n  operationId: get Number Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stock/product/{product}/country/{country}/location/{location}/quantity/{quantity}\n  method: get\n  operationId: Check Available Stock By Location\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricelist/product/{product}\n  method: get\n  operationId: get Pricelist By Product\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/addressReference\n  method: delete\n  operationId: Delete address reference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/pops\n  method: get\n  operationId: get POPs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/pops/product/{product}\n  method: get\n  operationId: get POPs by Product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: post\n  operationId: Update routes\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /specifications\n  method: get\n  operationId: get specifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order\n  method: post\n  operationId: Order Single Number\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/calendar/product/{product}\n  method: get\n  operationId: get Calendars by Product\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/{orderReference}/orderItem/{orderItemReference}\n  method: patch\n  operationId: Edit Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/addressReferences\n  method: post\n  operationId: Update address reference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/documenttypes\n  method: get\n  operationId:\
  \ Get Document Types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /availablenumbers\n  method: get\n  operationId: get available numbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricelist/product/{product}/country/{country}\n  method: get\n  operationId: get Pricelist By Product And Country\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portings/{portingRequestId}/documents\n  method: get\n  operationId: get porting request documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portings/{portingRequestId}/documents\n  method: post\n  operationId: Update\
  \ Porting Request Documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portings\n  method: get\n  operationId: get porting requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portings\n  method: post\n  operationId: Create porting request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portings/{portingRequestId}/addresses\n  method: patch\n  operationId: Update porting request addresses\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portings/specifications\n  method: get\n  operationId: get porting specifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portings/{portingRequestId}\n  method: get\n  operationId: get porting request by id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portings/{portingRequestId}\n  method: delete\n  operationId: cancel porting request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound/subscriptions\n  method: get\n  operationId: Get Inbound Messages Subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbound/subscriptions\n  method: post\n  operationId: Create Inbound Messages Subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound/subscriptions\n  method: delete\n  operationId: Delete Inbound Messages Subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions\n  method: post\n  operationId: Process SMS Conversion info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversionsinfos\n  method: post\n  operationId: Process SMS Conversion infos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outbound/{senderAddress}/requests\n  method: post\n  operationId: Send Message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outbound/subscriptions\n  method: get\n  operationId: Get Delivery Info Subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outbound/subscriptions\n  method: post\n  operationId: Create Delivery Info Subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outbound/subscriptions\n  method: delete\n  operationId: Delete Delivery Info Subscription\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound/registrations/{inboundNumber}/messages\n  method: get\n  operationId: Get Inbound Messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outbound/{senderAddress}/requests/{requestId}/deliveryInfos\n  method: get\n  operationId: Get Delivery Infos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/agentic-access/bics-network-agentic-access.yml
summary_line: 76 operations · 38 acting · 7 human-in-the-loop
tags:
- Number Verification
- Telecom
- Mobile Identity
- Anti-Fraud
- Device Location
- OTP
- SMS
- Numbering
- Number Portability
- Fraud Prevention
- Carrier
- CPaaS
---
