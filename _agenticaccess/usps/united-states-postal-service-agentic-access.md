---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: usps-addresses-api-openapi.yml
  format: yaml
  label: United States Postal Service Addresses API
  slug: usps-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/openapi/usps-addresses-api-openapi.yml
- filename: usps-carrier-pickup-api-openapi.yml
  format: yaml
  label: United States Postal Service Carrier Pickup API
  slug: usps-carrier-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/openapi/usps-carrier-pickup-api-openapi.yml
- filename: usps-domestic-prices-api-openapi.yml
  format: yaml
  label: United States Postal Service Domestic Prices API
  slug: usps-domestic-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/openapi/usps-domestic-prices-api-openapi.yml
- filename: usps-tracking-api-openapi.yml
  format: yaml
  label: United States Postal Service Tracking API
  slug: usps-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/openapi/usps-tracking-api-openapi.yml
consequence_counts:
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: United States Postal Service Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'United States Postal Service exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: United States Postal Service
provider_slug: usps
slug: united-states-postal-service-agentic-access
source_filename: united-states-postal-service-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/united-states-postal-service-addresses-api-openapi.yml, openapi/united-states-postal-service-carrier-pickup-api-openapi.yml,\n  openapi/united-states-postal-service-domestic-prices-api-openapi.yml, openapi/united-states-postal-service-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /addresses/v3/address\n  method: get\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/v3/city-state\n\
  \  method: get\n  operationId: getCityState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/v3/zipcode\n  method: get\n  operationId: getZIPCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickup/v3/carrier-pickup\n  method: post\n  operationId: scheduleCarrierPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickup/v3/carrier-pickup\n  method: get\n  operationId: getCarrierPickup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /pickup/v3/carrier-pickup\n  method: put\n  operationId: updateCarrierPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickup/v3/carrier-pickup\n  method: delete\n  operationId: cancelCarrierPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prices/v3/base-rates/search\n  method: post\n  operationId: searchBaseRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/v3/extra-service-rates/search\n\
  \  method: post\n  operationId: searchExtraServiceRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/v3/total-rates/search\n  method: post\n  operationId: searchTotalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/v3/tracking/{trackingNumber}\n  method: get\n  operationId: getTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/v3/tracking\n  method: post\n  operationId: getMultipleTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/agentic-access/united-states-postal-service-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Government
- Postal Service
- Shipping
- Logistics
- Address Validation
- Package Tracking
---
