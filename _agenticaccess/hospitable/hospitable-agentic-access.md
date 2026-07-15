---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Properties API
  slug: hospitable-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Listings API
  slug: hospitable-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reservations API
  slug: hospitable-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Messages API
  slug: hospitable-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Calendar API
  slug: hospitable-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reviews API
  slug: hospitable-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hospitable Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reservations/{uuid}/messages
operation_count: 13
overview: 'Hospitable exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hospitable
provider_slug: hospitable
slug: hospitable-agentic-access
source_filename: hospitable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hospitable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /properties\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{uuid}\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/search\n\
  \  method: post\n  operationId: searchProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{uuid}\n  method: get\n  operationId: getReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{uuid}/messages\n\
  \  method: get\n  operationId: listReservationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{uuid}/messages\n  method: post\n  operationId: sendReservationMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{uuid}/calendar\n  method: get\n  operationId: getPropertyCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{uuid}/calendar\n  method: put\n  operationId: updatePropertyCalendar\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{uuid}/reviews\n  method: get\n  operationId: listPropertyReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews/{uuid}/response\n  method: post\n  operationId: respondToReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/agentic-access/hospitable-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Airbnb
- Hospitality
- Automation
---
