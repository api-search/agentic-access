---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 4
api_specs:
- filename: hitchpin-django-api-openapi.json
  format: json
  label: HitchPin Django API (Instant Invoicing)
  slug: hitchpin-django-api-instant-invoicing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-django-api-openapi.json
- filename: hitchpin-receipt-rendering-openapi.json
  format: json
  label: HitchPin Receipt Rendering Service
  slug: hitchpin-receipt-rendering-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-receipt-rendering-openapi.json
- filename: hitchpin-url-shortener-openapi.json
  format: json
  label: HitchPin URL Shortcode Service
  slug: hitchpin-url-shortcode-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-url-shortener-openapi.json
consequence_counts:
  physical: 3
  read: 4
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Hitchpin Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /instant-invoices/{invoice_number}/revoke/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /instant-invoice-share/{share_hash}/pay/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /instant-invoices/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /instant-invoices/{invoice_number}/share/
operation_count: 11
overview: 'HitchPin exposes 11 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 3 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HitchPin
provider_slug: hitchpin
slug: hitchpin-agentic-access
source_filename: hitchpin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/hitchpin-django-api-openapi.json, openapi/hitchpin-receipt-rendering-openapi.json,\n  openapi/hitchpin-url-shortener-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 4\n    acting: 7\n  by_consequence:\n    read: 4\n    physical: 3\n    safety-critical: 1\n    write: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /instant-invoice-share/{share_hash}/\n  method: get\n  operationId: retrieve_shared_instant_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-invoice-share/{share_hash}/pay/\n  method: post\n \
  \ operationId: pay_instant_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instant-invoice-share/{share_hash}/receipt/\n  method: get\n  operationId: get_instant_invoice_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-invoices/\n  method: get\n  operationId: list_instant_invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-invoices/\n  method: post\n  operationId: create_instant_invoices\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instant-invoices/{invoice_number}/\n  method: get\n  operationId: retrieve_instant_invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-invoices/{invoice_number}/revoke/\n  method: delete\n  operationId: void_instant_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /instant-invoices/{invoice_number}/share/\n  method:\
  \ post\n  operationId: share_instant_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render\n  method: put\n  operationId: RenderReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render-link\n  method: post\n  operationId: CreateReceiptUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: ShortenUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/agentic-access/hitchpin-agentic-access.yml
summary_line: 11 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Marketplace
- Agriculture
- Livestock
- Hay and Forage
- Farm Equipment
- Invoicing
- Payments
- Rural
---
