---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 15
api_specs:
- filename: customer-alliance-analytics-api-openapi.yml
  format: yaml
  label: Customer Alliance Analytics API
  slug: customer-alliance-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-analytics-api-openapi.yml
- filename: customer-alliance-guests-api-openapi.yml
  format: yaml
  label: Customer Alliance Guests API
  slug: customer-alliance-guests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-guests-api-openapi.yml
- filename: customer-alliance-identity-api-openapi.yml
  format: yaml
  label: Customer Alliance Identity API
  slug: customer-alliance-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-identity-api-openapi.yml
- filename: customer-alliance-insights-api-openapi.yml
  format: yaml
  label: Customer Alliance Insights API
  slug: customer-alliance-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-insights-api-openapi.yml
- filename: customer-alliance-nodes-api-openapi.yml
  format: yaml
  label: Customer Alliance Nodes API
  slug: customer-alliance-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-nodes-api-openapi.yml
- filename: customer-alliance-reviews-api-openapi.yml
  format: yaml
  label: Customer Alliance Reviews API
  slug: customer-alliance-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-reviews-api-openapi.yml
- filename: customer-alliance-surveys-api-openapi.yml
  format: yaml
  label: Customer Alliance Surveys API
  slug: customer-alliance-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-surveys-api-openapi.yml
- filename: customer-alliance-webhook-events-api-openapi.yml
  format: yaml
  label: Customer Alliance Webhook events API
  slug: customer-alliance-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-webhook-events-api-openapi.yml
- filename: customer-alliance-webhooks-api-openapi.yml
  format: yaml
  label: Customer Alliance Webhooks API
  slug: customer-alliance-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customer-alliance/openapi/customer-alliance-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Customer Alliance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{id}/test
operation_count: 22
overview: 'Customer Alliance exposes 22 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Customer Alliance
provider_slug: customer-alliance
slug: customer-alliance-agentic-access
source_filename: customer-alliance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/customer-alliance.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 15\n    acting: 7\n  by_consequence:\n    read: 15\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: get\n  operationId: listReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: post\n  operationId:\
  \ pushReviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews/{id}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/scores\n  method: get\n  operationId: getAnalyticsScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes\n  method: get\n  operationId: listNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property-attributes\n  method: get\n  operationId: listPropertyAttributes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}\n  method: get\n  operationId: getSurvey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/responses\n  method: get\n  operationId: listSurveyResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/responses/{responseId}/answers\n  method: get\n  operationId: listResponseAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /survey-responses\n  method: post\n  operationId: pushSurveyResponses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/recommendations\n  method: get\n  operationId: listRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/mentions\n  method: get\n  operationId: listMentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/topics\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /guests\n  method: post\n  operationId: pushGuest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/customer-alliance/agentic-access/customer-alliance-agentic-access.yml
summary_line: 22 operations · 7 acting
tags:
- Company
- Hospitality
- Review Management
- Software-as-a-Service
- Hotels
---
