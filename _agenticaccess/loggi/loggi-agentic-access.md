---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: loggi-authapi-api-openapi.yml
  format: yaml
  label: Loggi Auth API
  slug: loggi-authapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-authapi-api-openapi.yml
- filename: loggi-detailsapi-api-openapi.yml
  format: yaml
  label: Loggi Details API
  slug: loggi-detailsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-detailsapi-api-openapi.yml
- filename: loggi-dropofflocationsapi-api-openapi.yml
  format: yaml
  label: Loggi Dropoff Locations API
  slug: loggi-dropofflocationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-dropofflocationsapi-api-openapi.yml
- filename: loggi-integratorcompanyapi-api-openapi.yml
  format: yaml
  label: Loggi Integrator Company API
  slug: loggi-integratorcompanyapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-integratorcompanyapi-api-openapi.yml
- filename: loggi-labelapi-api-openapi.yml
  format: yaml
  label: Loggi Label API
  slug: loggi-labelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-labelapi-api-openapi.yml
- filename: loggi-packagecancelapi-api-openapi.yml
  format: yaml
  label: Loggi Package Cancel API
  slug: loggi-packagecancelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packagecancelapi-api-openapi.yml
- filename: loggi-packageupdateapi-api-openapi.yml
  format: yaml
  label: Loggi Package Update API
  slug: loggi-packageupdateapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packageupdateapi-api-openapi.yml
- filename: loggi-quotationapi-api-openapi.yml
  format: yaml
  label: Loggi Quotation API
  slug: loggi-quotationapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-quotationapi-api-openapi.yml
- filename: loggi-shipmentapi-api-openapi.yml
  format: yaml
  label: Loggi Shipment API
  slug: loggi-shipmentapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-shipmentapi-api-openapi.yml
- filename: loggi-trackingapi-api-openapi.yml
  format: yaml
  label: Loggi Tracking API
  slug: loggi-trackingapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-trackingapi-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loggi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/companies/{company_id}/async-shipments
operation_count: 11
overview: 'Loggi exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loggi
provider_slug: loggi
slug: loggi-agentic-access
source_filename: loggi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/loggi-authentication-openapi.yml, openapi/loggi-freight-price-quotation-openapi.yml,\n  openapi/loggi-integrator-openapi.yml, openapi/loggi-labels-openapi.yml, openapi/loggi-package-details-openapi.yml,\n  openapi/loggi-package-openapi.yml, openapi/loggi-pontos-openapi.yml, openapi/loggi-shipments-openapi.yml,\n  openapi/loggi-tracking-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 8\n    connected: 3\n  by_consequence:\n    write: 7\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n  operationId: AuthenticateV1\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/oauth2/token\n  method: post\n  operationId: AuthenticateV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}/quotations\n  method: post\n  operationId: Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrator/activate\n  method: post\n  operationId: CreateIntegratorCompany\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}/labels\n  method: post\n  operationId: CriarEtiqueta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}/packages/{tracking_code}\n  method: get\n  operationId: PackageDetailsTrackingCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}/packages\n  method: patch\n  operationId: PackageUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}/packages/cancel\n  method: post\n  operationId: PackageCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dropoff/locations\n  method: post\n  operationId: ListDropoffLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}/async-shipments\n  method: post\n  operationId: CreateAsyncShipment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}/packages/{tracking_code}/tracking\n  method: get\n  operationId: TrackPackageTrackingCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/agentic-access/loggi-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- Company
- Logistics
- Shipping
- Last Mile Delivery
- Freight
- Tracking
- Brazil
---
