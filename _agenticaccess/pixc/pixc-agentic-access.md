---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: schema
  format: yaml
  label: Pixc Public API
  slug: pixc-public-api
  spec_type: OpenAPI
  url: https://dashboard.pixc.com/v1/schema
consequence_counts:
  physical: 2
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pixc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/order/{orderId}
operation_count: 16
overview: 'Pixc exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pixc
provider_slug: pixc
slug: pixc-agentic-access
source_filename: pixc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/pixc-orders-api-openapi.yml, openapi/pixc-templates-api-openapi.yml, openapi/pixc-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    physical: 2\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/order\n  method: get\n  operationId: apiListOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:order:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order\n  method: post\n  operationId: apiAddOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - api:order:create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/order/{orderId}\n  method: get\n  operationId: apiShowOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:order:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/{orderId}\n  method: delete\n  operationId: apiCancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api:order:cancel\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/order/{orderId}/download\n  method: get\n  operationId: apiDownloadListOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:order:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/{orderId}/image\n  method: get\n  operationId: apiImageListOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:order:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/template\n  method: get\n  operationId: apiListTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:template:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/template\n  method: post\n  operationId: apiAddTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:template:create\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/template/{templateId}\n  method: get\n  operationId: apiShowTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:template:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/template/{templateId}\n  method: put\n  operationId: apiUpdateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:template:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/template/{templateId}\n  method: delete\n  operationId: apiRemoveTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    scope:\n    - api:template:remove\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhook\n  method: get\n  operationId: apiListWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api:webhook:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhook\n  method: post\n  operationId: apiAddWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:webhook:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhook/{webhookId}\n  method: get\n  operationId: apiShowWebhook\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - api:webhook:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhook/{webhookId}\n  method: put\n  operationId: apiUpdateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:webhook:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhook/{webhookId}\n  method: delete\n  operationId: apiRemoveWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:webhook:remove\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixc/refs/heads/main/agentic-access/pixc-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Company
- Shopify
- Ecommerce
- Photo Editing
- Image Optimization
- Image Processing
- Product Photography
- Background Removal
- SEO
- Automation
- AI
- Webhooks
- Digital Asset Management
---
