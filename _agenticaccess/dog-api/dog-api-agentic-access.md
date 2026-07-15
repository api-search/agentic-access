---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: dog-api.yml
  format: yaml
  label: Dog API
  slug: dog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/openapi/dog-api.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dog Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Dog API exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dog API
provider_slug: dog-api
slug: dog-api-agentic-access
source_filename: dog-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dog-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /breeds/list/all\n  method: get\n  operationId: listAllBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/list/all/random\n  method: get\n  operationId: randomBreedEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/list/all/random/{amount}\n  method: get\n  operationId:\
  \ randomBreedEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/list\n  method: get\n  operationId: listTopLevelBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/list/random\n  method: get\n  operationId: randomTopLevelBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/list/random/{amount}\n  method: get\n  operationId: randomTopLevelBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/list\n  method: get\n  operationId: listSubBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/list/random\n  method: get\n  operationId: randomSubBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/list/random/{amount}\n  method: get\n  operationId: randomSubBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images\n  method: get\n  operationId: listImagesByBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/random\n  method: get\n  operationId: randomImageByBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/random/{amount}\n\
  \  method: get\n  operationId: randomImagesByBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images\n  method: get\n  operationId: listImagesBySubBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/random\n  method: get\n  operationId: randomImageBySubBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/random/{amount}\n  method: get\n  operationId: randomImagesBySubBreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/image/random\n  method: get\n  operationId:\
  \ randomImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/image/random/{amount}\n  method: get\n  operationId: randomImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds/image/random/{amount}/alt\n  method: get\n  operationId: randomImagesWithAlt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/alt\n  method: get\n  operationId: listImagesByBreedWithAlt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/images/random/{amount}/alt\n  method: get\n  operationId: randomImagesByBreedWithAlt\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/alt\n  method: get\n  operationId: listImagesBySubBreedWithAlt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}/images/random/{amount}/alt\n  method: get\n  operationId: randomImagesBySubBreedWithAlt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}\n  method: get\n  operationId: getBreedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/{breed}/{subBreed}\n  method: get\n  operationId: getSubBreedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/agentic-access/dog-api-agentic-access.yml
summary_line: 24 operations
tags:
- Dogs
- Images
- Open Data
- Open Source
---
