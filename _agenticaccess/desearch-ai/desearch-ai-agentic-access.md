---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 44
api_specs:
- filename: desearch-ai-ai-search-api-openapi.yml
  format: yaml
  label: desearch-ai AI Search API
  slug: desearch-ai-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-ai-search-api-openapi.yml
- filename: desearch-ai-company-search-api-openapi.yml
  format: yaml
  label: desearch-ai Company Search API
  slug: desearch-ai-company-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-company-search-api-openapi.yml
- filename: desearch-ai-facebook-search-api-openapi.yml
  format: yaml
  label: desearch-ai Facebook Search API
  slug: desearch-ai-facebook-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-facebook-search-api-openapi.yml
- filename: desearch-ai-instagram-search-api-openapi.yml
  format: yaml
  label: desearch-ai Instagram Search API
  slug: desearch-ai-instagram-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-instagram-search-api-openapi.yml
- filename: desearch-ai-network-stats-api-openapi.yml
  format: yaml
  label: desearch-ai Network Stats API
  slug: desearch-ai-network-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-network-stats-api-openapi.yml
- filename: desearch-ai-people-search-api-openapi.yml
  format: yaml
  label: desearch-ai People Search API
  slug: desearch-ai-people-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-people-search-api-openapi.yml
- filename: desearch-ai-search-api-openapi.yml
  format: yaml
  label: desearch-ai Search API
  slug: desearch-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-search-api-openapi.yml
- filename: desearch-ai-tiktok-search-api-openapi.yml
  format: yaml
  label: desearch-ai TikTok Search API
  slug: desearch-ai-tiktok-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-tiktok-search-api-openapi.yml
- filename: desearch-ai-web-search-api-openapi.yml
  format: yaml
  label: desearch-ai Web Search API
  slug: desearch-ai-web-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-web-search-api-openapi.yml
- filename: desearch-ai-x-search-api-openapi.yml
  format: yaml
  label: desearch-ai X Search API
  slug: desearch-ai-x-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desearch-ai/openapi/desearch-ai-x-search-api-openapi.yml
consequence_counts:
  read: 44
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Desearch Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 60
overview: 'desearch-ai exposes 60 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: desearch-ai
provider_slug: desearch-ai
slug: desearch-ai-agentic-access
source_filename: desearch-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/desearch-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 60\n  by_action_class:\n    connected: 44\n    acting: 16\n  by_consequence:\n    read: 44\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search_api_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/ai/search\n  method: post\n  operationId: desearch_desearch_ai_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/ai/search/links/web\n  method: post\n  operationId: search_links_web_desearch_ai_search_links_web_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/ai/search/links/twitter\n  method: post\n  operationId: search_links_twitter_desearch_ai_search_links_twitter_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter\n  method: get\n  operationId: twitter_search_twitter_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/urls\n  method: get\n  operationId: twitter_by_urls_twitter_urls_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/post\n  method: get\n  operationId: twitter_by_id_twitter_post_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/post/user\n  method: get\n  operationId: tweets_by_user_twitter_post_user_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/post/retweeters\n  method: get\n  operationId: get_retweeters_twitter_post_retweeters_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/posts\n  method: get\n  operationId: tweets_by_username_twitter_user_posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/replies\n  method: get\n  operationId: tweets_replies_by_user_twitter_replies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/replies/post\n  method: get\n  operationId: tweets_replies_by_post_twitter_replies_post_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/trends\n  method: get\n  operationId: get_trends_twitter_trends_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/tiktok/search\n  method: post\n  operationId: tiktok_search_desearch_tiktok_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/tiktok/post/{id}\n  method: get\n  operationId: tiktok_post_by_id_desearch_tiktok_post__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/tiktok/profile/{username}\n  method: get\n  operationId: tiktok_profile_desearch_tiktok_profile__username__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/tiktok/profile/{username}/posts\n  method: get\n  operationId: tiktok_profile_posts_desearch_tiktok_profile__username__posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /desearch/tiktok/comments/{video_id}\n  method: get\n  operationId: tiktok_comments_desearch_tiktok_comments__video_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/tiktok/hashtag/{tag}\n  method: get\n  operationId: tiktok_hashtag_desearch_tiktok_hashtag__tag__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/tiktok/trending\n  method: get\n  operationId: tiktok_trending_desearch_tiktok_trending_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/facebook/search\n  method: post\n  operationId: facebook_search_desearch_facebook_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/facebook/post/{id}\n  method: get\n  operationId: facebook_post_by_id_desearch_facebook_post__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/facebook/profile/{profile_id}\n  method: get\n  operationId: facebook_profile_desearch_facebook_profile__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/facebook/profile/{profile_id}/posts\n  method: get\n  operationId: facebook_profile_posts_desearch_facebook_profile__profile_id__posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/facebook/comments/{post_id}\n  method: get\n  operationId: facebook_comments_desearch_facebook_comments__post_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/facebook/hashtag/{tag}\n  method: get\n  operationId: facebook_hashtag_desearch_facebook_hashtag__tag__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/instagram/search\n  method: post\n  operationId: instagram_search_desearch_instagram_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /desearch/instagram/media/{id}\n  method: get\n  operationId: instagram_media_desearch_instagram_media__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/instagram/profile/{username}\n  method: get\n  operationId: instagram_profile_desearch_instagram_profile__username__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/instagram/profile/{username}/posts\n  method: get\n  operationId: instagram_profile_posts_desearch_instagram_profile__username__posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/instagram/comments/{shortcode}\n  method: get\n  operationId: instagram_comments_desearch_instagram_comments__shortcode__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/instagram/hashtag/{tag}\n  method: get\n  operationId: instagram_hashtag_desearch_instagram_hashtag__tag__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web\n  method: get\n  operationId: web_search_web_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/extract\n  method: get\n  operationId: desearch_crawl_web_extract_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/crawl\n  method: get\n  operationId: desearch_crawl_web_crawl_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/search/x\n  method: post\n  operationId: x_profile_search_desearch_people_search_x_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/search/youtube\n  method: post\n  operationId: youtube_creator_search_desearch_people_search_youtube_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/search/linkedin\n  method: post\n  operationId: linkedin_profile_search_desearch_people_search_linkedin_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/search/tiktok\n  method: post\n  operationId: tiktok_creator_search_desearch_people_search_tiktok_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/profiles\n  method: get\n  operationId: list_people_profiles_desearch_people_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/profiles/export\n  method: get\n\
  \  operationId: export_people_profiles_desearch_people_profiles_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/tasks\n  method: get\n  operationId: list_people_tasks_desearch_people_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/tasks/{task_id}\n  method: get\n  operationId: get_people_task_desearch_people_tasks__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/tasks/{task_id}/results\n  method: get\n  operationId: get_people_results_desearch_people_tasks__task_id__results_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /desearch/people/tasks/{task_id}/export\n  method: get\n  operationId: export_people_results_desearch_people_tasks__task_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/people/tasks/{task_id}/pause\n  method: post\n  operationId: pause_people_task_desearch_people_tasks__task_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/tasks/{task_id}/resume\n  method: post\n  operationId: resume_people_task_desearch_people_tasks__task_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/people/tasks/{task_id}/cancel\n  method: post\n  operationId: cancel_people_task_desearch_people_tasks__task_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/companies/search\n  method: post\n  operationId: company_search_desearch_companies_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/companies/enrich\n\
  \  method: post\n  operationId: company_enrich_desearch_companies_enrich_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/companies/tasks\n  method: get\n  operationId: list_company_tasks_desearch_companies_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/companies/tasks/{task_id}\n  method: get\n  operationId: get_company_task_desearch_companies_tasks__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/companies/tasks/{task_id}/results\n  method: get\n  operationId: get_company_results_desearch_companies_tasks__task_id__results_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/companies/tasks/{task_id}/export\n  method: get\n  operationId: export_company_results_desearch_companies_tasks__task_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desearch/companies/tasks/{task_id}/pause\n  method: post\n  operationId: pause_company_task_desearch_companies_tasks__task_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/companies/tasks/{task_id}/resume\n  method: post\n  operationId: resume_company_task_desearch_companies_tasks__task_id__resume_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desearch/companies/tasks/{task_id}/cancel\n  method: post\n  operationId: cancel_company_task_desearch_companies_tasks__task_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/stats\n  method: get\n  operationId: get_network_stats_network_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/stats/history\n  method: get\n  operationId:\
  \ get_network_stats_history_network_stats_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/stats/stream\n  method: get\n  operationId: get_network_stats_stream_network_stats_stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/desearch-ai/agentic-access/desearch-ai-agentic-access.yml
summary_line: 60 operations · 16 acting
tags:
- Artificial Intelligence
- Search
- Web
- Bittensor
- Company
---
