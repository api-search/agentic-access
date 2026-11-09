---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 7
api_specs:
- filename: blog2social-com-account-api-openapi.yml
  format: yaml
  label: Blog2Social Account API
  slug: blog2social-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-account-api-openapi.yml
- filename: blog2social-com-authentication-api-openapi.yml
  format: yaml
  label: Blog2Social Authentication API
  slug: blog2social-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-authentication-api-openapi.yml
- filename: blog2social-com-insights-api-openapi.yml
  format: yaml
  label: Blog2Social Insights API
  slug: blog2social-com-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-insights-api-openapi.yml
- filename: blog2social-com-network-api-openapi.yml
  format: yaml
  label: Blog2Social Network API
  slug: blog2social-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-network-api-openapi.yml
- filename: blog2social-com-share-api-openapi.yml
  format: yaml
  label: Blog2Social Share API
  slug: blog2social-com-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-share-api-openapi.yml
- filename: blog2social-com-user-api-openapi.yml
  format: yaml
  label: Blog2Social User API
  slug: blog2social-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-user-api-openapi.yml
- filename: blog2social-com-video-api-openapi.yml
  format: yaml
  label: Blog2Social Video API
  slug: blog2social-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blog2social-com/openapi/blog2social-com-video-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Blog2Social Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /network/post/insights/status/disable
operation_count: 21
overview: 'Blog2Social exposes 21 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 13 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blog2Social
provider_slug: blog2social-com
slug: blog2social-com-agentic-access
source_filename: blog2social-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blog2social-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 14\n    connected: 7\n  by_consequence:\n    write: 13\n    read: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /user/auth\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/list\n  method: post\n  operationId: listUser\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/delete\n  method: post\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/list\n  method: post\n  operationId: listNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/add\n  method: post\n  operationId: add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /network/update\n  method: post\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/categories\n  method: post\n  operationId: listBoards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/properties\n  method: post\n  operationId: network_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/auth/list\n  method: post\n  operationId: listAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /user/auth/delete\n  method: post\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/create\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/remove\n  method: post\n  operationId: remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /network/post/insights/v2/get\n  method: post\n  operationId: v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/insights/total\n  method: post\n  operationId: v1-total\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/insights/graph\n  method: post\n  operationId: v1-graph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/insights/status/enable\n  method: post\n  operationId: v1-enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/post/insights/status/disable\n  method: post\n  operationId: v1-disable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /network/post/create/\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/upload\n  method: post\n  operationId: video_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/overview\n  method: post\n  operationId: account_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/check\n  method: post\n  operationId: video_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blog2social-com/agentic-access/blog2social-com-agentic-access.yml
summary_line: 21 operations · 14 acting · 1 human-in-the-loop
tags:
- Social Media
- Automation
- WordPress
- Marketing
- Software-as-a-Service
---
