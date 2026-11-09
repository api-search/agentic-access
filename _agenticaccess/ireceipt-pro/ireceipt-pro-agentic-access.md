---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: ireceipt-pro-jpg-api-openapi.yml
  format: yaml
  label: ireceipt-pro /jpg API
  slug: ireceipt-pro-jpg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-jpg-api-openapi.yml
- filename: ireceipt-pro-pdf-api-openapi.yml
  format: yaml
  label: ireceipt-pro /pdf API
  slug: ireceipt-pro-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-pdf-api-openapi.yml
- filename: ireceipt-pro-ping-api-openapi.yml
  format: yaml
  label: ireceipt-pro /ping API
  slug: ireceipt-pro-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-ping-api-openapi.yml
- filename: ireceipt-pro-png-api-openapi.yml
  format: yaml
  label: ireceipt-pro /png API
  slug: ireceipt-pro-png-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-png-api-openapi.yml
- filename: ireceipt-pro-webp-api-openapi.yml
  format: yaml
  label: ireceipt-pro /webp API
  slug: ireceipt-pro-webp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-webp-api-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ireceipt Pro Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'ireceipt-pro exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ireceipt-pro
provider_slug: ireceipt-pro
slug: ireceipt-pro-agentic-access
source_filename: ireceipt-pro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ireceipt-pro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /pdf/public/{template}\n  method: get\n  operationId: pdfGetPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf/public/{template}\n  method: post\n  operationId: pdfPostPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf/private/{template}\n  method: get\n  operationId: pdfGetPrivate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf/private/{template}\n  method: post\n  operationId: pdfPostPrivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jpg/public/{template}\n  method: get\n  operationId: jpgGetPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jpg/public/{template}\n  method: post\n  operationId: jpgPostPublic\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jpg/private/{template}\n  method: get\n  operationId: jpgGetPrivate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jpg/private/{template}\n  method: post\n  operationId: jpgPostPrivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /png/public/{template}\n  method: get\n  operationId: pngGetPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /png/public/{template}\n  method: post\n  operationId: pngPostPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /png/private/{template}\n  method: get\n  operationId: pngGetPrivate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /png/private/{template}\n  method: post\n  operationId: pngPostPrivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /webp/public/{template}\n  method: get\n  operationId: webpGetPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webp/public/{template}\n  method: post\n  operationId: webpPostPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webp/private/{template}\n  method: get\n  operationId: webpGetPrivate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webp/private/{template}\n  method: post\n  operationId: webpPostPrivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ping\n  method: get\n  operationId: pingGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ireceipt-pro/agentic-access/ireceipt-pro-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Company
- PDF
- Image Generation
- Templates
---
