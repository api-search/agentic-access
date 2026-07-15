---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Listings and Properties API
  slug: listings-properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: offices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Open Houses API
  slug: open-houses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge RESO Web API
  slug: reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bridge Interactive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Bridge Interactive exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bridge Interactive
provider_slug: bridge-interactive
slug: bridge-interactive-agentic-access
source_filename: bridge-interactive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bridge-interactive-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /{dataset_id}/listings\n  method: get\n  operationId: getListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/listings/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/agents\n  method: get\n\
  \  operationId: getAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/agents/{id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/offices\n  method: get\n  operationId: getOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/offices/{id}\n  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset_id}/openhouses\n  method: get\n  operationId: getOpenHouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/$metadata\n  method: get\n  operationId: getResoMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/Property\n  method: get\n  operationId: getResoProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/Property/replication\n  method: get\n  operationId: getResoPropertyReplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/Member\n  method: get\n  operationId: getResoMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /OData/{dataset_id}/Office\n  method: get\n  operationId: getResoOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/OpenHouse\n  method: get\n  operationId: getResoOpenHouse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OData/{dataset_id}/Media\n  method: get\n  operationId: getResoMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/agentic-access/bridge-interactive-agentic-access.yml
summary_line: 14 operations
tags:
- Real Estate
- MLS
- RESO
- Listings
- Property Data
---
