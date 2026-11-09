---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 8
api_specs:
- filename: postonce-accounts-api-openapi.yml
  format: yaml
  label: PostOnce Accounts API
  slug: postonce-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postonce/openapi/postonce-accounts-api-openapi.yml
- filename: postonce-drafts-api-openapi.yml
  format: yaml
  label: PostOnce Drafts API
  slug: postonce-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postonce/openapi/postonce-drafts-api-openapi.yml
- filename: postonce-media-api-openapi.yml
  format: yaml
  label: PostOnce Media API
  slug: postonce-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postonce/openapi/postonce-media-api-openapi.yml
- filename: postonce-posts-api-openapi.yml
  format: yaml
  label: PostOnce Posts API
  slug: postonce-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postonce/openapi/postonce-posts-api-openapi.yml
- filename: postonce-workflows-api-openapi.yml
  format: yaml
  label: PostOnce Workflows API
  slug: postonce-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postonce/openapi/postonce-workflows-api-openapi.yml
consequence_counts:
  read: 8
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Postonce Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'PostOnce exposes 22 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PostOnce
provider_slug: postonce
slug: postonce-agentic-access
source_filename: postonce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/postonce-accounts-api-openapi.yml, openapi/postonce-drafts-api-openapi.yml,\n  openapi/postonce-media-api-openapi.yml, openapi/postonce-posts-api-openapi.yml, openapi/postonce-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 8\n    acting: 14\n  by_consequence:\n    read: 8\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts\n  method: get\n  operationId: getV1Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}\n  method: delete\n  operationId: deleteV1AccountsById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/connect/{platform}\n  method: post\n  operationId: postV1AccountsConnectByPlatform\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drafts\n  method: get\n  operationId: getV1Drafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts\n  method: post\n  operationId: postV1Drafts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drafts/{id}\n  method: get\n  operationId: getV1DraftsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts/{id}\n  method: patch\n  operationId: patchV1DraftsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/uploads\n  method: post\n  operationId: postV1MediaUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/{id}\n  method: get\n  operationId: getV1MediaById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts\n  method: get\n  operationId: getV1Posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts\n  method: post\n  operationId: postV1Posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}\n  method: get\n  operationId: getV1PostsById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/{id}\n  method: patch\n  operationId: patchV1PostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}\n  method: delete\n  operationId: deleteV1PostsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}/publish\n  method: post\n  operationId: postV1PostsByIdPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}/cancel\n  method: post\n  operationId: postV1PostsByIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/{id}/targets/{targetId}/retry\n  method: post\n  operationId: postV1PostsByIdTargetsByTargetIdRetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows\n  method: get\n  operationId: getV1Workflows\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows\n  method: post\n  operationId: postV1Workflows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{id}\n  method: get\n  operationId: getV1WorkflowsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows/{id}\n  method: put\n  operationId: putV1WorkflowsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{id}\n  method: delete\n  operationId: deleteV1WorkflowsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/postonce/agentic-access/postonce-agentic-access.yml
summary_line: 22 operations · 14 acting
tags:
- Company
- Social Media
- Automation
- Marketing
---
