---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: powerreviews-readservices-openapi.yml
  format: yaml
  label: PowerReviews Read API
  slug: powerreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-readservices-openapi.yml
- filename: powerreviews-writeservices-openapi.yml
  format: yaml
  label: PowerReviews Write API
  slug: powerreviews-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-writeservices-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Powerreviews Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'PowerReviews exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PowerReviews
provider_slug: powerreviews
slug: powerreviews-agentic-access
source_filename: powerreviews-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/powerreviews-readservices-openapi.yml, openapi/powerreviews-writeservices-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /m/{merchantId}/l/{locale}/product/{pageIds}/snippet\n  method: get\n  operationId: getProductSnippetsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchantId}/l/{locale}/product/{pageId}/questions\n  method: get\n  operationId: getQuestionsUsingGET\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchantId}/l/{locale}/product/{pageId}/reviews\n  method: get\n  operationId: getProductReviewsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchantId}/reviews\n  method: get\n  operationId: getAllReviewsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchantId}/questions\n  method: get\n  operationId: getAllQuestionsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchantId}/l/{locale}/question/{questionId}/answers\n  method: get\n  operationId: getAnswersUsingGET\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /m/{merchant_id}/l/{locale}/configuration\n  method: get\n  operationId: getConfigurationByMerchantUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/b2b/answer\n  method: post\n  operationId: submitAnswerUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/b2b/merchant-response\n  method: post\n  operationId: submitMerchantResponseUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/b2b/question\n  method: post\n  operationId: submitQuestionUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/b2b/writereview/review_template\n  method: get\n  operationId: startReviewUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/b2b/writereview/submit_review\n  method: post\n  operationId: submitReviewUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/agentic-access/powerreviews-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- E-Commerce
- Ratings and Reviews
- User Generated Content
- Retail
- Marketing
- Syndication
- Questions and Answers
- Product Data
---
