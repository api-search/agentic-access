---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 16
api_specs:
- filename: yoast-pages-api-openapi.yml
  format: yaml
  label: Yoast Pages API
  slug: yoast-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-pages-api-openapi.yml
- filename: yoast-posts-api-openapi.yml
  format: yaml
  label: Yoast Posts API
  slug: yoast-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-posts-api-openapi.yml
- filename: yoast-seo-head-api-openapi.yml
  format: yaml
  label: Yoast SEO Head API
  slug: yoast-seo-head-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-seo-head-api-openapi.yml
- filename: yoast-abilities-api-openapi.yml
  format: yaml
  label: Yoast SEO Abilities API
  slug: yoast-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-abilities-api-openapi.yml
- filename: yoast-provisioning-account-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Account API
  slug: yoast-provisioning-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-account-api-openapi.yml
- filename: yoast-provisioning-downloads-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Downloads API
  slug: yoast-provisioning-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-downloads-api-openapi.yml
- filename: yoast-provisioning-users-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Users API
  slug: yoast-provisioning-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-users-api-openapi.yml
- filename: yoast-schema-aggregator-api-openapi.yml
  format: yaml
  label: Yoast Schema Aggregator API
  slug: yoast-schema-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-schema-aggregator-api-openapi.yml
- filename: yoast-subscription-provisioning-api-openapi.yml
  format: yaml
  label: Yoast Subscription Provisioning API
  slug: yoast-subscription-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-subscription-provisioning-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Yoast Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/account/regenerate-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/subscriptions/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/subscriptions/{id}/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/subscriptions/{id}/refund
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/subscriptions/{id}/renew
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/subscriptions/{id}/set-site
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/provisioning/user/schedule-delete
operation_count: 23
overview: 'Yoast exposes 23 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yoast
provider_slug: yoast
slug: yoast-agentic-access
source_filename: yoast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/yoast-abilities-api-openapi.yml, openapi/yoast-pages-api-openapi.yml, openapi/yoast-posts-api-openapi.yml,\n  openapi/yoast-provisioning-account-api-openapi.yml, openapi/yoast-provisioning-downloads-api-openapi.yml,\n  openapi/yoast-provisioning-users-api-openapi.yml, openapi/yoast-schema-aggregator-api-openapi.yml,\n  openapi/yoast-seo-head-api-openapi.yml, openapi/yoast-subscription-provisioning-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 16\n    acting: 7\n  by_consequence:\n    read: 16\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /wp-abilities/v1/abilities\n  method: get\n  operationId:\
  \ listAbilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-abilities/v1/abilities/yoast-seo/get-seo-scores/run\n  method: get\n  operationId: runGetSeoScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-abilities/v1/abilities/yoast-seo/get-readability-scores/run\n  method: get\n  operationId: runGetReadabilityScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-abilities/v1/abilities/yoast-seo/get-inclusive-language-scores/run\n  method: get\n  operationId: runGetInclusiveLanguageScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n\
  \  method: get\n  operationId: listPagesWithSeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPageWithSeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPostsWithSeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPostWithSeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/provisioning/account/regenerate-token\n  method: post\n  operationId: provisioningAccountControllerRegenerateToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/provisioning/downloads/currentVersion\n  method: get\n  operationId: provisioningDownloadsControllerCurrentVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/provisioning/downloads/currentVersion\n  method: get\n  operationId: provisioningDownloadsControllerCurrentVersionV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/provisioning/downloads/currentZip\n  method: get\n  operationId: provisioningDownloadsControllerCurrentZip\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/provisioning/user/schedule-delete\n  method: post\n  operationId: provisioningUsersControllerScheduleDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /yoast/v1/schema-aggregator/get-schema/{post_type}\n  method: get\n  operationId: getAggregatedSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/schema-aggregator/get-schema/{post_type}/{page}\n  method: get\n  operationId: getAggregatedSchemaPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/schema-aggregator/get-xml\n  method: get\n  operationId: getSchemaMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/provisioning/subscriptions/create\n  method: post\n  operationId: subscriptionProvisioningControllerCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/provisioning/subscriptions/{id}\n\
  \  method: get\n  operationId: subscriptionProvisioningControllerGetOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/provisioning/subscriptions/{id}/renew\n  method: post\n  operationId: subscriptionProvisioningControllerRenewSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/provisioning/subscriptions/{id}/cancel\n  method: post\n  operationId: subscriptionProvisioningControllerCancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/provisioning/subscriptions/{id}/refund\n  method: post\n  operationId: subscriptionProvisioningControllerRefundSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/provisioning/subscriptions/{id}/set-site\n  method: post\n  operationId: subscriptionProvisioningControllerSetSiteForSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/agentic-access/yoast-agentic-access.yml
summary_line: 23 operations · 7 acting · 7 human-in-the-loop
tags:
- SEO
- WordPress
- Content Optimization
- Schema
- Metadata
- Structured Data
- Headless CMS
- Content Analysis
- Agent Readiness
- Plugins
---
