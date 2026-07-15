---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: facebook-pages-openapi.yml
  format: yaml
  label: Meta Graph API - Pages
  slug: graph-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-openapi.yml
consequence_counts:
  read: 11
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Facebook Pages Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Facebook Pages API exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Facebook Pages API
provider_slug: facebook-pages
slug: facebook-pages-agentic-access
source_filename: facebook-pages-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/facebook-pages-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /{page-id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}\n  method: post\n  operationId: updatePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/feed\n  method: get\n  operationId: listPageFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/feed\n  method: post\n  operationId: publishPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/posts\n  method: get\n  operationId: listPagePosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/photos\n  method: get\n  operationId: listPagePhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/photos\n  method: post\n  operationId: uploadPagePhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/insights\n  method: get\n  operationId: getPageInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/conversations\n  method: get\n  operationId: listPageConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/tagged\n  method: get\n  operationId:\
  \ listPageTagged\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/settings\n  method: get\n  operationId: getPageSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/settings\n  method: post\n  operationId: updatePageSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n\
  \    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{object-id}/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{object-id}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{comment-id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/subscribed_apps\n  method: get\n  operationId: listSubscribedApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /{page-id}/subscribed_apps\n  method: post\n  operationId: subscribePageApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n- path: /me/accounts\n  method: get\n  operationId: listMyPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - pages_manage_metadata\n    - pages_manage_posts\n    - pages_read_engagement\n    - pages_show_list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/agentic-access/facebook-pages-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Social Media
- Facebook
- Meta Graph API
- Pages
- Content Publishing
- Social Insights
---
