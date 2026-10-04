---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: aylien-absa-api-openapi.yml
  format: yaml
  label: AYLIEN Absa API
  slug: aylien-absa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-absa-api-openapi.yml
- filename: aylien-autocomplete-api-openapi.yml
  format: yaml
  label: AYLIEN Autocomplete API
  slug: aylien-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-autocomplete-api-openapi.yml
- filename: aylien-classify-api-openapi.yml
  format: yaml
  label: AYLIEN Classify API
  slug: aylien-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-classify-api-openapi.yml
- filename: aylien-cluster-api-openapi.yml
  format: yaml
  label: AYLIEN Cluster API
  slug: aylien-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-cluster-api-openapi.yml
- filename: aylien-concepts-api-openapi.yml
  format: yaml
  label: AYLIEN Concepts API
  slug: aylien-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-concepts-api-openapi.yml
- filename: aylien-elsa-api-openapi.yml
  format: yaml
  label: AYLIEN Elsa API
  slug: aylien-elsa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-elsa-api-openapi.yml
- filename: aylien-entities-api-openapi.yml
  format: yaml
  label: AYLIEN Entities API
  slug: aylien-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-entities-api-openapi.yml
- filename: aylien-extract-api-openapi.yml
  format: yaml
  label: AYLIEN Extract API
  slug: aylien-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-extract-api-openapi.yml
- filename: aylien-hashtags-api-openapi.yml
  format: yaml
  label: AYLIEN Hashtags API
  slug: aylien-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-hashtags-api-openapi.yml
- filename: aylien-histogram-api-openapi.yml
  format: yaml
  label: AYLIEN Histogram API
  slug: aylien-histogram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-histogram-api-openapi.yml
- filename: aylien-language-api-openapi.yml
  format: yaml
  label: AYLIEN Language API
  slug: aylien-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-language-api-openapi.yml
- filename: aylien-related-story-api-openapi.yml
  format: yaml
  label: AYLIEN Related Story API
  slug: aylien-related-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-related-story-api-openapi.yml
- filename: aylien-sentiment-api-openapi.yml
  format: yaml
  label: AYLIEN Sentiment API
  slug: aylien-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-sentiment-api-openapi.yml
- filename: aylien-story-api-openapi.yml
  format: yaml
  label: AYLIEN Story API
  slug: aylien-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-story-api-openapi.yml
- filename: aylien-summarize-api-openapi.yml
  format: yaml
  label: AYLIEN Summarize API
  slug: aylien-summarize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-summarize-api-openapi.yml
- filename: aylien-time-series-api-openapi.yml
  format: yaml
  label: AYLIEN Time Series API
  slug: aylien-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-time-series-api-openapi.yml
- filename: aylien-trends-api-openapi.yml
  format: yaml
  label: AYLIEN Trends API
  slug: aylien-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-trends-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aylien Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'AYLIEN exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AYLIEN
provider_slug: aylien
slug: aylien-agentic-access
source_filename: aylien-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/aylien-absa-api-openapi.yml, openapi/aylien-autocomplete-api-openapi.yml, openapi/aylien-classify-api-openapi.yml,\n  openapi/aylien-cluster-api-openapi.yml, openapi/aylien-concepts-api-openapi.yml, openapi/aylien-elsa-api-openapi.yml,\n  openapi/aylien-entities-api-openapi.yml, openapi/aylien-extract-api-openapi.yml, openapi/aylien-hashtags-api-openapi.yml,\n  openapi/aylien-histogram-api-openapi.yml, openapi/aylien-language-api-openapi.yml, openapi/aylien-related-story-api-openapi.yml,\n  openapi/aylien-sentiment-api-openapi.yml, openapi/aylien-story-api-openapi.yml, openapi/aylien-summarize-api-openapi.yml,\n  openapi/aylien-time-series-api-openapi.yml, openapi/aylien-trends-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /absa\n  method: get\n  operationId: aspectSentiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompletes\n  method: get\n  operationId: listAutocompletes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classify/iptc-subjectcode\n  method: get\n  operationId: classifyIPTC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classify/iab-qag\n  method: get\n  operationId: classifyIAB\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concepts\n  method: get\n  operationId: concepts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elsa\n  method: get\n  operationId: entitySentiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: get\n  operationId: entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract\n  method: get\n  operationId: extractArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /hashtags\n  method: get\n  operationId: hashtags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /histograms\n  method: get\n  operationId: listHistograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /language\n  method: get\n  operationId: language\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related_stories\n  method: post\n  operationId: listRelatedStoriesPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related_stories\n  method: get\n  operationId: listRelatedStoriesGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sentiment\n  method: get\n  operationId: documentSentiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories\n  method: get\n  operationId: listStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories\n  method: post\n  operationId: advancedListStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize\n  method: get\n  operationId: summarize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_series\n  method:\
  \ get\n  operationId: listTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trends\n  method: get\n  operationId: listTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/agentic-access/aylien-agentic-access.yml
summary_line: 20 operations
tags:
- News Intelligence
- Text Analysis
- NLP
- Sentiment Analysis
- Entity Recognition
- Natural Language Processing
- News API
- Article Extraction
- Summarization
- Concept Detection
---
