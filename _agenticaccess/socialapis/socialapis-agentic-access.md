---
acting_count: 0
action_class_counts:
  connected: 53
api_specs:
- filename: socialapis-account-api-openapi.yml
  format: yaml
  label: SocialAPIs Account API
  slug: socialapis-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-account-api-openapi.yml
- filename: socialapis-facebook-groups-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Groups API
  slug: socialapis-facebook-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-groups-api-openapi.yml
- filename: socialapis-facebook-marketplace-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Marketplace API
  slug: socialapis-facebook-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-marketplace-api-openapi.yml
- filename: socialapis-facebook-media-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Media API
  slug: socialapis-facebook-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-media-api-openapi.yml
- filename: socialapis-facebook-pages-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Pages API
  slug: socialapis-facebook-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-pages-api-openapi.yml
- filename: socialapis-facebook-posts-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Posts API
  slug: socialapis-facebook-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-posts-api-openapi.yml
- filename: socialapis-facebook-search-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Search API
  slug: socialapis-facebook-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-search-api-openapi.yml
- filename: socialapis-instagram-api-openapi.yml
  format: yaml
  label: SocialAPIs Instagram API
  slug: socialapis-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-instagram-api-openapi.yml
- filename: socialapis-meta-ads-library-api-openapi.yml
  format: yaml
  label: SocialAPIs Meta Ads Library API
  slug: socialapis-meta-ads-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-meta-ads-library-api-openapi.yml
- filename: socialapis-other-api-openapi.yml
  format: yaml
  label: SocialAPIs Other API
  slug: socialapis-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-other-api-openapi.yml
consequence_counts:
  read: 53
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Socialapis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'SocialAPIs exposes 53 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SocialAPIs
provider_slug: socialapis
slug: socialapis-agentic-access
source_filename: socialapis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/socialapis-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 53\n  by_consequence:\n    read: 53\n  human_in_the_loop_required: 0\noperations:\n- path: /facebook/pages/id\n  method: get\n  operationId: facebook_get_page_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/pages/details\n  method: get\n  operationId: facebook_get_page_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/pages/posts\n  method:\
  \ get\n  operationId: facebook_get_page_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/pages/reels\n  method: get\n  operationId: facebook_get_page_reels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/pages/videos\n  method: get\n  operationId: facebook_get_page_videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/pages/albums\n  method: get\n  operationId: facebook_get_page_albums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/groups/id\n  method: get\n  operationId: facebook_get_group_id\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/groups/details\n  method: get\n  operationId: facebook_get_group_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/groups/posts\n  method: get\n  operationId: facebook_get_group_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/groups/videos\n  method: get\n  operationId: facebook_get_group_videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/groups/albums\n  method: get\n  operationId: facebook_get_group_albums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/albums/items\n  method: get\n  operationId: facebook_get_album_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/id\n  method: get\n  operationId: facebook_get_post_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/details\n  method: get\n  operationId: facebook_get_post_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/details/extended\n  method: get\n  operationId: facebook_get_post_details_extended\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /facebook/posts/attachments\n  method: get\n  operationId: facebook_get_post_attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/video\n  method: get\n  operationId: facebook_get_video_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/comments\n  method: get\n  operationId: facebook_get_post_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/posts/comments/replies\n  method: get\n  operationId: facebook_get_comment_replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/search/pages\n\
  \  method: get\n  operationId: facebook_search_pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/search/people\n  method: get\n  operationId: facebook_search_people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/search/locations\n  method: get\n  operationId: facebook_search_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/search/posts\n  method: get\n  operationId: facebook_search_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/search/videos\n  method: get\n  operationId: facebook_search_videos\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/ads/countries\n  method: get\n  operationId: facebook_ads_countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/ads/search\n  method: get\n  operationId: facebook_ads_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/ads/page-details\n  method: get\n  operationId: facebook_ads_page_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/ads/archive-details\n  method: get\n  operationId: facebook_ads_archive_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/ads/keywords\n  method: get\n  operationId: facebook_ads_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/search\n  method: get\n  operationId: facebook_marketplace_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/listing\n  method: get\n  operationId: facebook_marketplace_listing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/seller\n  method: get\n  operationId: facebook_marketplace_seller\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/categories\n  method: get\n  operationId: facebook_marketplace_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/city-coordinates\n  method: get\n  operationId: facebook_marketplace_city_coordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/vehicles\n  method: get\n  operationId: facebook_marketplace_vehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/marketplace/rentals\n  method: get\n  operationId: facebook_marketplace_rentals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /facebook/media/download\n  method: get\n  operationId: facebook_download_media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/user/id\n  method: get\n  operationId: instagram_get_user_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/profile/details\n  method: get\n  operationId: instagram_get_profile_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/profile/posts\n  method: get\n  operationId: instagram_get_profile_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/profile/reels\n\
  \  method: get\n  operationId: instagram_get_profile_reels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/profile/highlights\n  method: get\n  operationId: instagram_get_profile_highlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/highlight/details\n  method: get\n  operationId: instagram_get_highlight_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/post/id\n  method: get\n  operationId: instagram_get_post_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/post/details\n  method: get\n  operationId: instagram_get_post_details\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/reels/feed\n  method: get\n  operationId: instagram_get_reels_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/reels/audio\n  method: get\n  operationId: instagram_get_reels_by_audio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/search\n  method: get\n  operationId: instagram_popular_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/location/posts\n  method: get\n  operationId: instagram_get_location_posts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/location/nearby\n  method: get\n  operationId: instagram_get_nearby_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: account_get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/top-ups\n  method: get\n  operationId: account_get_top_ups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/limits\n  method: get\n  operationId: account_get_limits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/socialapis/agentic-access/socialapis-agentic-access.yml
summary_line: 53 operations
tags:
- Company
- Social Media
- Data
- Developers
---
