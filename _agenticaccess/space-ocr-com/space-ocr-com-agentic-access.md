---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: space-ocr-com-amount-api-openapi.yml
  format: yaml
  label: space-ocr-com Amount API
  slug: space-ocr-com-amount-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-amount-api-openapi.yml
- filename: space-ocr-com-create-api-openapi.yml
  format: yaml
  label: space-ocr-com Create API
  slug: space-ocr-com-create-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-create-api-openapi.yml
- filename: space-ocr-com-edit-api-openapi.yml
  format: yaml
  label: space-ocr-com Edit API
  slug: space-ocr-com-edit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-edit-api-openapi.yml
- filename: space-ocr-com-health-api-openapi.yml
  format: yaml
  label: space-ocr-com Health API
  slug: space-ocr-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-health-api-openapi.yml
- filename: space-ocr-com-jobs-api-openapi.yml
  format: yaml
  label: space-ocr-com Jobs API
  slug: space-ocr-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-jobs-api-openapi.yml
- filename: space-ocr-com-ocr-api-openapi.yml
  format: yaml
  label: space-ocr-com Ocr API
  slug: space-ocr-com-ocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-ocr-api-openapi.yml
- filename: space-ocr-com-remove-api-openapi.yml
  format: yaml
  label: space-ocr-com Remove API
  slug: space-ocr-com-remove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-remove-api-openapi.yml
- filename: space-ocr-com-space-api-openapi.yml
  format: yaml
  label: space-ocr-com Space API
  slug: space-ocr-com-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-space-api-openapi.yml
- filename: space-ocr-com-upload-api-openapi.yml
  format: yaml
  label: space-ocr-com Upload API
  slug: space-ocr-com-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-upload-api-openapi.yml
- filename: space-ocr-com-view-api-openapi.yml
  format: yaml
  label: space-ocr-com View API
  slug: space-ocr-com-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-view-api-openapi.yml
- filename: space-ocr-com-webhook-api-openapi.yml
  format: yaml
  label: space-ocr-com Webhook API
  slug: space-ocr-com-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-webhook-api-openapi.yml
- filename: space-ocr-com-webhooks-api-openapi.yml
  format: yaml
  label: space-ocr-com Webhooks API
  slug: space-ocr-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/space-ocr-com/openapi/space-ocr-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Space Ocr Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ocr/text
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhook/test
operation_count: 23
overview: 'space-ocr-com exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: space-ocr-com
provider_slug: space-ocr-com
slug: space-ocr-com-agentic-access
source_filename: space-ocr-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/space-ocr-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 9\n    acting: 14\n  by_consequence:\n    read: 9\n    write: 12\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /amount\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/fields\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ocr/markdown\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ocr/text\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /space\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /create\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload/ticket\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /upload/direct\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload/direct\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remove\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /view\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method:\
  \ put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/test\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/deliveries\n \
  \ method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/deliveries/{deliveryId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/deliveries/{deliveryId}/redeliver\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/space-ocr-com/agentic-access/space-ocr-com-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- OCR
- Artificial Intelligence
- Document Processing
- Field-Extraction
---
