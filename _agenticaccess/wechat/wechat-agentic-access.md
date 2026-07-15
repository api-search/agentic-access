---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Pay APIv3 (Direct-Connect Merchant)
  slug: wechat-pay-apiv3-direct-merchant
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Official Accounts API
  slug: wechat-official-accounts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Work (WeCom) API
  slug: wechat-work-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wechat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'WeChat exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WeChat
provider_slug: wechat
slug: wechat-agentic-access
source_filename: wechat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wechat-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /cgi-bin/token\n  method: get\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sns/jscode2session\n  method: get\n  operationId: code2Session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wxa/getpaidunionid\n  method: get\n  operationId: getPaidUnionId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/agentic-access/wechat-agentic-access.yml
summary_line: 3 operations
tags:
- Messaging
- Social
- Payments
- Mini Programs
- Mini Games
- Official Accounts
- Enterprise Communication
- Cloud Hosting
- Video
- Identity
- China
- Super App
- Tencent
---
