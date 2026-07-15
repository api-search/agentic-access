---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: dog-ceo-openapi.yml
  format: yaml
  label: Dog CEO API
  slug: dog-ceo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dog-ceo/refs/heads/main/openapi/dog-ceo-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dog Ceo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Dog CEO exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dog CEO
provider_slug: dog-ceo
slug: dog-ceo-agentic-access
source_filename: dog-ceo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dog-ceo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /breeds/list/all\n  method: get\n  operationId: listAllBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/image/random\n  method: get\n  operationId: getRandomImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/image/random/{count}\n  method: get\n  operationId:\
  \ getRandomImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images\n  method: get\n  operationId: getBreedImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/random\n  method: get\n  operationId: getBreedRandomImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/random/{count}\n  method: get\n  operationId: getBreedRandomImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/list\n  method: get\n  operationId: listSubBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images\n  method: get\n  operationId: getSubBreedImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/random\n  method: get\n  operationId: getSubBreedRandomImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/random/{count}\n  method: get\n  operationId: getSubBreedRandomImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dog-ceo/refs/heads/main/agentic-access/dog-ceo-agentic-access.yml
summary_line: 10 operations
tags:
- Dogs
- Images
- Animals
- Open Source
- Free API
- Machine Learning
- Education
---
