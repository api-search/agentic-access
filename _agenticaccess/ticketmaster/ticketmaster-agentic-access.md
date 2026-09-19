---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: ticketmaster-availability-api-openapi.yml
  format: yaml
  label: Ticketmaster Availability API
  slug: ticketmaster-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-availability-api-openapi.yml
- filename: ticketmaster-offerings-api-openapi.yml
  format: yaml
  label: Ticketmaster Offerings API
  slug: ticketmaster-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-offerings-api-openapi.yml
- filename: ticketmaster-attractions-api-openapi.yml
  format: yaml
  label: Ticketmaster Attractions API
  slug: ticketmaster-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-attractions-api-openapi.yml
- filename: ticketmaster-classifications-api-openapi.yml
  format: yaml
  label: Ticketmaster Classifications API
  slug: ticketmaster-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-classifications-api-openapi.yml
- filename: ticketmaster-events-api-openapi.yml
  format: yaml
  label: Ticketmaster Events API
  slug: ticketmaster-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-events-api-openapi.yml
- filename: ticketmaster-suggestions-api-openapi.yml
  format: yaml
  label: Ticketmaster Suggestions API
  slug: ticketmaster-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-suggestions-api-openapi.yml
- filename: ticketmaster-venues-api-openapi.yml
  format: yaml
  label: Ticketmaster Venues API
  slug: ticketmaster-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-venues-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ticketmaster Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Ticketmaster exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ticketmaster
provider_slug: ticketmaster
slug: ticketmaster-agentic-access
source_filename: ticketmaster-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/ticketmaster-attractions-api-openapi.yml, openapi/ticketmaster-availability-api-openapi.yml,\n  openapi/ticketmaster-classifications-api-openapi.yml, openapi/ticketmaster-events-api-openapi.yml,\n  openapi/ticketmaster-offerings-api-openapi.yml, openapi/ticketmaster-suggestions-api-openapi.yml,\n  openapi/ticketmaster-venues-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /attractions.json\n  method: get\n  operationId: searchAttractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /attractions/{id}.json\n  method: get\n  operationId: getAttraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/availability.json\n  method: get\n  operationId: getEventAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifications.json\n  method: get\n  operationId: searchClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events.json\n  method: get\n  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}.json\n  method: get\n  operationId:\
  \ getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}/images.json\n  method: get\n  operationId: getEventImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/offers.json\n  method: get\n  operationId: getEventOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest.json\n  method: get\n  operationId: getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venues.json\n  method: get\n  operationId: searchVenues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /venues/{id}.json\n  method: get\n  operationId: getVenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/agentic-access/ticketmaster-agentic-access.yml
summary_line: 11 operations
tags:
- Commerce
- Concerts
- Entertainment
- Event
- Sports
- Tickets
- Venues
---
