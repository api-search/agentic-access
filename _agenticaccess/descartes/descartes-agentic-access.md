---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 9
api_specs:
- filename: descartes-3rd-party-tms-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group 3rd Party TMS Integration API
  slug: descartes-3rd-party-tms-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-3rd-party-tms-integration-api-openapi.yml
- filename: descartes-api-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group API - XML API
  slug: descartes-api-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-api-xml-api-openapi.yml
- filename: descartes-carrier-data-connection-and-communication-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Carrier Data Connection and Communication API
  slug: descartes-carrier-data-connection-and-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-carrier-data-connection-and-communication-api-openapi.yml
- filename: descartes-custom-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Custom Integration API
  slug: descartes-custom-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-custom-integration-api-openapi.yml
- filename: descartes-export-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Export API
  slug: descartes-export-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-export-api-api-openapi.yml
- filename: descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
  format: yaml
  label: Descartes Systems Group FraudGuard Carrier and Load Lookup API
  slug: descartes-fraudguard-carrier-and-load-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
- filename: descartes-import-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Import API
  slug: descartes-import-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-import-api-api-openapi.yml
- filename: descartes-load-visibility-order-creation-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility Order Creation - XML API
  slug: descartes-load-visibility-order-creation-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-order-creation-xml-api-openapi.yml
- filename: descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility URL and Data Export Retrieval API
  slug: descartes-load-visibility-url-and-data-export-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
- filename: descartes-search-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Search API
  slug: descartes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-search-api-api-openapi.yml
consequence_counts:
  physical: 6
  read: 9
  safety-critical: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Descartes Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1.0/orders/stoporder/{orderId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1.0/tms/data/stopevent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/order/trackingnumberassignment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/orders/SendMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/orders/changeorder/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/orders/createorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/tms/data/shipmentstatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1.0/tms/data/tmsgateway
operation_count: 25
overview: 'Descartes Systems Group exposes 25 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 8 write, 6 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Descartes Systems Group
provider_slug: descartes
slug: descartes-agentic-access
source_filename: descartes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/descartes-macropoint-capacity-openapi.yml, openapi/descartes-macropoint-carrier-openapi.yml,\n  openapi/descartes-macropoint-visibility-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 16\n    connected: 9\n  by_consequence:\n    write: 8\n    read: 9\n    safety-critical: 2\n    physical: 6\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v2/Carrier\n  method: post\n  operationId: postCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v2/Load\n  method: post\n  operationId: postLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/LSPFindPowerExportV3\n  method: get\n  operationId: getLSPFindPowerExportV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/LSPHistoryExportV3\n  method: get\n  operationId: getLSPHistoryExportV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lspoffer\n  method: put\n  operationId: putLspoffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lspoffer/tms/{lspId}/{offerId}\n  method: get\n  operationId: getLspofferTmsLspIdOfferId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lspoffer/tms/{lspId}\n  method: get\n  operationId: getLspofferTmsLspId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lspoffer/tms/{lspId}/accept/{offerId}\n  method: get\n  operationId: getLspofferTmsLspIdAcceptOfferId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lspoffer/{offerId}\n  method:\
  \ delete\n  operationId: deleteLspofferOfferId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lspoffer/{offerId}\n  method: get\n  operationId: getLspofferOfferId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lspoffer/accept/{offerId}\n  method: get\n  operationId: getLspofferAcceptOfferId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/tms/data/location\n  method: post\n  operationId: postTmsDataLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/tms/data/stopevent\n  method: post\n  operationId: postTmsDataStopevent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1.0/order/trackingnumberassignment\n  method: post\n  operationId: postOrderTrackingnumberassignment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/1.0/tms/data/shipmentstatus\n  method: post\n  operationId: postTmsDataShipmentstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/TMS/Data/FormUpload\n  method: post\n  operationId: postTMSDataFormUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/orders/createorder\n  method: post\n  operationId: postOrdersCreateorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/orders/changeorder/{orderId}\n  method: post\n  operationId: postOrdersChangeorderOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/orders/stoporder/{orderId}\n  method: post\n  operationId: postOrdersStoporderOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1.0/tms/data/tmsgateway\n  method: post\n  operationId: postTmsDataTmsgateway\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/carrier/carrierwishlist\n  method: post\n  operationId: postCarrierCarrierwishlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/carrier/requestpartnerstatus/{CarrierID}\n  method: get\n  operationId: getCarrierRequestpartnerstatusCarrierID\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/orders/SendMessage\n  method: post\n  operationId: postOrdersSendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carrier-lookup\n  method: options\n  operationId: optionsCarrierlookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/fraudguard\n  method: post\n  operationId: postFraudguard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/agentic-access/descartes-agentic-access.yml
summary_line: 25 operations · 16 acting · 2 human-in-the-loop
tags:
- Logistics
- Supply Chain
- Freight Visibility
- Shipment Tracking
- Customs Compliance
- Global Trade
- Trade Content
- Carrier Sourcing
---
