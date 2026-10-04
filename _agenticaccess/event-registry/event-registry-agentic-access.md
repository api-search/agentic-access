---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 9
api_specs:
- filename: event-registry-articles-api-openapi.yml
  format: yaml
  label: Event Registry Articles API
  slug: event-registry-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-articles-api-openapi.yml
- filename: event-registry-events-api-openapi.yml
  format: yaml
  label: Event Registry Events API
  slug: event-registry-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-events-api-openapi.yml
- filename: event-registry-suggest-api-openapi.yml
  format: yaml
  label: Event Registry Suggest API
  slug: event-registry-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-suggest-api-openapi.yml
- filename: event-registry-topic-pages-api-openapi.yml
  format: yaml
  label: Event Registry Topic Pages API
  slug: event-registry-topic-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-topic-pages-api-openapi.yml
- filename: event-registry-usage-api-openapi.yml
  format: yaml
  label: Event Registry Usage API
  slug: event-registry-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-usage-api-openapi.yml
consequence_counts:
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Event Registry Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Event Registry exposes 14 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Event Registry
provider_slug: event-registry
slug: event-registry-agentic-access
source_filename: event-registry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/event-registry-articles-api-openapi.yml, openapi/event-registry-events-api-openapi.yml,\n  openapi/event-registry-suggest-api-openapi.yml, openapi/event-registry-topic-pages-api-openapi.yml,\n  openapi/event-registry-usage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 9\n    acting: 5\n  by_consequence:\n    read: 9\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /article/getArticles\n  method: post\n  operationId: searchArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article/getArticle\n  method:\
  \ post\n  operationId: getArticleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article/getArticlesForTopicPage\n  method: post\n  operationId: getTopicPageArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/getEvents\n  method: post\n  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/getEvent\n  method: post\n  operationId: getEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/getEventsForTopicPage\n  method: post\n  operationId: getTopicPageEvents\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggestConceptsFast\n  method: post\n  operationId: suggestConcepts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suggestCategoriesFast\n  method: post\n  operationId: suggestCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suggestSourcesFast\n  method: post\n  operationId: suggestSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suggestLocationsFast\n  method: post\n  operationId: suggestLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suggestAuthorsFast\n  method: post\n  operationId: suggestAuthors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /article/getArticlesForTopicPage\n  method: post\n  operationId: getTopicPageArticles\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/getEventsForTopicPage\n  method: post\n  operationId: getTopicPageEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: post\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/agentic-access/event-registry-agentic-access.yml
summary_line: 14 operations · 5 acting
tags:
- News
- Media Monitoring
- News Intelligence
- Event Detection
- Named Entity Recognition
- Sentiment Analysis
- Media Analytics
- News API
---
