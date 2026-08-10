---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 25
api_specs:
- filename: boundless-bio-comments-api-openapi.yml
  format: yaml
  label: Boundless Bio Comments API
  slug: boundless-bio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-comments-api-openapi.yml
- filename: boundless-bio-discovery-api-openapi.yml
  format: yaml
  label: Boundless Bio Discovery API
  slug: boundless-bio-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-discovery-api-openapi.yml
- filename: boundless-bio-leadership-api-openapi.yml
  format: yaml
  label: Boundless Bio Leadership API
  slug: boundless-bio-leadership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-leadership-api-openapi.yml
- filename: boundless-bio-media-api-openapi.yml
  format: yaml
  label: Boundless Bio Media API
  slug: boundless-bio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-media-api-openapi.yml
- filename: boundless-bio-pages-api-openapi.yml
  format: yaml
  label: Boundless Bio Pages API
  slug: boundless-bio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-pages-api-openapi.yml
- filename: boundless-bio-posts-api-openapi.yml
  format: yaml
  label: Boundless Bio Posts API
  slug: boundless-bio-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-posts-api-openapi.yml
- filename: boundless-bio-search-api-openapi.yml
  format: yaml
  label: Boundless Bio Search API
  slug: boundless-bio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-search-api-openapi.yml
- filename: boundless-bio-settings-api-openapi.yml
  format: yaml
  label: Boundless Bio Settings API
  slug: boundless-bio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-settings-api-openapi.yml
- filename: boundless-bio-taxonomy-api-openapi.yml
  format: yaml
  label: Boundless Bio Taxonomy API
  slug: boundless-bio-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-taxonomy-api-openapi.yml
- filename: boundless-bio-users-api-openapi.yml
  format: yaml
  label: Boundless Bio Users API
  slug: boundless-bio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-users-api-openapi.yml
consequence_counts:
  physical: 5
  read: 25
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boundless Bio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wp/v2/who-we-are
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wp/v2/who-we-are/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /wp/v2/who-we-are/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /wp/v2/who-we-are/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /wp/v2/who-we-are/{id}
operation_count: 73
overview: 'Boundless Bio exposes 73 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 43 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Boundless Bio
provider_slug: boundless-bio
slug: boundless-bio-agentic-access
source_filename: boundless-bio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: generated\nsource: openapi/boundless-bio-content-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    connected: 25\n    acting: 48\n  by_consequence:\n    read: 25\n    write: 43\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: post\n  operationId: createCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategoriesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: post\n  operationId: createCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: put\n  operationId: updateCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: patch\n  operationId: patchCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/categories/{id}\n  method: delete\n  operationId: deleteCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /wp/v2/comments\n  method: post\n  operationId: createComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getCommentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: post\n  operationId: createCommentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: put\n  operationId:\
  \ updateCommentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: patch\n  operationId: patchCommentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/comments/{id}\n  method: delete\n  operationId: deleteCommentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /wp/v2/media\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: post\n  operationId: createMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: post\n  operationId: createMediaById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: put\n  operationId: updateMediaById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: patch\n  operationId: patchMediaById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}\n  method: delete\n  operationId: deleteMediaById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/media/{id}/edit\n  method: post\n  operationId: createMediaByIdEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages\n  method: get\n  operationId: getPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: post\n  operationId: createPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: post\n  operationId: createPagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: put\n  operationId: updatePagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /wp/v2/pages/{id}\n  method: patch\n  operationId: patchPagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/pages/{id}\n  method: delete\n  operationId: deletePagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts\n  method: get\n  operationId: getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: post\n  operationId: createPosts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPostsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: post\n  operationId: createPostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: put\n  operationId: updatePostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: patch\n  operationId: patchPostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/posts/{id}\n  method: delete\n  operationId: deletePostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/search\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/settings\n  method: post\n  operationId: createSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/settings\n  method: put\n  operationId: updateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /wp/v2/settings\n  method: patch\n  operationId: patchSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/statuses\n  method: get\n  operationId: getStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatusesByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /wp/v2/tags\n  method: post\n  operationId: createTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTagsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: post\n  operationId: createTagsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: put\n  operationId: updateTagsById\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: patch\n  operationId: patchTagsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/tags/{id}\n  method: delete\n  operationId: deleteTagsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: getTaxonomies\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomiesByTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: getTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getTypesByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wp/v2/users\n  method: post\n  operationId: createUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: get\n  operationId: getUsersMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/me\n  method: post\n  operationId: createUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: put\n  operationId: updateUsersMe\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: patch\n  operationId: patchUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/me\n  method: delete\n  operationId: deleteUsersMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n\
  \  method: get\n  operationId: getUsersById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: post\n  operationId: createUsersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: put\n  operationId: updateUsersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: patch\n  operationId: patchUsersById\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/users/{id}\n  method: delete\n  operationId: deleteUsersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/who-we-are\n  method: get\n  operationId: getWhoWeAre\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/who-we-are\n  method: post\n  operationId: createWhoWeAre\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/who-we-are/{id}\n  method: get\n  operationId: getWhoWeAreById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/who-we-are/{id}\n  method: post\n  operationId: createWhoWeAreById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/who-we-are/{id}\n  method: put\n  operationId: updateWhoWeAreById\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/who-we-are/{id}\n  method: patch\n  operationId: patchWhoWeAreById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wp/v2/who-we-are/{id}\n  method: delete\n  operationId: deleteWhoWeAreById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/agentic-access/boundless-bio-agentic-access.yml
summary_line: 73 operations · 48 acting
tags:
- Company
- Biotechnology
- Oncology
- Precision Medicine
- Drug Discovery
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Genomics
- Diagnostics
- Research
- Content
---
