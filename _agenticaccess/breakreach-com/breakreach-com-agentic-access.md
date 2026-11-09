---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 21
api_specs:
- filename: breakreach-com-accounts-api-openapi.yml
  format: yaml
  label: Breakreach Accounts API
  slug: breakreach-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-accounts-api-openapi.yml
- filename: breakreach-com-analytics-api-openapi.yml
  format: yaml
  label: Breakreach Analytics API
  slug: breakreach-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-analytics-api-openapi.yml
- filename: breakreach-com-comment-dm-rules-api-openapi.yml
  format: yaml
  label: Breakreach Comment Dm Rules API
  slug: breakreach-com-comment-dm-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-comment-dm-rules-api-openapi.yml
- filename: breakreach-com-comments-api-openapi.yml
  format: yaml
  label: Breakreach Comments API
  slug: breakreach-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-comments-api-openapi.yml
- filename: breakreach-com-connect-links-api-openapi.yml
  format: yaml
  label: Breakreach Connect Links API
  slug: breakreach-com-connect-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-connect-links-api-openapi.yml
- filename: breakreach-com-dm-automations-api-openapi.yml
  format: yaml
  label: Breakreach Dm Automations API
  slug: breakreach-com-dm-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-dm-automations-api-openapi.yml
- filename: breakreach-com-inbox-api-openapi.yml
  format: yaml
  label: Breakreach Inbox API
  slug: breakreach-com-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-inbox-api-openapi.yml
- filename: breakreach-com-media-api-openapi.yml
  format: yaml
  label: Breakreach Media API
  slug: breakreach-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-media-api-openapi.yml
- filename: breakreach-com-next-slot-api-openapi.yml
  format: yaml
  label: Breakreach Next Slot API
  slug: breakreach-com-next-slot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-next-slot-api-openapi.yml
- filename: breakreach-com-performance-api-openapi.yml
  format: yaml
  label: Breakreach Performance API
  slug: breakreach-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-performance-api-openapi.yml
- filename: breakreach-com-pinterest-boards-api-openapi.yml
  format: yaml
  label: Breakreach Pinterest Boards API
  slug: breakreach-com-pinterest-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-pinterest-boards-api-openapi.yml
- filename: breakreach-com-post-insights-api-openapi.yml
  format: yaml
  label: Breakreach Post Insights API
  slug: breakreach-com-post-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-post-insights-api-openapi.yml
- filename: breakreach-com-posts-api-openapi.yml
  format: yaml
  label: Breakreach Posts API
  slug: breakreach-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-posts-api-openapi.yml
- filename: breakreach-com-workspaces-api-openapi.yml
  format: yaml
  label: Breakreach Workspaces API
  slug: breakreach-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-workspaces-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Breakreach Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/connect-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inbox/{conversationId}/messages
operation_count: 38
overview: 'Breakreach exposes 38 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 15 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Breakreach
provider_slug: breakreach-com
slug: breakreach-com-agentic-access
source_filename: breakreach-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/breakreach-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 21\n    acting: 17\n  by_consequence:\n    read: 21\n    write: 15\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect-links\n  method: post\n  operationId: createConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect-links/{id}\n  method: get\n  operationId: getConnectLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect-links/{id}\n  method: delete\n  operationId: revokeConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}\n  method: patch\n  operationId: updatePost\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}\n  method: delete\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/upload\n  method: post\n  operationId: uploadMediaFile\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/next-slot\n  method: get\n  operationId: getNextSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pinterest-boards\n  method: get\n  operationId: listPinterestBoards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/stats\n  method: get\n  operationId: getAccountStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/post-insights\n  method: get\n  operationId: getPostInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/trends\n  method: get\n  operationId: getAccountTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/{id}/metrics\n  method: get\n  operationId: getPostMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/{id}/comments\n  method: get\n  operationId: getPostComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/comments\n  method: get\n  operationId: listRecentComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comments/reply\n  method: post\n  operationId: replyToComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comments/{commentId}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/performance\n  method: get\n  operationId:\
  \ getContentPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inbox\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inbox/{conversationId}/messages\n  method: get\n  operationId: getConversationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inbox/{conversationId}/messages\n  method: post\n  operationId: sendDirectMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comment-dm-rules\n  method: get\n  operationId: listCommentDmRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comment-dm-rules\n  method: post\n  operationId: createCommentDmRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comment-dm-rules/media\n  method: get\n  operationId: listCommentDmMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comment-dm-rules/{id}\n  method: patch\n  operationId: updateCommentDmRule\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comment-dm-rules/{id}\n  method: delete\n  operationId: deleteCommentDmRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comment-dm-rules/{id}/events\n  method: get\n  operationId: listCommentDmEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dm-automations\n  method: get\n  operationId: listDmAutomations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dm-automations\n  method: post\n  operationId: createDmAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dm-automations/{id}\n  method: patch\n  operationId: updateDmAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dm-automations/{id}\n  method: delete\n  operationId: deleteDmAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dm-automations/{id}/runs\n  method: get\n  operationId: listDmAutomationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/breakreach-com/agentic-access/breakreach-com-agentic-access.yml
summary_line: 38 operations · 17 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Social Media
- Automation
- Scheduling
- Marketing
---
