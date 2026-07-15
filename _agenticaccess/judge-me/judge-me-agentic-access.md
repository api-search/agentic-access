---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviews API
  slug: judge-me-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviewers API
  slug: judge-me-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Products API
  slug: judge-me-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Widgets API
  slug: judge-me-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me OAuth API
  slug: judge-me-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Webhooks API
  slug: judge-me-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Judge Me Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/send_manual_review_request
operation_count: 6
overview: 'Judge.me exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Judge.me
provider_slug: judge-me
slug: judge-me-agentic-access
source_filename: judge-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/judge-me-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /reviews\n  method: get\n  operationId: listReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: post\n  operationId: createReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/-1\n  method: get\n  operationId: lookupProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /widgets/product_review\n  method: get\n  operationId: getProductReviewWidget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /widgets/preview_badge\n  method: get\n  operationId: getPreviewBadgeWidget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/send_manual_review_request\n  method: post\n  operationId: sendManualReviewRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/agentic-access/judge-me-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Reviews
- E-commerce
- Shopify
- Ratings
- Social Proof
---
