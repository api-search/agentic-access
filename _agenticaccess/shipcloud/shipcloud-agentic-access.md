---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 21
api_specs:
- filename: shipcloud-addresses-api-openapi.yml
  format: yaml
  label: shipcloud Addresses API
  slug: shipcloud-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-addresses-api-openapi.yml
- filename: shipcloud-carriers-api-openapi.yml
  format: yaml
  label: shipcloud Carriers API
  slug: shipcloud-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-carriers-api-openapi.yml
- filename: shipcloud-default-returns-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Returns Address API
  slug: shipcloud-default-returns-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-returns-address-api-openapi.yml
- filename: shipcloud-default-shipping-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Shipping Address API
  slug: shipcloud-default-shipping-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-shipping-address-api-openapi.yml
- filename: shipcloud-invoice-address-api-openapi.yml
  format: yaml
  label: shipcloud Invoice Address API
  slug: shipcloud-invoice-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-invoice-address-api-openapi.yml
- filename: shipcloud-manifests-api-openapi.yml
  format: yaml
  label: shipcloud Manifests API
  slug: shipcloud-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-manifests-api-openapi.yml
- filename: shipcloud-me-api-openapi.yml
  format: yaml
  label: shipcloud Me API
  slug: shipcloud-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-me-api-openapi.yml
- filename: shipcloud-orders-api-openapi.yml
  format: yaml
  label: shipcloud Orders API
  slug: shipcloud-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-orders-api-openapi.yml
- filename: shipcloud-pickup-dropoff-locations-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Dropoff Locations API
  slug: shipcloud-pickup-dropoff-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-dropoff-locations-api-openapi.yml
- filename: shipcloud-pickup-requests-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Requests API
  slug: shipcloud-pickup-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-requests-api-openapi.yml
- filename: shipcloud-shipment-quotes-api-openapi.yml
  format: yaml
  label: shipcloud Shipment Quotes API
  slug: shipcloud-shipment-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipment-quotes-api-openapi.yml
- filename: shipcloud-shipments-api-openapi.yml
  format: yaml
  label: shipcloud Shipments API
  slug: shipcloud-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipments-api-openapi.yml
- filename: shipcloud-trackers-api-openapi.yml
  format: yaml
  label: shipcloud Trackers API
  slug: shipcloud-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-trackers-api-openapi.yml
- filename: shipcloud-webhooks-api-openapi.yml
  format: yaml
  label: shipcloud Webhooks API
  slug: shipcloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 21
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipcloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipment_quotes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /shipments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shipments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: shipments/{shipment_id}/shipment_documents
operation_count: 33
overview: 'shipcloud exposes 33 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 6 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: shipcloud
provider_slug: shipcloud
slug: shipcloud-agentic-access
source_filename: shipcloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/shipcloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 21\n    acting: 12\n  by_consequence:\n    read: 21\n    write: 6\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /addresses\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /addresses/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /default_returns_address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /default_shipping_address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice_address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickup_dropoff_locations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickup_requests\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickup_requests\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickup_requests/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment_quotes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: shipments/{shipment_id}/shipment_documents\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: shipments/{shipment_id}/shipment_documents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: shipments/{shipment_id}/shipment_documents/{shipment_document_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackers\n  method: get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trackers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/agentic-access/shipcloud-agentic-access.yml
summary_line: 33 operations · 12 acting
tags:
- Company
- Shipping
- Logistics
- Carriers
- Labels
- Tracking
- E-Commerce
---
