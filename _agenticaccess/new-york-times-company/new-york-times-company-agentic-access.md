---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: article-search-v2-openapi.yml
  format: yaml
  label: Article Search API
  slug: article-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/article-search-v2-openapi.yml
- filename: top-stories-v2-openapi.yml
  format: yaml
  label: Top Stories API
  slug: top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/top-stories-v2-openapi.yml
- filename: most-popular-api-v2-openapi.yml
  format: yaml
  label: Most Popular API
  slug: most-popular-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/most-popular-api-v2-openapi.yml
- filename: timeswire-v3-openapi.yml
  format: yaml
  label: Times Newswire API
  slug: times-newswire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/timeswire-v3-openapi.yml
- filename: archive-api-openapi.yml
  format: yaml
  label: Archive API
  slug: archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/archive-api-openapi.yml
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/books-api-openapi.yml
- filename: movie-reviews-v2-openapi.yml
  format: yaml
  label: Movie Reviews API
  slug: movie-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/movie-reviews-v2-openapi.yml
- filename: times-tags-v3-openapi.yml
  format: yaml
  label: TimesTags API
  slug: timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/times-tags-v3-openapi.yml
- filename: semantic-api-openapi.yml
  format: yaml
  label: Semantic API
  slug: semantic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/semantic-api-openapi.yml
- filename: geo-api-v2-openapi.yml
  format: yaml
  label: Geographic API
  slug: geographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/geo-api-v2-openapi.yml
- filename: community-api-v3-openapi.yml
  format: yaml
  label: Community API (Deprecated)
  slug: community-api-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/community-api-v3-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: New York Times Company Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'The New York Times Company exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The New York Times Company
provider_slug: new-york-times-company
slug: new-york-times-company-agentic-access
source_filename: new-york-times-company-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/archive-api-openapi.yml, openapi/article-search-v2-openapi.yml, openapi/books-api-openapi.yml,\n  openapi/community-api-v3-openapi.yml, openapi/geo-api-v2-openapi.yml, openapi/most-popular-api-v2-openapi.yml,\n  openapi/movie-reviews-v2-openapi.yml, openapi/semantic-api-openapi.yml, openapi/times-tags-v3-openapi.yml,\n  openapi/timeswire-v3-openapi.yml, openapi/top-stories-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /{year}/{month}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articlesearch.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists.json\n  method: get\n  operationId: GET_lists-format\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{date}/{list}.json\n  method: get\n  operationId: GET_lists-date-list-json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/overview.json\n  method: get\n  operationId: GET_lists-overview-format\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/names.json\n  method: get\n  operationId: GET_lists-names-format\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/best-sellers/history.json\n  method: get\n  operationId: GET_lists-best-sellers-history-json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews.json\n  method: get\n  operationId: GET_reviews-format\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-content/recent.json\n  method: get\n  operationId: GET_user-content-recent-json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-content/url.json\n  method: get\n  operationId: GET_user-content-url-json\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-content/by-date.json\n  method: get\n  operationId: GET_user-content-by-date-json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-content/user.json\n  method: get\n  operationId: GET_user-content-user-json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailed/{period}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shared/{period}.json\n  method: get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shared/{period}/{share_type}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewed/{period}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /critics/{reviewer}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews/{type}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews/search.json\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /name/{concept-type}/{specific-concept}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timestags\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{source}/{section}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{source}/{section}/{time-period}.json\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{section}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/agentic-access/new-york-times-company-agentic-access.yml
summary_line: 27 operations
tags:
- News
- Media
- Publishing
- Newspapers
- Articles
- Books
- Movies
- Sports
- Games
- Cooking
- Reviews
- Search
- Semantic
- Tagging
- Controlled Vocabulary
- Geographic
- Archive
---
