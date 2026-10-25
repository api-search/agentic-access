---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: blackrock-authorizationurl-generate-api-openapi.yml
  format: yaml
  label: BlackRock Authorization Url:generate API
  slug: blackrock-authorizationurl-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-authorizationurl-generate-api-openapi.yml
- filename: blackrock-studionotifications-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications API
  slug: blackrock-studionotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-api-openapi.yml
- filename: blackrock-studionotifications-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:batch Create API
  slug: blackrock-studionotifications-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-batchcreate-api-openapi.yml
- filename: blackrock-studionotifications-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:filter API
  slug: blackrock-studionotifications-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-filter-api-openapi.yml
- filename: blackrock-studiosubscriptions-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions API
  slug: blackrock-studiosubscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-api-openapi.yml
- filename: blackrock-studiosubscriptions-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:batch Create API
  slug: blackrock-studiosubscriptions-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-batchcreate-api-openapi.yml
- filename: blackrock-studiosubscriptions-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:filter API
  slug: blackrock-studiosubscriptions-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-filter-api-openapi.yml
- filename: blackrock-token-checktokenexists-api-openapi.yml
  format: yaml
  label: BlackRock Token:check Token Exists API
  slug: blackrock-token-checktokenexists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-checktokenexists-api-openapi.yml
- filename: blackrock-token-generate-api-openapi.yml
  format: yaml
  label: BlackRock Token:generate API
  slug: blackrock-token-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-generate-api-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blackrock Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'BlackRock exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlackRock
provider_slug: blackrock
slug: blackrock-agentic-access
source_filename: blackrock-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/blackrock-studio-notification-openapi.yml, openapi/blackrock-studio-subscription-openapi.yml,\n  openapi/blackrock-token-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /studioNotifications\n  method: post\n  operationId: StudioNotificationAPI_CreateStudioNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioNotification\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioNotifications/{id}\n  method: get\n  operationId: StudioNotificationAPI_GetStudioNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - platform.studio.studio_notification.v1.StudioNotification\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studioNotifications:batchCreate\n  method: post\n  operationId: StudioNotificationAPI_BatchCreateStudioNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioNotification\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioNotifications:filter\n  method: post\n  operationId: StudioNotificationAPI_FilterStudioNotifications\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioNotification\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioSubscriptions\n  method: post\n  operationId: StudioSubscriptionAPI_CreateStudioSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioSubscriptions/{id}\n  method: get\n  operationId: StudioSubscriptionAPI_GetStudioSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studioSubscriptions/{id}\n  method: delete\n  operationId: StudioSubscriptionAPI_DeleteStudioSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioSubscriptions/{studioSubscription.id}\n  method: patch\n  operationId: StudioSubscriptionAPI_UpdateStudioSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioSubscriptions:batchCreate\n  method: post\n  operationId: StudioSubscriptionAPI_BatchCreateStudioSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studioSubscriptions:filter\n  method: post\n  operationId: StudioSubscriptionAPI_FilterStudioSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - platform.studio.studio_notification.v1.StudioSubscription\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /authorizationUrl:generate\n  method: get\n  operationId: TokenAPI_GenerateAuthorizationUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - platform.infrastructure.token.v1.Token:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token:checkTokenExists\n  method: get\n  operationId: TokenAPI_CheckTokenExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - platform.infrastructure.token.v1.Token:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token:generate\n  method: get\n  operationId: TokenAPI_GenerateToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - platform.infrastructure.token.v1.Token:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/agentic-access/blackrock-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Asset Management
- Finance
- Fintech
- Investment Management
- Portfolio Management
- Risk Analytics
- Fortune 500
---
