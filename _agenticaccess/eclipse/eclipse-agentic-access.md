---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: eclipse-eclipse-marketplace-rest-api-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Eclipse Marketplace REST API API
  slug: eclipse-eclipse-marketplace-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-eclipse-marketplace-rest-api-api-openapi.yml
- filename: eclipse-favorites-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Favorites API
  slug: eclipse-favorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-favorites-api-openapi.yml
- filename: eclipse-featured-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Featured API
  slug: eclipse-featured-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-featured-api-openapi.yml
- filename: eclipse-node-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Node API
  slug: eclipse-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-node-api-openapi.yml
- filename: eclipse-popular-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Popular API
  slug: eclipse-popular-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-popular-api-openapi.yml
- filename: eclipse-recent-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Recent API
  slug: eclipse-recent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-recent-api-openapi.yml
- filename: eclipse-search-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Search API
  slug: eclipse-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-search-api-openapi.yml
- filename: eclipse-taxonomy-api-openapi.yml
  format: yaml
  label: Eclipse Foundation Taxonomy API
  slug: eclipse-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/openapi/eclipse-taxonomy-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eclipse Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Eclipse Foundation exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eclipse Foundation
provider_slug: eclipse
slug: eclipse-agentic-access
source_filename: eclipse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/eclipse-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: listMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /node/{nodeId}\n  method: get\n  operationId: getNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxonomy/term/{ids}\n  method: get\n  operationId: getTaxonomyTerm\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/apachesolr_search/{term}\n  method: get\n  operationId: searchListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /favorites/top\n  method: get\n  operationId: getTopFavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /popular/top\n  method: get\n  operationId: getTopPopular\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recent\n  method: get\n  operationId: getRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /featured\n  method: get\n  operationId: getFeatured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/agentic-access/eclipse-agentic-access.yml
summary_line: 8 operations
tags:
- Eclipse Foundation
- Foundation
- Open Source
- Standards
---
