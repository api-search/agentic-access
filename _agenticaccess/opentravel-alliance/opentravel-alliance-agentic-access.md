---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 4
api_specs:
- filename: opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Hotel Descriptive Content Resource
  slug: opentravel-2020a-hotel-descriptive-content-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
- filename: opentravel-2020a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Facility Resource
  slug: opentravel-2020a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-facility-resource-defs-openapi.json
- filename: opentravel-2018a-hospitality-offers-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Hospitality Offers Resource
  slug: opentravel-2018a-hospitality-offers-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-hospitality-offers-resource-defs-openapi.json
- filename: opentravel-2018a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Facility Resource
  slug: opentravel-2018a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-facility-resource-defs-openapi.json
consequence_counts:
  read: 4
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opentravel Alliance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'OpenTravel Alliance exposes 15 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenTravel Alliance
provider_slug: opentravel-alliance
slug: opentravel-alliance-agentic-access
source_filename: opentravel-alliance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: generated\nsource: openapi/opentravel-2018a-facility-resource-openapi.json, openapi/opentravel-2018a-hospitality-offers-resource-openapi.json,\n  openapi/opentravel-2020a-facility-resource-defs-openapi.json, openapi/opentravel-2020a-facility-resource-openapi.json,\n  openapi/opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json, openapi/opentravel-2020a-hotel-descriptive-content-resource-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 11\n    connected: 4\n  by_consequence:\n    write: 11\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /HospitalityFindHospitalityAvailability\n  method: post\n  operationId: FindHospitalityAvailability\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HospitalityRetrieveFacilityAvailability\n  method: post\n  operationId: RetrieveHospitalityAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Facilities\n  method: post\n  operationId: HospitalityFacilitySearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /HospitalityPropertyOffers\n  method: post\n  operationId: FindSinglePropertyOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HospitalityOffers\n  method: post\n  operationId: FindMultiPropertyOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Facilities\n  method: post\n  operationId: Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Facilities/{Identifier}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Facilities\n  method: post\n  operationId: Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Facilities/{Identifier}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HotelDescriptiveContents\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /HotelDescriptiveContents/Notifications\n  method: post\n  operationId: Notification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HotelDescriptiveContents/Query\n  method: post\n  operationId: Query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HotelDescriptiveContents\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /HotelDescriptiveContents/Notifications\n  method: post\n  operationId: Notification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HotelDescriptiveContents/Query\n  method: post\n  operationId: Query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/agentic-access/opentravel-alliance-agentic-access.yml
summary_line: 15 operations · 11 acting
tags:
- Travel
- United States
- Standards
- Aviation
- Hospitality
- Hotels
- Car Rental
- Rail
- Cruise
- Distribution
- GDS
- Booking
- Channel
- XML
- JSON-Schema
---
