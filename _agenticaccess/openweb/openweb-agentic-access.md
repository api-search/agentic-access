---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 14
api_specs:
- filename: openweb-export-api-openapi.yml
  format: yaml
  label: OpenWeb Export API
  slug: openweb-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-export-api-openapi.yml
- filename: openweb-top-comments-api-openapi.yml
  format: yaml
  label: OpenWeb top comments API
  slug: openweb-top-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-top-comments-api-openapi.yml
- filename: openweb-trending-articles-api-openapi.yml
  format: yaml
  label: OpenWeb trending articles API
  slug: openweb-trending-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-trending-articles-api-openapi.yml
- filename: openweb-article-api-openapi.yml
  format: yaml
  label: OpenWeb Article API
  slug: openweb-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-article-api-openapi.yml
- filename: openweb-comment-api-openapi.yml
  format: yaml
  label: OpenWeb Comment API
  slug: openweb-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-comment-api-openapi.yml
- filename: openweb-live-blog-api-openapi.yml
  format: yaml
  label: OpenWeb live blog API
  slug: openweb-live-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-live-blog-api-openapi.yml
- filename: openweb-moderation-policy-api-openapi.yml
  format: yaml
  label: OpenWeb moderation policy API
  slug: openweb-moderation-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-moderation-policy-api-openapi.yml
- filename: openweb-score-and-reviews-api-openapi.yml
  format: yaml
  label: OpenWeb score and reviews API
  slug: openweb-score-and-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-score-and-reviews-api-openapi.yml
- filename: openweb-sso-api-openapi.yml
  format: yaml
  label: OpenWeb SSO API
  slug: openweb-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-sso-api-openapi.yml
- filename: openweb-token-api-openapi.yml
  format: yaml
  label: OpenWeb Token API
  slug: openweb-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/openapi/openweb-token-api-openapi.yml
consequence_counts:
  read: 14
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openweb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'OpenWeb exposes 24 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenWeb
provider_slug: openweb
slug: openweb-agentic-access
source_filename: openweb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/openweb-export-api-openapi.yml, openapi/openweb-moderation-policy-openapi.yml,\n  openapi/openweb-publisher-authentication-api-openapi.yml, openapi/openweb-seo-service-openapi.yml,\n  openapi/openweb-single-sign-on-api-openapi.yml, openapi/openweb-top-comments-api-openapi.yml,\n  openapi/openweb-trending-articles-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 10\n    connected: 14\n  by_consequence:\n    write: 10\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/export/comments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/export/comments/abort\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/export/comments/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/export/comments/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/export\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v4/export/abort\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/export/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/export/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation-policy/spot/{spot_id}/post/{post_id}\n  method: get\n  operationId: get-conversation-policy-spot-spot_id-post-post_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation-policy/spot/{spot_id}/post/{post_id}/{policy}\n  method: post\n  operationId:\
  \ post-conversation-policy-spot-spot_id-post-post_id-policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publisher/auth\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /article/live-blog/{spot_id}/{liveblog_id}\n  method: post\n  operationId: post-liveblog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /article/{spot_id}/{post_id}\n  method: post\n  operationId: post-article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/{spot_id}/{post_id}\n  method: post\n  operationId: post-comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stars-and-reviews/{spot_id}/{post_id}\n  method: post\n  operationId: post-reviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso/v1/register-user\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso/v1/update-user\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso/v1/user\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso/v1/user/{primary_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sso/v1/user/{primary_key}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /top-comments-conversation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top-comments-spot\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top-comments-user\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trending-articles\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweb/refs/heads/main/agentic-access/openweb-agentic-access.yml
summary_line: 24 operations · 10 acting
tags:
- Company
- Consumer
- Community
- Comments
- Audience Engagement
- Publishing
- Media
- Moderation
- Identity
- SSO
- Webhook
---
