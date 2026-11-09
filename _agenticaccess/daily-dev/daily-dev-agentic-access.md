---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 35
api_specs:
- filename: daily-dev-bookmarks-api-openapi.yml
  format: yaml
  label: daily-dev Bookmarks API
  slug: daily-dev-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-bookmarks-api-openapi.yml
- filename: daily-dev-custom-feeds-api-openapi.yml
  format: yaml
  label: daily-dev Custom Feeds API
  slug: daily-dev-custom-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-custom-feeds-api-openapi.yml
- filename: daily-dev-experiences-api-openapi.yml
  format: yaml
  label: daily-dev Experiences API
  slug: daily-dev-experiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-experiences-api-openapi.yml
- filename: daily-dev-feed-filters-api-openapi.yml
  format: yaml
  label: daily-dev Feed Filters API
  slug: daily-dev-feed-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-feed-filters-api-openapi.yml
- filename: daily-dev-feeds-api-openapi.yml
  format: yaml
  label: daily-dev Feeds API
  slug: daily-dev-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-feeds-api-openapi.yml
- filename: daily-dev-for-you-api-openapi.yml
  format: yaml
  label: daily-dev For You API
  slug: daily-dev-for-you-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-for-you-api-openapi.yml
- filename: daily-dev-notifications-api-openapi.yml
  format: yaml
  label: daily-dev Notifications API
  slug: daily-dev-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-notifications-api-openapi.yml
- filename: daily-dev-plugins-api-openapi.yml
  format: yaml
  label: daily-dev Plugins API
  slug: daily-dev-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-plugins-api-openapi.yml
- filename: daily-dev-posts-api-openapi.yml
  format: yaml
  label: daily-dev Posts API
  slug: daily-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-posts-api-openapi.yml
- filename: daily-dev-profile-api-openapi.yml
  format: yaml
  label: daily-dev Profile API
  slug: daily-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-profile-api-openapi.yml
- filename: daily-dev-recommend-api-openapi.yml
  format: yaml
  label: daily-dev Recommend API
  slug: daily-dev-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-recommend-api-openapi.yml
- filename: daily-dev-search-api-openapi.yml
  format: yaml
  label: daily-dev Search API
  slug: daily-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-search-api-openapi.yml
- filename: daily-dev-stack-api-openapi.yml
  format: yaml
  label: daily-dev Stack API
  slug: daily-dev-stack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-stack-api-openapi.yml
- filename: daily-dev-tags-api-openapi.yml
  format: yaml
  label: daily-dev Tags API
  slug: daily-dev-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-tags-api-openapi.yml
consequence_counts:
  physical: 1
  read: 35
  safety-critical: 3
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Daily Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /feeds/foryou/learned
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /feeds/foryou/ranking
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /feeds/foryou/seen
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /profile/stack/reorder
operation_count: 83
overview: 'daily-dev exposes 83 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 44 write, 1 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: daily-dev
provider_slug: daily-dev
slug: daily-dev-agentic-access
source_filename: daily-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/daily-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 83\n  by_action_class:\n    connected: 35\n    acting: 48\n  by_consequence:\n    read: 35\n    write: 44\n    safety-critical: 3\n    physical: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /feeds/foryou\n  method: get\n  operationId: getFeedsForyou\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/popular\n  method: get\n  operationId: getFeedsPopular\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/discussed\n  method: get\n  operationId: getFeedsDiscussed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/tag/{tag}\n  method: get\n  operationId: getFeedsTagTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/source/{source}\n  method: get\n  operationId: getFeedsSourceSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/{id}\n  method: get\n  operationId: getPostsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /posts/{id}/comments\n  method: get\n  operationId: getPostsIdComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/posts\n  method: get\n  operationId: getSearchPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/tags\n  method: get\n  operationId: getSearchTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/sources\n  method: get\n  operationId: getSearchSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /bookmarks/\n  method: get\n  operationId: getBookmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookmarks/\n  method: post\n  operationId: postBookmarks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookmarks/search\n  method: get\n  operationId: getBookmarksSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookmarks/lists\n  method: get\n  operationId: getBookmarksLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookmarks/lists\n  method: post\n  operationId: postBookmarksLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookmarks/lists/{id}\n  method: delete\n  operationId: deleteBookmarksListsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookmarks/{id}\n  method: delete\n  operationId: deleteBookmarksId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookmarks/{id}\n  method: patch\n  operationId: patchBookmarksId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/custom/advanced-settings\n  method: get\n  operationId: getFeedsCustomAdvancedSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/custom/\n  method: post\n  operationId: postFeedsCustom\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/custom/\n  method: get\n  operationId: getFeedsCustom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/custom/{feedId}\n  method: get\n  operationId: getFeedsCustomFeedId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/custom/{feedId}\n  method: patch\n  operationId: patchFeedsCustomFeedId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/custom/{feedId}\n  method: delete\n  operationId: deleteFeedsCustomFeedId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/custom/{feedId}/info\n  method: get\n  operationId: getFeedsCustomFeedIdInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/custom/{feedId}/advanced\n  method: patch\n  operationId: patchFeedsCustomFeedIdAdvanced\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/\n  method: get\n  operationId: getFeedsFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/filters/tags/follow\n  method: post\n  operationId: postFeedsFiltersTagsFollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/tags/unfollow\n  method: post\n  operationId: postFeedsFiltersTagsUnfollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/tags/block\n  method: post\n  operationId: postFeedsFiltersTagsBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/tags/unblock\n  method: post\n  operationId: postFeedsFiltersTagsUnblock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /feeds/filters/sources/follow\n  method: post\n  operationId: postFeedsFiltersSourcesFollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/sources/unfollow\n  method: post\n  operationId: postFeedsFiltersSourcesUnfollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/sources/block\n  method: post\n  operationId: postFeedsFiltersSourcesBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/sources/unblock\n  method: post\n  operationId: postFeedsFiltersSourcesUnblock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}\n  method: get\n  operationId: getFeedsFiltersFeedId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/filters/{feedId}/tags/follow\n  method: post\n  operationId: postFeedsFiltersFeedIdTagsFollow\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/tags/unfollow\n  method: post\n  operationId: postFeedsFiltersFeedIdTagsUnfollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/tags/block\n  method: post\n  operationId: postFeedsFiltersFeedIdTagsBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/tags/unblock\n  method: post\n  operationId: postFeedsFiltersFeedIdTagsUnblock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/sources/follow\n  method: post\n  operationId: postFeedsFiltersFeedIdSourcesFollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/sources/unfollow\n\
  \  method: post\n  operationId: postFeedsFiltersFeedIdSourcesUnfollow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/sources/block\n  method: post\n  operationId: postFeedsFiltersFeedIdSourcesBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/filters/{feedId}/sources/unblock\n  method: post\n  operationId: postFeedsFiltersFeedIdSourcesUnblock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/profile\n  method: get\n  operationId: getFeedsForyouProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/foryou/controls\n  method: get\n  operationId: getFeedsForyouControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/foryou/left-out\n  method: get\n  operationId: getFeedsForyouLeftOut\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/foryou/posts/{id}/explanation\n\
  \  method: get\n  operationId: getFeedsForyouPostsIdExplanation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/foryou/topics/mode\n  method: post\n  operationId: postFeedsForyouTopicsMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/topics/weight\n  method: post\n  operationId: postFeedsForyouTopicsWeight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /feeds/foryou/sources/mode\n  method: post\n  operationId: postFeedsForyouSourcesMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/sources/weight\n  method: post\n  operationId: postFeedsForyouSourcesWeight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/authors/mode\n  method: post\n  operationId: postFeedsForyouAuthorsMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/authors/weight\n  method: post\n  operationId: postFeedsForyouAuthorsWeight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/ranking\n  method: post\n  operationId: postFeedsForyouRanking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /feeds/foryou/ranking\n  method: delete\n  operationId: deleteFeedsForyouRanking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /feeds/foryou/learning\n  method: post\n  operationId: postFeedsForyouLearning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/fill-ins\n  method: post\n  operationId: postFeedsForyouFillIns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/foryou/learned\n  method: delete\n  operationId: deleteFeedsForyouLearned\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /feeds/foryou/seen\n  method: delete\n  operationId: deleteFeedsForyouSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /notifications/\n  method: get\n  operationId: getNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/unread/count\n  method: get\n  operationId: getNotificationsUnreadCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/read\n  method: post\n  operationId: postNotificationsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/\n  method: get\n  operationId:\
  \ getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/\n  method: patch\n  operationId: patchProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/stack/search\n  method: get\n  operationId: getProfileStackSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/stack/\n  method: get\n  operationId: getProfileStack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/stack/\n  method: post\n  operationId: postProfileStack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/stack/{id}\n  method: patch\n  operationId: patchProfileStackId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/stack/{id}\n  method: delete\n  operationId: deleteProfileStackId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/stack/reorder\n  method: put\n  operationId: putProfileStackReorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/experiences/\n  method: get\n  operationId: getProfileExperiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/experiences/\n  method: post\n  operationId: postProfileExperiences\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/experiences/{id}\n  method: get\n  operationId: getProfileExperiencesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/experiences/{id}\n  method: put\n  operationId: putProfileExperiencesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/experiences/{id}\n  method: delete\n  operationId:\
  \ deleteProfileExperiencesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommend/keyword\n  method: get\n  operationId: getRecommendKeyword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommend/semantic\n  method: get\n  operationId: getRecommendSemantic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugins/\n  method: get\n  operationId: getPlugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugins/\n  method: post\n  operationId: postPlugins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plugins/{id}\n  method: get\n  operationId: getPluginsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugins/{id}\n  method: put\n  operationId: putPluginsId\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/daily-dev/agentic-access/daily-dev-agentic-access.yml
summary_line: 83 operations · 48 acting · 3 human-in-the-loop
tags:
- Company
- Developer Tools
- NewsAggregator
- Artificial Intelligence
- Community
---
