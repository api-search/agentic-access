---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 37
api_specs:
- filename: chatterapi-com-account-api-openapi.yml
  format: yaml
  label: chatterapi-com Account API
  slug: chatterapi-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatterapi-com/openapi/chatterapi-com-account-api-openapi.yml
- filename: chatterapi-com-everywhere-api-openapi.yml
  format: yaml
  label: chatterapi-com Everywhere API
  slug: chatterapi-com-everywhere-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatterapi-com/openapi/chatterapi-com-everywhere-api-openapi.yml
- filename: chatterapi-com-reddit-api-openapi.yml
  format: yaml
  label: chatterapi-com Reddit API
  slug: chatterapi-com-reddit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatterapi-com/openapi/chatterapi-com-reddit-api-openapi.yml
- filename: chatterapi-com-x-api-openapi.yml
  format: yaml
  label: chatterapi-com X API
  slug: chatterapi-com-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatterapi-com/openapi/chatterapi-com-x-api-openapi.yml
consequence_counts:
  physical: 1
  read: 37
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chatterapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x/dm/send
operation_count: 42
overview: 'chatterapi-com exposes 42 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: chatterapi-com
provider_slug: chatterapi-com
slug: chatterapi-com-agentic-access
source_filename: chatterapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/chatterapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 37\n    acting: 5\n  by_consequence:\n    read: 37\n    physical: 1\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/reddit/search\n  method: get\n  operationId: reddit_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/nsfw/search\n  method: get\n  operationId: reddit_nsfw_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/reddit/comments/search\n  method: get\n  operationId: reddit_search_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/media/search\n  method: get\n  operationId: reddit_search_media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/posts/{id}\n  method: get\n  operationId: reddit_scrape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/threads/{id}\n  method: get\n  operationId: reddit_thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/subreddits/search\n  method: get\n  operationId: reddit_communities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/nsfw/subreddits/search\n  method: get\n  operationId: reddit_nsfw_communities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/subreddits/{name}\n  method: get\n  operationId: reddit_subreddit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/subreddits/{name}/posts\n  method: get\n  operationId: reddit_subreddit_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users/{name}\n  method: get\n  operationId: reddit_user\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users/{name}/status\n  method: get\n  operationId: reddit_user_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users/{name}/comments\n  method: get\n  operationId: reddit_user_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users/{name}/posts\n  method: get\n  operationId: reddit_user_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users/search\n  method: get\n  operationId: reddit_user_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/reddit/users/{name}/analysis\n  method: get\n  operationId: reddit_user_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/leads\n  method: get\n  operationId: reddit_leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}\n  method: get\n  operationId: x_user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{source}/follows/{target}\n  method: get\n  operationId: x_follow_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/search\n  method: get\n  operationId: x_user_search\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}/followers\n  method: get\n  operationId: x_followers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}/following\n  method: get\n  operationId: x_following\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}/verified-followers\n  method: get\n  operationId: x_verified_followers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}/tweets\n  method: get\n  operationId: x_tweets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/users/{handle}/mentions\n  method: get\n  operationId: x_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweets/search\n  method: get\n  operationId: x_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweets/{id}\n  method: get\n  operationId: x_tweet_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweets/{id}/replies\n  method: get\n  operationId: x_replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweets/{id}/retweeters\n  method:\
  \ get\n  operationId: x_retweeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/lists/{id}/members\n  method: get\n  operationId: x_list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/leads\n  method: get\n  operationId: x_leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/dm/send\n  method: post\n  operationId: x_dm_send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/x/actions/follow\n  method: post\n  operationId: x_follow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x/actions/like\n  method: post\n  operationId: x_like\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x/tweets\n  method: post\n  operationId: x_tweet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/search\n  method: get\n  operationId: everywhere_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads\n  method: get\n  operationId: everywhere_leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mentions\n  method: get\n  operationId: everywhere_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/run/{toolId}\n  method: post\n  operationId: run_tool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chatterapi-com/agentic-access/chatterapi-com-agentic-access.yml
summary_line: 42 operations · 5 acting
tags:
- Social Media
- Reddit
- X
- Data
- MCP
---
