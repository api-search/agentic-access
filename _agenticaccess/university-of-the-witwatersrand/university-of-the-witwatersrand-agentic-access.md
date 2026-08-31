---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: university-of-the-witwatersrand-root-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Root API
  slug: university-of-the-witwatersrand-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-root-api-openapi.yml
- filename: university-of-the-witwatersrand-communities-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Communities API
  slug: university-of-the-witwatersrand-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-communities-api-openapi.yml
- filename: university-of-the-witwatersrand-collections-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Collections API
  slug: university-of-the-witwatersrand-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-collections-api-openapi.yml
- filename: university-of-the-witwatersrand-items-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Items API
  slug: university-of-the-witwatersrand-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-items-api-openapi.yml
- filename: university-of-the-witwatersrand-discovery-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Discovery API
  slug: university-of-the-witwatersrand-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-discovery-api-openapi.yml
- filename: university-of-the-witwatersrand-request-api-openapi.yml
  format: yaml
  label: WIReDSpace OAI-PMH Interface
  slug: university-of-the-witwatersrand-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-request-api-openapi.yml
consequence_counts:
  read: 9
description: 'Recommended x-agentic-access execution contracts, classified heuristically from the institution-operated WIReDSpace OpenAPIs (DSpace 9.2 REST + OAI-PMH 2.0). Regenerated 2026-08-30 after the vendor-operated Figshare contract was removed from this repo: 157 operations that belonged to api.figshare.com were dropped, because a governance contract inherits the operator of the API it governs. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: University Of The Witwatersrand Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'University of the Witwatersrand exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of the Witwatersrand
provider_slug: university-of-the-witwatersrand
slug: university-of-the-witwatersrand-agentic-access
source_filename: university-of-the-witwatersrand-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: generated\nsource: openapi/university-of-the-witwatersrand-wiredspace-oai.yaml, openapi/university-of-the-witwatersrand-wiredspace-rest.yaml\nx-operator: institution\ndescription: 'Recommended x-agentic-access execution contracts, classified heuristically from the institution-operated\n  WIReDSpace OpenAPIs (DSpace 9.2 REST + OAI-PMH 2.0). Regenerated 2026-08-30 after the vendor-operated\n  Figshare contract was removed from this repo: 157 operations that belonged to api.figshare.com were\n  dropped, because a governance contract inherits the operator of the API it governs. A governance starting\n  point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.'\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /request\n  method: get\n  operationId: oaiRequest\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities\n  method: get\n  operationId: getCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections/{uuid}\n\
  \  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/items/{uuid}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover/browses\n  method: get\n  operationId: getBrowses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover/search/objects\n  method: get\n  operationId: searchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/agentic-access/university-of-the-witwatersrand-agentic-access.yml
summary_line: 9 operations
tags:
- University
- Higher Education
- Education
- Research
- South Africa
- Africa
- Institutional Repository
- Research Data
- Open Access
- Identity Federation
- OAI-PMH
- DSpace
---
