---
acting_count: 0
action_class_counts:
  connected: 43
api_specs:
- filename: sociallisteningapi-discourse-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Discourse API
  slug: sociallisteningapi-discourse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-discourse-api-openapi.yml
- filename: sociallisteningapi-facebook-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Facebook API
  slug: sociallisteningapi-facebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-facebook-api-openapi.yml
- filename: sociallisteningapi-google-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Google API
  slug: sociallisteningapi-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-google-api-openapi.yml
- filename: sociallisteningapi-instagram-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Instagram API
  slug: sociallisteningapi-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-instagram-api-openapi.yml
- filename: sociallisteningapi-meta-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Meta API
  slug: sociallisteningapi-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-meta-api-openapi.yml
- filename: sociallisteningapi-pinterest-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Pinterest API
  slug: sociallisteningapi-pinterest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-pinterest-api-openapi.yml
- filename: sociallisteningapi-reddit-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Reddit API
  slug: sociallisteningapi-reddit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-reddit-api-openapi.yml
- filename: sociallisteningapi-tiktok-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Tiktok API
  slug: sociallisteningapi-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-tiktok-api-openapi.yml
- filename: sociallisteningapi-x-api-openapi.yml
  format: yaml
  label: SocialListeningAPI X API
  slug: sociallisteningapi-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-x-api-openapi.yml
- filename: sociallisteningapi-youtube-api-openapi.yml
  format: yaml
  label: SocialListeningAPI YouTube API
  slug: sociallisteningapi-youtube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-youtube-api-openapi.yml
- filename: sociallisteningapi-hacker-news-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Hacker News API
  slug: sociallisteningapi-hacker-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-hacker-news-api-openapi.yml
- filename: sociallisteningapi-linked-in-api-openapi.yml
  format: yaml
  label: SocialListeningAPI Linked In API
  slug: sociallisteningapi-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-linked-in-api-openapi.yml
consequence_counts:
  read: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sociallisteningapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'SocialListeningAPI exposes 43 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 43 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SocialListeningAPI
provider_slug: sociallisteningapi
slug: sociallisteningapi-agentic-access
source_filename: sociallisteningapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/sociallisteningapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 43\n  by_consequence:\n    read: 43\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/instagram/search\n  method: get\n  operationId: searchInstagram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/instagram/search\n  method:\
  \ post\n  operationId: searchInstagramWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/instagram/profile\n  method: get\n  operationId: getInstagramProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/instagram/profile\n  method: post\n  operationId: getInstagramProfileWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/search\n  method: get\n  operationId: searchLinkedin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/search\n  method: post\n  operationId: searchLinkedinWithPost\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/profile\n  method: get\n  operationId: getLinkedinProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/profile\n  method: post\n  operationId: getLinkedinProfileWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/profile/posts\n  method: get\n  operationId: getLinkedinProfilePosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/profile/posts\n  method: post\n  operationId: getLinkedinProfilePostsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/user/posts\n  method: get\n  operationId: getLinkedinUserPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/user/posts\n  method: post\n  operationId: getLinkedinUserPostsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/search\n  method: get\n  operationId: searchX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/search\n  method: post\n  operationId: searchXWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/user\n\
  \  method: get\n  operationId: getXUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/user\n  method: post\n  operationId: getXUserWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/user/posts\n  method: get\n  operationId: getXUserPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/user/posts\n  method: post\n  operationId: getXUserPostsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/tweet/thread\n  method: get\n  operationId: getXTweetThread\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/tweet/thread\n  method: post\n  operationId: getXTweetThreadWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/tweet/replies\n  method: get\n  operationId: getXTweetReplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/x/tweet/replies\n  method: post\n  operationId: getXTweetRepliesWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reddit/search-posts\n  method: get\n  operationId: searchRedditPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/reddit/search-posts\n  method: post\n  operationId: searchRedditPostsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reddit/search-comments\n  method: get\n  operationId: searchRedditComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reddit/search-comments\n  method: post\n  operationId: searchRedditCommentsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reddit/post/comments\n  method: get\n  operationId: getRedditPostComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reddit/post/comments\n\
  \  method: post\n  operationId: getRedditPostCommentsWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/facebook/search\n  method: get\n  operationId: searchFacebook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/facebook/search\n  method: post\n  operationId: searchFacebookWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hackernews/search\n  method: get\n  operationId: searchHackernews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hackernews/search\n  method: post\n  operationId: searchHackernewsWithPost\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tiktok/search\n  method: get\n  operationId: searchTiktok\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tiktok/search\n  method: post\n  operationId: searchTiktokWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/youtube/search\n  method: get\n  operationId: searchYoutube\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/youtube/search\n  method: post\n  operationId: searchYoutubeWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/pinterest/search\n  method: get\n  operationId: searchPinterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pinterest/search\n  method: post\n  operationId: searchPinterestWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/google/search\n  method: get\n  operationId: searchGoogle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/google/search\n  method: post\n  operationId: searchGoogleWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discourse/search\n  method: get\n  operationId:\
  \ searchDiscourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discourse/search\n  method: post\n  operationId: searchDiscourseWithPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/agentic-access/sociallisteningapi-agentic-access.yml
summary_line: 43 operations
tags:
- Social Listening
- Social Media
- Search
- Brand Monitoring
- Market Research
- MCP
- Reddit
- LinkedIn
---
