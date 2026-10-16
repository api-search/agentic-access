---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: xproapi-default-api-openapi.yml
  format: yaml
  label: Xproapi Default API
  slug: xproapi-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-default-api-openapi.yml
- filename: xproapi-follow-followings-api-openapi.yml
  format: yaml
  label: Xproapi Follow, Followings API
  slug: xproapi-follow-followings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-follow-followings-api-openapi.yml
- filename: xproapi-tweet-activity-api-openapi.yml
  format: yaml
  label: Xproapi Tweet Activity API
  slug: xproapi-tweet-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-tweet-activity-api-openapi.yml
- filename: xproapi-tweets-api-openapi.yml
  format: yaml
  label: Xproapi Tweets API
  slug: xproapi-tweets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-tweets-api-openapi.yml
- filename: xproapi-users-api-openapi.yml
  format: yaml
  label: Xproapi Users API
  slug: xproapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/openapi/xproapi-users-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xproapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Xproapi exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xproapi
provider_slug: xproapi
slug: xproapi-agentic-access
source_filename: xproapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/xproapi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /twitter/user_about\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/batch_info_by_ids\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/batch_info_by_usernames\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/tweet_timeline\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/last_tweets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/advanced_search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/replies/v2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/quotes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/retweeters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/thread_context\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /twitter/tweet/replies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/followers/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/followings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/followers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twitter/user/mentions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /twitter/article\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xproapi/refs/heads/main/agentic-access/xproapi-agentic-access.yml
summary_line: 19 operations
tags:
- Company
- API
- X
- Social
- Monitoring
- Data
---
