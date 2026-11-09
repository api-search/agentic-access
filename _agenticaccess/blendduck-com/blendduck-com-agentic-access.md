---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 14
api_specs:
- filename: blendduck-com-analytics-api-openapi.yml
  format: yaml
  label: BlendDuck Analytics API
  slug: blendduck-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-analytics-api-openapi.yml
- filename: blendduck-com-channels-api-openapi.yml
  format: yaml
  label: BlendDuck Channels API
  slug: blendduck-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-channels-api-openapi.yml
- filename: blendduck-com-media-api-openapi.yml
  format: yaml
  label: BlendDuck Media API
  slug: blendduck-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-media-api-openapi.yml
- filename: blendduck-com-posts-api-openapi.yml
  format: yaml
  label: BlendDuck Posts API
  slug: blendduck-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-posts-api-openapi.yml
- filename: blendduck-com-providers-api-openapi.yml
  format: yaml
  label: BlendDuck Providers API
  slug: blendduck-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-providers-api-openapi.yml
- filename: blendduck-com-tenant-api-openapi.yml
  format: yaml
  label: BlendDuck Tenant API
  slug: blendduck-com-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-tenant-api-openapi.yml
- filename: blendduck-com-webhooks-api-openapi.yml
  format: yaml
  label: BlendDuck Webhooks API
  slug: blendduck-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blendduck-com/openapi/blendduck-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blendduck Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/{webhookEndpointId}/test
operation_count: 25
overview: 'BlendDuck exposes 25 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlendDuck
provider_slug: blendduck-com
slug: blendduck-com-agentic-access
source_filename: blendduck-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blendduck-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 14\n    acting: 11\n  by_consequence:\n    read: 14\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/tenant\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/channels/{channelId}\n\
  \  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/channels/{channelId}\n  method: delete\n  operationId: disconnectChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/posts/{postId}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts/{postId}\n  method: patch\n  operationId: updatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/posts/{postId}\n  method: delete\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/v1/analytics\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/media/{mediaId}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookEndpointId}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{webhookEndpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookEndpointId}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookEndpointId}/rotate\n  method: post\n  operationId: rotateWebhookEndpointSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/webhooks/{webhookEndpointId}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{webhookEndpointId}/deliveries/{webhookDeliveryId}\n  method: get\n  operationId: getWebhookDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{webhookEndpointId}/test\n  method: post\n  operationId: sendWebhookTest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookEndpointId}/deliveries/{webhookDeliveryId}/replay\n\
  \  method: post\n  operationId: replayWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers/{providerId}\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blendduck-com/agentic-access/blendduck-com-agentic-access.yml
summary_line: 25 operations · 11 acting
tags:
- Social
- Collaboration
- Artificial Intelligence
- Branding
- Marketing
- Company
---
