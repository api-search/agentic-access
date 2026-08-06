---
acting_count: 0
action_class_counts:
  connected: 31
api_specs:
- filename: daring-foods-recipes-api-openapi.yml
  format: yaml
  label: Daring Foods Recipes API
  slug: daring-foods-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-recipes-api-openapi.yml
- filename: daring-foods-products-api-openapi.yml
  format: yaml
  label: Daring Foods Retail Products API
  slug: daring-foods-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-products-api-openapi.yml
- filename: daring-foods-foodservice-api-openapi.yml
  format: yaml
  label: Daring Foods Foodservice Products API
  slug: daring-foods-foodservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-foodservice-api-openapi.yml
- filename: daring-foods-pages-api-openapi.yml
  format: yaml
  label: Daring Foods Pages API
  slug: daring-foods-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-pages-api-openapi.yml
- filename: daring-foods-media-api-openapi.yml
  format: yaml
  label: Daring Foods Media API
  slug: daring-foods-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-media-api-openapi.yml
- filename: daring-foods-taxonomy-api-openapi.yml
  format: yaml
  label: Daring Foods Taxonomy API
  slug: daring-foods-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-taxonomy-api-openapi.yml
- filename: daring-foods-search-api-openapi.yml
  format: yaml
  label: Daring Foods Search API
  slug: daring-foods-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-search-api-openapi.yml
- filename: daring-foods-discovery-api-openapi.yml
  format: yaml
  label: Daring Foods Discovery API
  slug: daring-foods-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-discovery-api-openapi.yml
- filename: daring-foods-posts-api-openapi.yml
  format: yaml
  label: Daring Foods Posts API
  slug: daring-foods-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-posts-api-openapi.yml
- filename: daring-foods-oembed-api-openapi.yml
  format: yaml
  label: Daring Foods oEmbed API
  slug: daring-foods-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-oembed-api-openapi.yml
- filename: daring-foods-seo-api-openapi.yml
  format: yaml
  label: Daring Foods SEO Metadata API
  slug: daring-foods-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-seo-api-openapi.yml
consequence_counts:
  read: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Daring Foods Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Daring Foods exposes 31 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Daring Foods
provider_slug: daring-foods
slug: daring-foods-agentic-access
source_filename: daring-foods-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/daring-foods-discovery-api-openapi.yml, openapi/daring-foods-foodservice-api-openapi.yml,\n  openapi/daring-foods-media-api-openapi.yml, openapi/daring-foods-oembed-api-openapi.yml, openapi/daring-foods-pages-api-openapi.yml,\n  openapi/daring-foods-posts-api-openapi.yml, openapi/daring-foods-products-api-openapi.yml,\n  openapi/daring-foods-recipes-api-openapi.yml, openapi/daring-foods-search-api-openapi.yml,\n  openapi/daring-foods-seo-api-openapi.yml, openapi/daring-foods-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 31\n  by_consequence:\n    read: 31\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method:\
  \ get\n  operationId: getRouteIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2\n  method: get\n  operationId: getWpV2Namespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listPostTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getPostType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/foodservice-products\n  method: get\n  operationId: listFoodserviceProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/foodservice-products/{id}\n  method: get\n  operationId: getFoodserviceProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/recipes\n  method: get\n  operationId:\
  \ listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/recipes/{id}\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchSiteContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/agentic-access/daring-foods-agentic-access.yml
summary_line: 31 operations
tags:
- Company
- Food
- Consumer Packaged Goods
- Plant Based
- Alternative Protein
- Food and Beverage
- Recipes
- Foodservice
- Grocery
- Content
---
