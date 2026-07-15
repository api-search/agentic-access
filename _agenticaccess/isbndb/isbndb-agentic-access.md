---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 15
api_specs:
- filename: doc.json
  format: json
  label: ISBNdb API
  slug: isbndb-api
  spec_type: OpenAPI
  url: https://api2.isbndb.com/doc.json
consequence_counts:
  read: 15
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Isbndb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'ISBNdb exposes 16 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ISBNdb
provider_slug: isbndb
slug: isbndb-agentic-access
source_filename: isbndb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 15\n    acting: 1\n  by_consequence:\n    read: 15\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /author/{name}\n  method: get\n  operationId: get_app_api_author_authordetails__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authors/{query}\n  method: get\n  operationId: get_app_api_author_searchauthors__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /book/{isbn}\n  method: get\n  operationId: get_app_api_book_book__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /books\n  method: post\n  operationId: post_app_api_book_bookmultiple__invoke\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /books/{query}\n  method: get\n  operationId: get_app_api_book_searchbook__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/books/updates\n  method: get\n  operationId: get_app_api_feed_updatedbooks__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /key\n  method: get\n  operationId: get_app_api_key__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{name}\n  method: get\n  operationId: get_app_api_publisher_publisherdetails__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{query}\n  method: get\n  operationId: get_app_api_publisher_searchpublishers__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/authors\n  method: get\n  operationId: get_app_api_search_searchauthors__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /search/books\n  method: get\n  operationId: get_app_api_search_searchbooks__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/publishers\n  method: get\n  operationId: get_app_api_search_searchpublishers__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/subjects\n  method: get\n  operationId: get_app_api_search_searchsubjects__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: get_app_api_stats_getstats__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /subjects/{query}\n  method: get\n  operationId: get_app_api_subject_searchsubjects__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subject/{name}\n  method: get\n  operationId: get_app_api_subject_subjectsdetails__invoke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/agentic-access/isbndb-agentic-access.yml
summary_line: 16 operations · 1 acting
tags:
- Books
- ISBN
- Publishing
- Metadata
- Library
- Bibliography
---
