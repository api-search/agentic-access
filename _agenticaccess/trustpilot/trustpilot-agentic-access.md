---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 23
api_specs:
- filename: trustpilot-business-units-openapi.yml
  format: yaml
  label: Trustpilot Business Units API
  slug: trustpilot-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-business-units-openapi.yml
- filename: trustpilot-service-reviews-openapi.yml
  format: yaml
  label: Trustpilot Service Reviews API
  slug: trustpilot-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-service-reviews-openapi.yml
- filename: trustpilot-invitation-openapi.yml
  format: yaml
  label: Trustpilot Invitation API
  slug: trustpilot-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-invitation-openapi.yml
- filename: trustpilot-product-reviews-openapi.yml
  format: yaml
  label: Trustpilot Product Reviews API
  slug: trustpilot-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-product-reviews-openapi.yml
consequence_counts:
  physical: 1
  read: 23
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trustpilot Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/private/business-units/{businessUnitId}/email-invitations
operation_count: 38
overview: 'Trustpilot exposes 38 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trustpilot
provider_slug: trustpilot
slug: trustpilot-agentic-access
source_filename: trustpilot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/trustpilot-business-units-openapi.yml, openapi/trustpilot-invitation-openapi.yml,\n  openapi/trustpilot-product-reviews-openapi.yml, openapi/trustpilot-service-reviews-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 23\n    acting: 15\n  by_consequence:\n    read: 23\n    physical: 1\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/business-units/search\n  method: get\n  operationId: searchBusinessUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/profileinfo\n  method:\
  \ get\n  operationId: getBusinessUnitProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/reviews\n  method: get\n  operationId: getBusinessUnitReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/all-reviews\n  method: get\n  operationId: getAllBusinessUnitReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/business-units/{businessUnitId}/reviews\n  method: get\n  operationId: getPrivateBusinessUnitReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/images\n\
  \  method: get\n  operationId: getBusinessUnitImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/images/logo\n  method: get\n  operationId: getBusinessUnitLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/categories\n  method: get\n  operationId: getBusinessUnitCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-units/{businessUnitId}/web-links\n  method: get\n  operationId: getBusinessUnitWebLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/business-units/{businessUnitId}/templates\n\
  \  method: get\n  operationId: getInvitationTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/business-units/{businessUnitId}/email-invitations\n  method: post\n  operationId: sendEmailInvitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/business-units/{businessUnitId}/invitation-links\n  method: post\n  operationId: createInvitationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/business-units/{businessUnitId}/invitation-data/delete\n  method: post\n  operationId: deleteInvitationData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/product-reviews/business-units/{businessUnitId}\n  method: get\n  operationId: getProductReviewsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-reviews/business-units/{businessUnitId}/reviews\n  method: get\n  operationId: getProductReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/product-reviews/business-units/{businessUnitId}/batch-summaries\n  method: post\n  operationId: getBatchProductReviewsSummaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/product-reviews/business-units/{businessUnitId}/attribute-summaries\n  method: post\n  operationId: getBatchAttributeRatingSummaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/product-reviews/business-units/{businessUnitId}/reviews\n  method: get\n  operationId: getPrivateProductReviews\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/product-reviews/{reviewId}\n  method: get\n  operationId: getPrivateProductReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/product-reviews/{reviewId}/create-conversation\n  method: post\n  operationId: createProductReviewConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/product-reviews/business-units/{businessUnitId}/summaries\n  method: get\n  operationId: getPrivateProductReviewsSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/product-reviews/business-units/{businessUnitId}/invitation-links\n  method: post\n  operationId: createProductReviewInvitationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/conversations/{conversationId}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/conversations/{conversationId}/state\n  method: post\n  operationId: setConversationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/conversations/{conversationId}/comments\n  method: post\n  operationId: createConversationComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{conversationId}\n  method: get\n  operationId: getPublicConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/latest\n  method: get\n  operationId: getLatestReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{reviewId}\n\
  \  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{reviewId}/web-links\n  method: get\n  operationId: getReviewWebLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{reviewId}/likes\n  method: get\n  operationId: getReviewLikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/reviews/{reviewId}\n  method: get\n  operationId: getPrivateReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/reviews/{reviewId}/reply\n  method: post\n  operationId: createReviewReply\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/reviews/{reviewId}/reply\n  method: delete\n  operationId: deleteReviewReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/reviews/{reviewId}/tags\n  method: get\n  operationId: getReviewTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private/reviews/{reviewId}/tags\n  method: post\n  operationId: setReviewTags\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/reviews/{reviewId}/tags\n  method: put\n  operationId: addReviewTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/reviews/{reviewId}/tags\n  method: delete\n  operationId: deleteReviewTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private/reviews/{reviewId}/find-reviewer\n\
  \  method: post\n  operationId: findReviewer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/agentic-access/trustpilot-agentic-access.yml
summary_line: 38 operations · 15 acting
tags:
- Consumer Reviews
- Reviews
- Trust
- Ratings
- Business Profiles
- Product Reviews
---
