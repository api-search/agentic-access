---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 26
api_specs:
- filename: atproto-com-atproto-openapi.yml
  format: yaml
  label: AT Protocol Core API (com.atproto)
  slug: com-atproto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-com-atproto-openapi.yml
- filename: atproto-app-bsky-openapi.yml
  format: yaml
  label: Bluesky Application API (app.bsky)
  slug: app-bsky
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-app-bsky-openapi.yml
consequence_counts:
  read: 26
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atproto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'AT Protocol exposes 37 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AT Protocol
provider_slug: atproto
slug: atproto-agentic-access
source_filename: atproto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atproto-app-bsky-openapi.yml, openapi/atproto-com-atproto-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 26\n    acting: 11\n  by_consequence:\n    read: 26\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /app.bsky.actor.getProfile\n  method: get\n  operationId: app_bsky_actor_getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.actor.getProfiles\n  method: get\n  operationId: app_bsky_actor_getProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.actor.searchActors\n  method: get\n  operationId: app_bsky_actor_searchActors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.actor.getPreferences\n  method: get\n  operationId: app_bsky_actor_getPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.actor.putPreferences\n  method: post\n  operationId: app_bsky_actor_putPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app.bsky.actor.getSuggestions\n  method: get\n  operationId:\
  \ app_bsky_actor_getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.getTimeline\n  method: get\n  operationId: app_bsky_feed_getTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.getAuthorFeed\n  method: get\n  operationId: app_bsky_feed_getAuthorFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.getPosts\n  method: get\n  operationId: app_bsky_feed_getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.getPostThread\n  method: get\n  operationId: app_bsky_feed_getPostThread\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.searchPosts\n  method: get\n  operationId: app_bsky_feed_searchPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.feed.getLikes\n  method: get\n  operationId: app_bsky_feed_getLikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.graph.getFollowers\n  method: get\n  operationId: app_bsky_graph_getFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.graph.getFollows\n  method: get\n  operationId: app_bsky_graph_getFollows\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.notification.listNotifications\n  method: get\n  operationId: app_bsky_notification_listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app.bsky.notification.getUnreadCount\n  method: get\n  operationId: app_bsky_notification_getUnreadCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.server.describeServer\n  method: get\n  operationId: com_atproto_server_describeServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.server.createSession\n  method: post\n  operationId: com_atproto_server_createSession\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.server.deleteSession\n  method: post\n  operationId: com_atproto_server_deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.server.getSession\n  method: get\n  operationId: com_atproto_server_getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.server.refreshSession\n  method: post\n  operationId: com_atproto_server_refreshSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.server.createAccount\n  method: post\n  operationId: com_atproto_server_createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.server.deleteAccount\n  method: post\n  operationId: com_atproto_server_deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /com.atproto.server.checkAccountStatus\n  method: get\n  operationId: com_atproto_server_checkAccountStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.identity.resolveHandle\n  method: get\n  operationId: com_atproto_identity_resolveHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.identity.updateHandle\n  method: post\n  operationId: com_atproto_identity_updateHandle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.identity.resolveDid\n  method: get\n  operationId:\
  \ com_atproto_identity_resolveDid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.repo.getRecord\n  method: get\n  operationId: com_atproto_repo_getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.repo.createRecord\n  method: post\n  operationId: com_atproto_repo_createRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.repo.putRecord\n  method: post\n  operationId: com_atproto_repo_putRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.repo.deleteRecord\n  method: post\n  operationId: com_atproto_repo_deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.repo.listRecords\n  method: get\n  operationId: com_atproto_repo_listRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.repo.uploadBlob\n  method: post\n  operationId: com_atproto_repo_uploadBlob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /com.atproto.repo.describeRepo\n  method: get\n  operationId: com_atproto_repo_describeRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.sync.getRepo\n  method: get\n  operationId: com_atproto_sync_getRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.sync.getBlob\n  method: get\n  operationId: com_atproto_sync_getBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /com.atproto.sync.listRepos\n  method: get\n  operationId: com_atproto_sync_listRepos\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/agentic-access/atproto-agentic-access.yml
summary_line: 37 operations · 11 acting
tags:
- Social Networking
- Decentralized
- Federated
- Open Source
- Bluesky
- Fediverse
- Identity
- XRPC
- Lexicon
---
