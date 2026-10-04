---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: fakerapi-addresses-api-openapi.yml
  format: yaml
  label: FakerAPI Addresses API
  slug: fakerapi-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-addresses-api-openapi.yml
- filename: fakerapi-books-api-openapi.yml
  format: yaml
  label: FakerAPI Books API
  slug: fakerapi-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-books-api-openapi.yml
- filename: fakerapi-companies-api-openapi.yml
  format: yaml
  label: FakerAPI Companies API
  slug: fakerapi-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-companies-api-openapi.yml
- filename: fakerapi-custom-api-openapi.yml
  format: yaml
  label: FakerAPI Custom API
  slug: fakerapi-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-custom-api-openapi.yml
- filename: fakerapi-images-api-openapi.yml
  format: yaml
  label: FakerAPI Images API
  slug: fakerapi-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-images-api-openapi.yml
- filename: fakerapi-persons-api-openapi.yml
  format: yaml
  label: FakerAPI Persons API
  slug: fakerapi-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-persons-api-openapi.yml
- filename: fakerapi-places-api-openapi.yml
  format: yaml
  label: FakerAPI Places API
  slug: fakerapi-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-places-api-openapi.yml
- filename: fakerapi-products-api-openapi.yml
  format: yaml
  label: FakerAPI Products API
  slug: fakerapi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-products-api-openapi.yml
- filename: fakerapi-texts-api-openapi.yml
  format: yaml
  label: FakerAPI Texts API
  slug: fakerapi-texts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-texts-api-openapi.yml
- filename: fakerapi-users-api-openapi.yml
  format: yaml
  label: FakerAPI Users API
  slug: fakerapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-users-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fakerapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'FakerAPI exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FakerAPI
provider_slug: fakerapi
slug: fakerapi-agentic-access
source_filename: fakerapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fakerapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /addresses\n  method: get\n  operationId: listAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /books\n  method: get\n  operationId: listBooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /persons\n  method: get\n  operationId: listPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places\n  method: get\n  operationId: listPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /texts\n  method: get\n  operationId: listTexts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom\n  method: get\n  operationId: listCustom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/agentic-access/fakerapi-agentic-access.yml
summary_line: 10 operations
tags:
- Test Data
- Fake Data
- Mocking
- Developer Tools
- Open Source
- Public APIs
---
