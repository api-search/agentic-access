---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: mason-apps-api-openapi.yml
  format: yaml
  label: Mason Apps API
  slug: mason-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-apps-api-openapi.yml
- filename: mason-create-image-api-openapi.yml
  format: yaml
  label: Mason Create Image API
  slug: mason-create-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-create-image-api-openapi.yml
- filename: mason-images-api-openapi.yml
  format: yaml
  label: Mason Images API
  slug: mason-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-images-api-openapi.yml
- filename: mason-retrieve-an-image-api-openapi.yml
  format: yaml
  label: Mason Retrieve an Image API
  slug: mason-retrieve-an-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-retrieve-an-image-api-openapi.yml
- filename: mason-search-api-openapi.yml
  format: yaml
  label: Mason Search API
  slug: mason-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-search-api-openapi.yml
- filename: mason-template-mappings-api-openapi.yml
  format: yaml
  label: Mason Template Mappings API
  slug: mason-template-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-template-mappings-api-openapi.yml
- filename: mason-tiered-discounts-api-openapi.yml
  format: yaml
  label: Mason Tiered Discounts API
  slug: mason-tiered-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-tiered-discounts-api-openapi.yml
- filename: mason-webhooks-api-openapi.yml
  format: yaml
  label: Mason Webhooks API
  slug: mason-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-webhooks-api-openapi.yml
consequence_counts:
  read: 5
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mason Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Mason exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mason
provider_slug: mason
slug: mason-agentic-access
source_filename: mason-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mason-apps-openapi.json, openapi/mason-discounts-openapi.json, openapi/mason-generation-openapi.json,\n  openapi/mason-search-openapi.json, openapi/mason-tasks-openapi.json, openapi/mason-webhooks-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 11\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/app\n  method: post\n  operationId: Create_an_app_v1_app_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app\n  method: get\n  operationId: Get_app_v1_app_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{app_id}\n  method: delete\n  operationId: Delete_app_v1_app__app_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scrooge/tiered-discounts\n  method: put\n  operationId: create_tiered_discounts_api_v1_scrooge_tiered_discounts_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scrooge/discounts/bulk\n  method: put\n  operationId: create_bulk_discounts_api_v1_scrooge_discounts_bulk_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scrooge/discounts/bulk/delete\n  method: put\n  operationId: cleanup_tiered_discounts_api_v1_scrooge_discounts_bulk_delete_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scrooge/tiered-discounts/delete\n  method: put\n  operationId: cleanup_tiered_discounts_api_v1_scrooge_tiered_discounts_delete_put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/images\n  method: post\n  operationId: Generation_api_v1_genie_images_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/images/{uid}\n  method: get\n  operationId: Get_Image_api_v1_genie_images__uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/template/{template_id}\n  method: get\n  operationId: Get_Template_Mappings_api_v1_genie_template__template_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: Asset_Search_v1_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/creative\n  method: post\n  operationId: Creative_task_v1_task_creative_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/creative/status\n  method: post\n  operationId: Creative_task_status_v1_creative_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook\n  method: post\n  operationId: Register_a_Webhook_v1_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook\n  method: get\n  operationId: Get_Webhook_v1_webhook_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/{id}\n  method: delete\n  operationId: Delete_Webhook_v1_webhook__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/agentic-access/mason-agentic-access.yml
summary_line: 16 operations · 11 acting
tags:
- Company
- E-Commerce
- Commerce
- Artificial Intelligence
- Agents
- Content Generation
- Discounts
- Promotions
- Webhook
- Shopify
---
