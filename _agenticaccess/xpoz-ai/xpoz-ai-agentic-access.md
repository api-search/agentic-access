---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 64
api_specs:
- filename: xpoz-ai-account-api-openapi.yml
  format: yaml
  label: xpoz-ai Account API
  slug: xpoz-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-account-api-openapi.yml
- filename: xpoz-ai-billing-api-openapi.yml
  format: yaml
  label: xpoz-ai Billing API
  slug: xpoz-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-billing-api-openapi.yml
- filename: xpoz-ai-crawl-settings-api-openapi.yml
  format: yaml
  label: xpoz-ai Crawl Settings API
  slug: xpoz-ai-crawl-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-crawl-settings-api-openapi.yml
- filename: xpoz-ai-instagram-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Instagram (live) API
  slug: xpoz-ai-instagram-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-instagram-live-api-openapi.yml
- filename: xpoz-ai-operations-api-openapi.yml
  format: yaml
  label: xpoz-ai Operations API
  slug: xpoz-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-operations-api-openapi.yml
- filename: xpoz-ai-platform-api-openapi.yml
  format: yaml
  label: xpoz-ai Platform API
  slug: xpoz-ai-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-platform-api-openapi.yml
- filename: xpoz-ai-reddit-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Reddit (live) API
  slug: xpoz-ai-reddit-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-reddit-live-api-openapi.yml
- filename: xpoz-ai-system-status-api-openapi.yml
  format: yaml
  label: xpoz-ai System Status API
  slug: xpoz-ai-system-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-system-status-api-openapi.yml
- filename: xpoz-ai-tiktok-live-api-openapi.yml
  format: yaml
  label: xpoz-ai TikTok (live) API
  slug: xpoz-ai-tiktok-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-tiktok-live-api-openapi.yml
- filename: xpoz-ai-twitter-live-api-openapi.yml
  format: yaml
  label: xpoz-ai Twitter (live) API
  slug: xpoz-ai-twitter-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpoz-ai/openapi/xpoz-ai-twitter-live-api-openapi.yml
consequence_counts:
  physical: 5
  read: 64
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Xpoz Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extra-credits/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extra-credits/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extra-csv-rows/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extra-csv-rows/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stripe/create-checkout-session
operation_count: 80
overview: 'xpoz-ai exposes 80 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 64 read, 10 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: xpoz-ai
provider_slug: xpoz-ai
slug: xpoz-ai-agentic-access
source_filename: xpoz-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/xpoz-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 80\n  by_action_class:\n    connected: 64\n    acting: 16\n  by_consequence:\n    read: 64\n    safety-critical: 1\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 1\noperations:\n- path: /api/data/twitter/posts/live\n  method: get\n  operationId: getDataTwitterPostsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/live\n  method: post\n  operationId: postDataTwitterPostsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/users/{username}/live\n  method: get\n  operationId: getDataTwitterPostsUsersUsernameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/{id}/live\n  method: get\n  operationId: getDataTwitterPostsIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/{id}/comments/live\n  method: get\n  operationId: getDataTwitterPostsIdCommentsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/{id}/quotes/live\n  method: get\n  operationId: getDataTwitterPostsIdQuotesLive\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/posts/{id}/interacting-users/live\n  method: get\n  operationId: getDataTwitterPostsIdInteractingUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/users/live\n  method: get\n  operationId: getDataTwitterUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/users/live\n  method: post\n  operationId: postDataTwitterUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/users/{username}/live\n  method: get\n  operationId: getDataTwitterUsersUsernameLive\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/twitter/users/{username}/connections/live\n  method: get\n  operationId: getDataTwitterUsersUsernameConnectionsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/live\n  method: get\n  operationId: getDataInstagramPostsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/users/{identifier}/live\n  method: get\n  operationId: getDataInstagramPostsUsersIdentifierLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/{id}/live\n  method: get\n  operationId: getDataInstagramPostsIdLive\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/{id}/comments/live\n  method: get\n  operationId: getDataInstagramPostsIdCommentsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/{id}/comments/{commentId}/live\n  method: get\n  operationId: getDataInstagramPostsIdCommentsCommentIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/posts/{id}/comments/{commentId}/replies/live\n  method: get\n  operationId: getDataInstagramPostsIdCommentsCommentIdRepliesLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/data/instagram/posts/{id}/interacting-users/live\n  method: get\n  operationId: getDataInstagramPostsIdInteractingUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/users/live\n  method: get\n  operationId: getDataInstagramUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/users/{identifier}/live\n  method: get\n  operationId: getDataInstagramUsersIdentifierLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/instagram/users/{identifier}/connections/live\n  method: get\n  operationId: getDataInstagramUsersIdentifierConnectionsLive\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/live\n  method: get\n  operationId: getDataRedditPostsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/users/{username}/live\n  method: get\n  operationId: getDataRedditPostsUsersUsernameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/subreddits/{name}/live\n  method: get\n  operationId: getDataRedditPostsSubredditsNameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/ids/live\n  method: get\n  operationId: getDataRedditPostsIdsLive\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/{id}/live\n  method: get\n  operationId: getDataRedditPostsIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/posts/{id}/comments/live\n  method: get\n  operationId: getDataRedditPostsIdCommentsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/comments/users/{username}/live\n  method: get\n  operationId: getDataRedditCommentsUsersUsernameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/comments/ids/live\n  method: get\n  operationId: getDataRedditCommentsIdsLive\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/comments/{id}/live\n  method: get\n  operationId: getDataRedditCommentsIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/users/live\n  method: get\n  operationId: getDataRedditUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/users/{username}/live\n  method: get\n  operationId: getDataRedditUsersUsernameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/subreddits/live\n  method: get\n  operationId: getDataRedditSubredditsLive\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/subreddits/{name}/live\n  method: get\n  operationId: getDataRedditSubredditsNameLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/reddit/resolve/live\n  method: get\n  operationId: getDataRedditResolveLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/live\n  method: get\n  operationId: getDataTiktokPostsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/hashtags/{hashtag}/live\n  method: get\n  operationId: getDataTiktokPostsHashtagsHashtagLive\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/sounds/{sound}/live\n  method: get\n  operationId: getDataTiktokPostsSoundsSoundLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/users/{identifier}/live\n  method: get\n  operationId: getDataTiktokPostsUsersIdentifierLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/{id}/live\n  method: get\n  operationId: getDataTiktokPostsIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/{id}/comments/live\n  method: get\n  operationId: getDataTiktokPostsIdCommentsLive\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/{id}/comments/{commentId}/live\n  method: get\n  operationId: getDataTiktokPostsIdCommentsCommentIdLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/posts/{id}/comments/{commentId}/replies/live\n  method: get\n  operationId: getDataTiktokPostsIdCommentsCommentIdRepliesLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/users/live\n  method: get\n  operationId: getDataTiktokUsersLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/users/{identifier}/live\n\
  \  method: get\n  operationId: getDataTiktokUsersIdentifierLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/users/{identifier}/connections/live\n  method: get\n  operationId: getDataTiktokUsersIdentifierConnectionsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/sounds/live\n  method: get\n  operationId: getDataTiktokSoundsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/tiktok/hashtags/live\n  method: get\n  operationId: getDataTiktokHashtagsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/operations/{id}\n\
  \  method: get\n  operationId: getDataOperationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.yaml\n  method: get\n  operationId: getOpenapi.yaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenapi.json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: put\n  operationId: putStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/status/history\n  method: get\n  operationId: getStatusHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status/subscribe\n  method: post\n  operationId: postStatusSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/status/unsubscribe\n  method: get\n  operationId: getStatusUnsubscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tokens\n  method: get\n  operationId: getTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tokens\n  method: post\n  operationId: postTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tokens/rotate\n\
  \  method: post\n  operationId: postTokensRotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/plan\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/usage-history\n  method: get\n  operationId: getUsageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crawl/settings\n  method: get\n\
  \  operationId: getCrawlSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crawl/settings\n  method: post\n  operationId: postCrawlSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crawl/settings/upload-csv\n  method: post\n  operationId: postCrawlSettingsUploadCsv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crawl/settings/export-csv\n  method: get\n  operationId: getCrawlSettingsExportCsv\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crawl/tweet\n  method: post\n  operationId: postCrawlTweet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crawl/tweet\n  method: get\n  operationId: getCrawlTweet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extra-credits/purchase\n  method: post\n  operationId: postExtraCreditsPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extra-credits/confirm\n  method: post\n  operationId: postExtraCreditsConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extra-csv-rows/purchase\n  method: post\n  operationId: postExtraCsvRowsPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extra-csv-rows/confirm\n\
  \  method: post\n  operationId: postExtraCsvRowsConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extra-tracked-items\n  method: get\n  operationId: getExtraTrackedItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extra-tracked-items\n  method: patch\n  operationId: patchExtraTrackedItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stripe/create-checkout-session\n\
  \  method: post\n  operationId: postStripeCreateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stripe/subscription\n  method: patch\n  operationId: patchStripeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stripe/webhooks\n  method: post\n  operationId: postStripeWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/trial/token\n  method: post\n  operationId: postTrialToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/xpoz-ai/agentic-access/xpoz-ai-agentic-access.yml
summary_line: 80 operations · 16 acting · 1 human-in-the-loop
tags:
- Company
- Social Data
- Artificial Intelligence
- Monitoring
- Analytics
- SDK
---
