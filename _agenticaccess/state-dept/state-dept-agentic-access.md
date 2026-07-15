---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: openapi.yaml
  format: yaml
  label: State Department Consular Affairs API
  slug: state-dept-consular-affairs
  spec_type: OpenAPI
  url: https://cadataapi.state.gov/
- filename: openapi.yaml
  format: yaml
  label: State Department Travel Advisories
  slug: state-dept-travel-advisories
  spec_type: OpenAPI
  url: https://cadataapi.state.gov/
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: State Dept Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'State Department exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: State Department
provider_slug: state-dept
slug: state-dept-agentic-access
source_filename: state-dept-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/state-dept-consular-affairs-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/TravelAdvisories\n  method: get\n  operationId: getTravelAdvisories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/TravelAdvisories/{countryCode}\n  method: get\n  operationId: getTravelAdvisoryByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/CountryTravelInformation\n  method: get\n  operationId: getCountryTravelInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/CountryTravelInformation/{tag}\n  method: get\n  operationId: getCountryTravelInformationByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/CountryTravelInformation/{tag}/{field}\n  method: get\n  operationId: getCountryTravelInformationByTagAndField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Passport/Applications/Locations\n  method: get\n  operationId: getAllPassportLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/Passport/Applications/Locations/States/{stateCode}\n  method: get\n  operationId: getPassportLocationsByState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Passport/Applications/Locations/ZipCode/{zipcode}\n  method: get\n  operationId: getPassportLocationsByZipCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Passport/Applications/Locations/ZipCode/{zipcode}/{miles}\n  method: get\n  operationId: getPassportLocationsByZipCodeAndRadius\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Passport/Applications/Locations/GeoLocation/{geolocation}\n  method: get\n  operationId: getPassportLocationsByGeoLocation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-dept/refs/heads/main/agentic-access/state-dept-agentic-access.yml
summary_line: 10 operations
tags:
- US Government
- Travel
- Passports
- Visas
- Travel Advisories
- Consular Affairs
- Foreign Policy
- Diplomatic
- Country Information
- Public Safety
---
