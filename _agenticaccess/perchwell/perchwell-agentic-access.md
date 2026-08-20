---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: perchwell-listings-api-openapi.yml
  format: yaml
  label: Perchwell Listings API
  slug: perchwell-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-listings-api-openapi.yml
- filename: perchwell-media-api-openapi.yml
  format: yaml
  label: Perchwell Media API
  slug: perchwell-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-media-api-openapi.yml
- filename: perchwell-member-api-openapi.yml
  format: yaml
  label: Perchwell Member API
  slug: perchwell-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-member-api-openapi.yml
- filename: perchwell-metadata-api-openapi.yml
  format: yaml
  label: Perchwell Metadata API
  slug: perchwell-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-metadata-api-openapi.yml
- filename: perchwell-office-api-openapi.yml
  format: yaml
  label: Perchwell Office API
  slug: perchwell-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-office-api-openapi.yml
- filename: perchwell-openhouse-api-openapi.yml
  format: yaml
  label: Perchwell OpenHouse API
  slug: perchwell-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-openhouse-api-openapi.yml
- filename: perchwell-property-api-openapi.yml
  format: yaml
  label: Perchwell Property API
  slug: perchwell-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-property-api-openapi.yml
consequence_counts:
  read: 10
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Perchwell Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Perchwell exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Perchwell
provider_slug: perchwell
slug: perchwell-agentic-access
source_filename: perchwell-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/perchwell-json-api-openapi.yml, openapi/perchwell-reso-web-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/feeds/{account_name}\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /$metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /Property\n  method: get\n  operationId: queryProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Property\n  method: post\n  operationId: createProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Property('{id}')\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Property('{id}')\n  method: patch\n  operationId: updateProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Member\n  method: get\n  operationId: queryMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Member\n  method: post\n  operationId: createMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Member('{id}')\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Member('{id}')\n  method: patch\n  operationId: updateMember\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Office\n  method: get\n  operationId: queryOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Office('{id}')\n  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OpenHouse\n  method: get\n  operationId: queryOpenHouse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OpenHouse\n  method: post\n  operationId: createOpenHouse\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OpenHouse('{id}')\n  method: get\n  operationId: getOpenHouse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OpenHouse('{id}')\n  method: patch\n  operationId: updateOpenHouse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OpenHouse('{id}')\n  method: delete\n  operationId: deleteOpenHouse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Media('{id}')\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/agentic-access/perchwell-agentic-access.yml
summary_line: 18 operations · 8 acting
tags:
- Company
- Real-Estate
- MLS
- Listings
- Property Data
- RESO
- RETS
- OData
- Real Estate Data
---
