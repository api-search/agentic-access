---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: abcuro-careers-api-openapi.yml
  format: yaml
  label: Abcuro Careers API
  slug: abcuro-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-careers-api-openapi.yml
- filename: abcuro-comments-api-openapi.yml
  format: yaml
  label: Abcuro Comments API
  slug: abcuro-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-comments-api-openapi.yml
- filename: abcuro-discovery-api-openapi.yml
  format: yaml
  label: Abcuro Discovery API
  slug: abcuro-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-discovery-api-openapi.yml
- filename: abcuro-investors-api-openapi.yml
  format: yaml
  label: Abcuro Investors API
  slug: abcuro-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-investors-api-openapi.yml
- filename: abcuro-media-api-openapi.yml
  format: yaml
  label: Abcuro Media API
  slug: abcuro-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-media-api-openapi.yml
- filename: abcuro-pages-api-openapi.yml
  format: yaml
  label: Abcuro Pages API
  slug: abcuro-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-pages-api-openapi.yml
- filename: abcuro-people-api-openapi.yml
  format: yaml
  label: Abcuro People API
  slug: abcuro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-people-api-openapi.yml
- filename: abcuro-press-releases-api-openapi.yml
  format: yaml
  label: Abcuro Press Releases API
  slug: abcuro-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-press-releases-api-openapi.yml
- filename: abcuro-publications-api-openapi.yml
  format: yaml
  label: Abcuro Publications API
  slug: abcuro-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-publications-api-openapi.yml
- filename: abcuro-search-api-openapi.yml
  format: yaml
  label: Abcuro Search API
  slug: abcuro-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-search-api-openapi.yml
- filename: abcuro-taxonomy-api-openapi.yml
  format: yaml
  label: Abcuro Taxonomy API
  slug: abcuro-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-taxonomy-api-openapi.yml
- filename: abcuro-users-api-openapi.yml
  format: yaml
  label: Abcuro Users API
  slug: abcuro-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-users-api-openapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abcuro Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Abcuro exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abcuro
provider_slug: abcuro
slug: abcuro-agentic-access
source_filename: abcuro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/abcuro-content-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMediaItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n\
  \  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/person_role\n  method: get\n  operationId: listPersonRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/person_role/{id}\n  method: get\n  operationId: getPersonRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_people/{id}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_investors\n  method: get\n  operationId: listInvestors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_investors/{id}\n  method: get\n  operationId: getInvestor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_pubs\n  method: get\n  operationId:\
  \ listPublications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_pubs/{id}\n  method: get\n  operationId: getPublication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/abcuro_jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/agentic-access/abcuro-agentic-access.yml
summary_line: 30 operations
tags:
- biotechnology
- pharmaceuticals
- immunology
- autoimmune-disease
- oncology
- clinical-trials
- life-sciences
- drug-development
- healthcare
- content-api
- wordpress
---
