---
acting_count: 42
action_class_counts:
  acting: 42
  connected: 23
api_specs:
- filename: skydance-media-categories-api-openapi.yml
  format: yaml
  label: Skydance Media Categories API
  slug: skydance-media-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-categories-api-openapi.yml
- filename: skydance-media-comments-api-openapi.yml
  format: yaml
  label: Skydance Media Comments API
  slug: skydance-media-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-comments-api-openapi.yml
- filename: skydance-media-media-api-openapi.yml
  format: yaml
  label: Skydance Media Media API
  slug: skydance-media-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-media-api-openapi.yml
- filename: skydance-media-pages-api-openapi.yml
  format: yaml
  label: Skydance Media Pages API
  slug: skydance-media-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-pages-api-openapi.yml
- filename: skydance-media-posts-api-openapi.yml
  format: yaml
  label: Skydance Media Posts API
  slug: skydance-media-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-posts-api-openapi.yml
- filename: skydance-media-search-api-openapi.yml
  format: yaml
  label: Skydance Media Search API
  slug: skydance-media-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-search-api-openapi.yml
- filename: skydance-media-settings-api-openapi.yml
  format: yaml
  label: Skydance Media Settings API
  slug: skydance-media-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-settings-api-openapi.yml
- filename: skydance-media-statuses-api-openapi.yml
  format: yaml
  label: Skydance Media Statuses API
  slug: skydance-media-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-statuses-api-openapi.yml
- filename: skydance-media-tags-api-openapi.yml
  format: yaml
  label: Skydance Media Tags API
  slug: skydance-media-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-tags-api-openapi.yml
- filename: skydance-media-taxonomies-api-openapi.yml
  format: yaml
  label: Skydance Media Taxonomies API
  slug: skydance-media-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-taxonomies-api-openapi.yml
- filename: skydance-media-types-api-openapi.yml
  format: yaml
  label: Skydance Media Types API
  slug: skydance-media-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-types-api-openapi.yml
- filename: skydance-media-users-api-openapi.yml
  format: yaml
  label: Skydance Media Users API
  slug: skydance-media-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/openapi/skydance-media-users-api-openapi.yml
consequence_counts:
  read: 23
  write: 42
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Skydance Media Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 65
overview: 'Skydance Media exposes 65 API operations that an AI agent could call, of which 42 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 42 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Skydance Media
provider_slug: skydance-media
slug: skydance-media-agentic-access
source_filename: skydance-media-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/skydance-media-content-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 23\n    acting: 42\n  by_consequence:\n    read: 23\n    write: 42\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: post\n  operationId: createCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategoriesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: post\n  operationId: createCategoriesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: put\n  operationId: replaceCategoriesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: patch\n  operationId: updateCategoriesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: delete\n  operationId: deleteCategoriesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /wp/v2/comments\n  method: post\n  operationId: createComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getCommentsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: post\n  operationId: createCommentsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: put\n  operationId: replaceCommentsId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: patch\n  operationId: updateCommentsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: delete\n  operationId: deleteCommentsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /wp/v2/media\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: post\n  operationId: createMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: post\n  operationId: createMediaId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: put\n  operationId: replaceMediaId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: patch\n  operationId: updateMediaId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: delete\n  operationId: deleteMediaId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages\n  method: get\n  operationId: getPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: post\n  operationId: createPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPagesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: post\n  operationId: createPagesId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: put\n  operationId: replacePagesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: patch\n  operationId: updatePagesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n\
  \  method: delete\n  operationId: deletePagesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts\n  method: get\n  operationId: getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: post\n  operationId: createPosts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPostsId\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: post\n  operationId: createPostsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: put\n  operationId: replacePostsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: patch\n  operationId: updatePostsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: delete\n  operationId: deletePostsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/search\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/settings\n  method: post\n  operationId: createSettings\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/settings\n  method: put\n  operationId: replaceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/settings\n  method: patch\n  operationId: updateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/statuses\n  method: get\n  operationId:\
  \ getStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatusesStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: post\n  operationId: createTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTagsId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: post\n  operationId: createTagsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: put\n  operationId: replaceTagsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: patch\n  operationId: updateTagsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: delete\n  operationId: deleteTagsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: getTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomiesTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n\
  \  method: get\n  operationId: getTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getTypesType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: post\n  operationId: createUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: get\n\
  \  operationId: getUsersId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: post\n  operationId: createUsersId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: put\n  operationId: replaceUsersId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: patch\n  operationId: updateUsersId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: delete\n  operationId: deleteUsersId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: get\n  operationId: getUsersMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/me\n  method: post\n  operationId: createUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: put\n  operationId: replaceUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: patch\n  operationId: updateUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: delete\n  operationId: deleteUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/agentic-access/skydance-media-agentic-access.yml
summary_line: 65 operations · 42 acting
tags:
- Company
- Entertainment
- Media
- Film
- Television
- Animation
- Video Games
- Sports
- Content
- WordPress
---
