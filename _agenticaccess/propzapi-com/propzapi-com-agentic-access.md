---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: propzapi-com-account-api-openapi.yml
  format: yaml
  label: propzapi-com Account API
  slug: propzapi-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propzapi-com/openapi/propzapi-com-account-api-openapi.yml
- filename: propzapi-com-billing-api-openapi.yml
  format: yaml
  label: propzapi-com Billing API
  slug: propzapi-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propzapi-com/openapi/propzapi-com-billing-api-openapi.yml
- filename: propzapi-com-images-api-openapi.yml
  format: yaml
  label: propzapi-com Images API
  slug: propzapi-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propzapi-com/openapi/propzapi-com-images-api-openapi.yml
- filename: propzapi-com-meta-api-openapi.yml
  format: yaml
  label: propzapi-com Meta API
  slug: propzapi-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propzapi-com/openapi/propzapi-com-meta-api-openapi.yml
- filename: propzapi-com-qr-api-openapi.yml
  format: yaml
  label: propzapi-com Qr API
  slug: propzapi-com-qr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propzapi-com/openapi/propzapi-com-qr-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Propzapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/subscribe
operation_count: 22
overview: 'propzapi-com exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: propzapi-com
provider_slug: propzapi-com
slug: propzapi-com-agentic-access
source_filename: propzapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/propzapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: head\n  operationId: health_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/og-preview\n\
  \  method: get\n  operationId: og_preview_v1_og_preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates\n  method: get\n  operationId: list_templates_v1_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates\n  method: post\n  operationId: create_template_ep_v1_templates_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images\n  method: post\n  operationId: create_image_v1_images_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/qr\n  method: post\n  operationId: qr_create_v1_qr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/qr\n  method: get\n  operationId: qr_list_v1_qr_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/qr/{code}\n  method: patch\n  operationId: qr_update_v1_qr__code__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/qr/{code}\n  method: delete\n  operationId: qr_delete_v1_qr__code__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/qr/{code}/analytics\n  method: get\n  operationId: qr_stats_v1_qr__code__analytics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/batch\n  method: post\n  operationId: create_images_batch_v1_images_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot\n  method: post\n  operationId: create_screenshot_v1_screenshot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/preview\n  method: post\n  operationId: preview_template_v1_templates_preview_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embed-url\n  method: post\n  operationId: embed_url_v1_embed_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{tid}\n  method: get\n  operationId: get_template_ep_v1_templates__tid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{tid}\n  method: patch\n  operationId: update_template_ep_v1_templates__tid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{tid}\n  method: delete\n  operationId: delete_template_ep_v1_templates__tid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/register\n  method: post\n  operationId: register_v1_register_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: account_v1_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/subscribe\n  method: post\n  operationId: subscribe_billing_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /billing/topup\n  method: post\n  operationId: topup_billing_topup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/propzapi-com/agentic-access/propzapi-com-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Company
- Image Generation
- Rendering
- AI Agents
---
