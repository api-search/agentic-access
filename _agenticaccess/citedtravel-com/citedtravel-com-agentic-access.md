---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: citedtravel-com-billing-api-openapi.yml
  format: yaml
  label: CitedTravel Billing API
  slug: citedtravel-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-billing-api-openapi.yml
- filename: citedtravel-com-entry-api-openapi.yml
  format: yaml
  label: CitedTravel Entry API
  slug: citedtravel-com-entry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-entry-api-openapi.yml
- filename: citedtravel-com-facts-api-openapi.yml
  format: yaml
  label: CitedTravel Facts API
  slug: citedtravel-com-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-facts-api-openapi.yml
- filename: citedtravel-com-meta-api-openapi.yml
  format: yaml
  label: CitedTravel Meta API
  slug: citedtravel-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-meta-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Citedtravel Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 14
overview: 'CitedTravel exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CitedTravel
provider_slug: citedtravel-com
slug: citedtravel-com-agentic-access
source_filename: citedtravel-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/citedtravel-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: get\n  operationId: resolveCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{cc}\n\
  \  method: get\n  operationId: getCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{cc}/{category}\n  method: get\n  operationId: getCountryCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/power/compat\n  method: get\n  operationId: powerCompat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entry\n  method: get\n  operationId: getEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trip-brief\n  method: get\n  operationId: getTripBrief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/changes\n  method: get\n  operationId: listChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources/{source_id}\n  method: get\n  operationId: getSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createFreeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: createPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/citedtravel-com/agentic-access/citedtravel-com-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Travel
- Data
- TravelFacts
- Open Data
---
