---
acting_count: 0
action_class_counts:
  connected: 18
api_specs:
- filename: library-of-congress-bills-api-openapi.yml
  format: yaml
  label: Library of Congress Bills API
  slug: library-of-congress-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-bills-api-openapi.yml
- filename: library-of-congress-collections-api-openapi.yml
  format: yaml
  label: Library of Congress Collections API
  slug: library-of-congress-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-collections-api-openapi.yml
- filename: library-of-congress-committees-api-openapi.yml
  format: yaml
  label: Library of Congress Committees API
  slug: library-of-congress-committees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-committees-api-openapi.yml
- filename: library-of-congress-congressional-record-api-openapi.yml
  format: yaml
  label: Library of Congress Congressional Record API
  slug: library-of-congress-congressional-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-congressional-record-api-openapi.yml
- filename: library-of-congress-issues-api-openapi.yml
  format: yaml
  label: Library of Congress Issues API
  slug: library-of-congress-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-issues-api-openapi.yml
- filename: library-of-congress-items-api-openapi.yml
  format: yaml
  label: Library of Congress Items API
  slug: library-of-congress-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-items-api-openapi.yml
- filename: library-of-congress-laws-api-openapi.yml
  format: yaml
  label: Library of Congress Laws API
  slug: library-of-congress-laws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-laws-api-openapi.yml
- filename: library-of-congress-members-api-openapi.yml
  format: yaml
  label: Library of Congress Members API
  slug: library-of-congress-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-members-api-openapi.yml
- filename: library-of-congress-pages-api-openapi.yml
  format: yaml
  label: Library of Congress Pages API
  slug: library-of-congress-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-pages-api-openapi.yml
- filename: library-of-congress-resources-api-openapi.yml
  format: yaml
  label: Library of Congress Resources API
  slug: library-of-congress-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-resources-api-openapi.yml
- filename: library-of-congress-search-api-openapi.yml
  format: yaml
  label: Library of Congress Search API
  slug: library-of-congress-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-search-api-openapi.yml
- filename: library-of-congress-titles-api-openapi.yml
  format: yaml
  label: Library of Congress Titles API
  slug: library-of-congress-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-titles-api-openapi.yml
consequence_counts:
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Library Of Congress Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Library of Congress exposes 18 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Library of Congress
provider_slug: library-of-congress
slug: library-of-congress-agentic-access
source_filename: library-of-congress-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/library-of-congress-chronicling-america-api-openapi.yml, openapi/library-of-congress-congress-gov-api-openapi.yml,\n  openapi/library-of-congress-loc-gov-json-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 18\n  by_consequence:\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /search/pages/results/\n  method: get\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/titles/results/\n  method: get\n  operationId: searchTitles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lccn/{lccn}.json\n  method: get\n  operationId: getTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lccn/{lccn}/{date}/ed-{edition}.json\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newspapers.json\n  method: get\n  operationId: listNewspapers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bill\n  method: get\n  operationId: listBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bill/{congress}/{billType}\n\
  \  method: get\n  operationId: listBillsByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bill/{congress}/{billType}/{billNumber}\n  method: get\n  operationId: getBill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /member\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /member/{bioguideId}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /committee\n  method: get\n  operationId: listCommittees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /law/{congress}\n  method: get\n  operationId: listLaws\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congressional-record\n  method: get\n  operationId: listCongressionalRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/\n  method: get\n  operationId: searchAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{name}/\n  method: get\n  operationId: getCollection\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item/{itemId}/\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/{resourceId}/\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/agentic-access/library-of-congress-agentic-access.yml
summary_line: 18 operations
tags:
- Cultural Heritage
- Federal Government
- Library
- Legislative
- Newspapers
- Search
---
