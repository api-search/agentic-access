---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: spring-data-association-api-openapi.yml
  format: yaml
  label: Spring Data Association API
  slug: spring-data-association-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-association-api-openapi.yml
- filename: spring-data-collection-api-openapi.yml
  format: yaml
  label: Spring Data Collection API
  slug: spring-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-collection-api-openapi.yml
- filename: spring-data-discovery-api-openapi.yml
  format: yaml
  label: Spring Data Discovery API
  slug: spring-data-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-discovery-api-openapi.yml
- filename: spring-data-item-api-openapi.yml
  format: yaml
  label: Spring Data Item API
  slug: spring-data-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-item-api-openapi.yml
- filename: spring-data-profile-api-openapi.yml
  format: yaml
  label: Spring Data Profile API
  slug: spring-data-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-profile-api-openapi.yml
- filename: spring-data-search-api-openapi.yml
  format: yaml
  label: Spring Data Search API
  slug: spring-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/openapi/spring-data-search-api-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spring Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Spring Data exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spring Data
provider_slug: spring-data
slug: spring-data-agentic-access
source_filename: spring-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/spring-data-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{resource}\n  method: get\n  operationId:\
  \ getResourceProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}\n  method: get\n  operationId: listResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{repository}/{id}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}/{id}\n  method: put\n  operationId:\
  \ replaceResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{repository}/{id}\n  method: patch\n  operationId: patchResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{repository}/{id}\n  method: delete\n  operationId: deleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{repository}/search\n  method: get\n  operationId: listSearchMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}/search/{method}\n  method: get\n  operationId: executeSearchMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}/{id}/{association}\n  method: get\n  operationId: getAssociation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repository}/{id}/{association}\n  method: put\n  operationId: setAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{repository}/{id}/{association}\n  method: delete\n  operationId: deleteAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-data/refs/heads/main/agentic-access/spring-data-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Data Access
- Database
- Framework
- Java
- JPA
- MongoDB
- ORM
- Redis
- REST
- Spring
---
