---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 10
api_specs:
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Invitations / Collect API
  slug: invitations-collect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Product Reviews API
  slug: product-reviews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Company Reviews API
  slug: company-reviews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Ratings / Widgets API
  slug: ratings-widgets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Questions API
  slug: questions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
- filename: reviews-io-openapi.yml
  format: yaml
  label: REVIEWS.io Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-openapi.yml
consequence_counts:
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reviews Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'REVIEWS.io exposes 16 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: REVIEWS.io
provider_slug: reviews-io
slug: reviews-io-agentic-access
source_filename: reviews-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/reviews-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 6\n    connected: 10\n  by_consequence:\n    write: 6\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /invitation\n  method: post\n  operationId: queueProductInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/invitation\n  method: post\n  operationId: queueProductInvitationOnly\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/invitation\n  method: get\n  operationId: listProductInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/invitation\n  method: post\n  operationId: queueCompanyInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/invitation\n  method: get\n  operationId: listCompanyInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/reviews\n  method: get\n  operationId: retrieveCompanyReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/review\n  method: get\n  operationId: retrieveProductReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/review/new\n  method: post\n  operationId: createProductReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/vote\n  method: get\n  operationId: voteProductReview\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/rating-batch\n  method: get\n  operationId: retrieveProductRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/all\n  method: get\n  operationId: retrieveReviewStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions/store\n  method: post\n  operationId: createQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews\n  method: get\n  operationId: retrieveReviewsAndQuestions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ugc\n  method: get\n  operationId: retrieveUserGeneratedContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/add\n  method: post\n  operationId: addWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/list\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/agentic-access/reviews-io-agentic-access.yml
summary_line: 16 operations · 6 acting
tags:
- Reviews
- UGC
- Ratings
- Reputation
- eCommerce
---
