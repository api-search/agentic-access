---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: prismareviews-connections-api-openapi.yml
  format: yaml
  label: Prisma Reviews Connections API
  slug: prismareviews-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-connections-api-openapi.yml
- filename: prismareviews-locations-api-openapi.yml
  format: yaml
  label: Prisma Reviews Locations API
  slug: prismareviews-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-locations-api-openapi.yml
- filename: prismareviews-platforms-api-openapi.yml
  format: yaml
  label: Prisma Reviews Platforms API
  slug: prismareviews-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-platforms-api-openapi.yml
- filename: prismareviews-replies-api-openapi.yml
  format: yaml
  label: Prisma Reviews Replies API
  slug: prismareviews-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-replies-api-openapi.yml
- filename: prismareviews-reviews-api-openapi.yml
  format: yaml
  label: Prisma Reviews Reviews API
  slug: prismareviews-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-reviews-api-openapi.yml
- filename: prismareviews-stats-api-openapi.yml
  format: yaml
  label: Prisma Reviews Stats API
  slug: prismareviews-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-stats-api-openapi.yml
- filename: prismareviews-usage-api-openapi.yml
  format: yaml
  label: Prisma Reviews Usage API
  slug: prismareviews-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-usage-api-openapi.yml
- filename: prismareviews-webhooks-api-openapi.yml
  format: yaml
  label: Prisma Reviews Webhooks API
  slug: prismareviews-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-webhooks-api-openapi.yml
consequence_counts:
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prismareviews Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Prisma Reviews exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prisma Reviews
provider_slug: prismareviews
slug: prismareviews-agentic-access
source_filename: prismareviews-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/prismareviews-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/reviews\n  method: get\n  operationId: listReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}/reply\n  method:\
  \ post\n  operationId: replyToReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reviews/{id}/reply\n  method: delete\n  operationId: deleteReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/{id}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/{id}/refresh\n  method: post\n  operationId: refreshLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/{id}/stats\n  method: get\n  operationId: getLocationStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platforms\n  method: get\n  operationId: listPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/platforms/{id}\n  method: get\n  operationId: getPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect_links\n  method: post\n  operationId: createConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/prismareviews/agentic-access/prismareviews-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Company
- Reviews
- Software-as-a-Service
- GDPR
- Spain
---
