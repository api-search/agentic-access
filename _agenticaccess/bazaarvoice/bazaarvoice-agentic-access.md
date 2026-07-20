---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: bazaarvoice-content-search-openapi.json
  format: json
  label: Bazaarvoice Content Search API
  slug: bazaarvoice-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-content-search-openapi.json
consequence_counts:
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bazaarvoice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Bazaarvoice exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bazaarvoice
provider_slug: bazaarvoice
slug: bazaarvoice-agentic-access
source_filename: bazaarvoice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bazaarvoice-content-search-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 8\n    connected: 7\n  by_consequence:\n    write: 8\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /lookahead\n  method: post\n  operationId: catalogLookaheadSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{clientId}/contributors/{contributorExternalId}\n  method: get\n  operationId: clientGetSingularContributor\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contributor\n  method: post\n  operationId: contributorLookaheadSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{legacyInternalId}\n  method: get\n  operationId: getQuestionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{clientId}/questions/{legacyInternalId}\n  method: get\n  operationId: getQuestionByIdAndClientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions/{legacyInternalId}/answers\n\
  \  method: post\n  operationId: getQuestionsUsingPOSTAndQuestionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews/{legacyInternalId}\n  method: get\n  operationId: getReviewById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{clientId}/reviews/{legacyInternalId}\n  method: get\n  operationId: getReviewByIdAndClientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contributors/{contributorExternalId}\n  method: get\n  operationId: getSingularContributor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contributors/{contributorExternalId}\n  method: post\n  operationId: searchContributors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{client-id}/ugc\n  method: get\n  operationId: getStructuredDataV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions\n  method: post\n  operationId: searchQuestionsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{clientId}/questions\n  method: post\n  operationId: searchQuestionsUsingPOSTAndClientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews\n  method: post\n  operationId: searchReviewsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{clientId}/reviews\n  method: post\n  operationId: searchReviewsUsingPOSTAndClientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/agentic-access/bazaarvoice-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Company
- Reviews
- Ratings
- User Generated Content
- Retail
- eCommerce
- Product Reviews
- Syndication
- Social Commerce
- SEO
---
