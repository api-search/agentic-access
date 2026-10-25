---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: trove-contributor-api-openapi.yml
  format: yaml
  label: Trove Contributor API
  slug: trove-contributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-contributor-api-openapi.yml
- filename: trove-list-api-openapi.yml
  format: yaml
  label: Trove List API
  slug: trove-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-list-api-openapi.yml
- filename: trove-newspaper-api-openapi.yml
  format: yaml
  label: Trove Newspaper API
  slug: trove-newspaper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-newspaper-api-openapi.yml
- filename: trove-people-api-openapi.yml
  format: yaml
  label: Trove People API
  slug: trove-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-people-api-openapi.yml
- filename: trove-search-api-openapi.yml
  format: yaml
  label: Trove Search API
  slug: trove-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-search-api-openapi.yml
- filename: trove-work-api-openapi.yml
  format: yaml
  label: Trove Work API
  slug: trove-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-work-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trove Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Trove exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trove
provider_slug: trove
slug: trove-agentic-access
source_filename: trove-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/trove-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/result\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/work/{workId}\n  method: get\n  operationId: getWork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/magazine/titles\n  method: get\n  operationId: findMagazineTitles\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/magazine/title/{id}\n  method: get\n  operationId: getMagazineTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/people/{id}\n  method: get\n  operationId: getPersonOrOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/list/{id}\n  method: get\n  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/newspaper/{id}\n  method: get\n  operationId: getNewspaperArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/newspaper/titles\n  method: get\n  operationId: findNewspaperTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/newspaper/title/{id}\n  method: get\n  operationId: getNewspaperTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/gazette/{id}\n  method: get\n  operationId: getGazetteArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/gazette/titles\n  method: get\n  operationId: findGazetteTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/gazette/title/{id}\n  method: get\n  operationId: getGazetteTitle\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/contributor\n  method: get\n  operationId: findContributors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/contributor/{id}\n  method: get\n  operationId: getContributor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/agentic-access/trove-agentic-access.yml
summary_line: 14 operations
tags:
- News
- Public APIs
- Libraries
- Cultural Heritage
- Digitised Newspapers
- Archives
- Open Data
- Australia
- Search
---
