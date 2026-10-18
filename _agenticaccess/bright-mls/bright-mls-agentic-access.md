---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: bright-mls-auth-api-openapi.yml
  format: yaml
  label: Bright MLS Auth API
  slug: bright-mls-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-auth-api-openapi.yml
- filename: bright-mls-listing-api-openapi.yml
  format: yaml
  label: Bright MLS Listing API
  slug: bright-mls-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-listing-api-openapi.yml
- filename: bright-mls-manifests-api-openapi.yml
  format: yaml
  label: Bright MLS Manifests API
  slug: bright-mls-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-manifests-api-openapi.yml
- filename: bright-mls-user-api-openapi.yml
  format: yaml
  label: Bright MLS User API
  slug: bright-mls-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-user-api-openapi.yml
- filename: bright-mls-data-hub-api-openapi.yml
  format: yaml
  label: Bright MLS Data Hub API
  slug: bright-mls-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-data-hub-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bright Mls Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /datahub/user
operation_count: 7
overview: 'Bright MLS exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bright MLS
provider_slug: bright-mls
slug: bright-mls-agentic-access
source_filename: bright-mls-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/bright-mls-data-hub-ingestion-service-openapi.json, openapi/bright-mls-datalake-distribution-service-openapi.json,\n  openapi/bright-mls-manifest-services-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 4\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /datahub\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /datahub/listing/delta/{date}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datahub/listing/historical/{date}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datahub/user\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datahub/auth/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests/{uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/agentic-access/bright-mls-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Company
- Real Estate
- MLS
- RESO
- OData
- Listings
- Property Data
---
