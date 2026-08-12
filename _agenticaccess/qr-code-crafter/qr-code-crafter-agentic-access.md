---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 6
api_specs:
- filename: openapi.json
  format: json
  label: QRCodeCrafter API
  slug: qrcodecrafter-api
  spec_type: OpenAPI
  url: https://qrcodecrafter.com/.well-known/openapi.json
consequence_counts:
  physical: 1
  read: 6
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qr Code Crafter Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send-feedback
operation_count: 19
overview: 'QR Code Crafter exposes 19 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: QR Code Crafter
provider_slug: qr-code-crafter
slug: qr-code-crafter-agentic-access
source_filename: qr-code-crafter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: generated\nsource: openapi/qr-code-crafter-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 6\n    acting: 13\n  by_consequence:\n    read: 6\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /.netlify/functions/generate-qr\n  method: get\n  operationId: downloadQr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.netlify/functions/generate-qr\n  method: post\n  operationId: generateQr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.netlify/functions/generate-verified-qr\n  method: post\n  operationId: generateVerifiedQr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.netlify/functions/generate-qr-bulk\n  method: post\n  operationId: generateBulkQr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/send-feedback\n  method: post\n  operationId: sendFeedback\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr\n  method: post\n  operationId: createDynamicQr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr/{slug}\n  method: get\n  operationId: getDynamicQr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dynamic-qr/{slug}\n  method: patch\n  operationId: updateDynamicQr\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr/{slug}\n  method: delete\n  operationId: deleteDynamicQr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults\n  method: post\n  operationId: createDynamicQrVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults/{vaultId}\n  method: get\n  operationId:\
  \ getDynamicQrVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dynamic-qr-vaults/{vaultId}\n  method: patch\n  operationId: updateDynamicQrVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults/{vaultId}\n  method: delete\n  operationId: deleteDynamicQrVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults/{vaultId}/qr\n  method: post\n  operationId: createDynamicQrVaultChild\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults/{vaultId}/qr/{slug}\n  method: patch\n  operationId: updateDynamicQrVaultChild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dynamic-qr-vaults/{vaultId}/qr/{slug}/analytics\n  method: get\n  operationId: getDynamicQrVaultChildAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dynamic-qr-vaults/{vaultId}/qr/{slug}/analytics\n\
  \  method: delete\n  operationId: deleteDynamicQrVaultChild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /r/{slug}\n  method: get\n  operationId: redirectDynamicQr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r/{slug}\n  method: head\n  operationId: headDynamicQr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qr-code-crafter/refs/heads/main/agentic-access/qr-code-crafter-agentic-access.yml
summary_line: 19 operations · 13 acting
tags:
- QR code
- QR code generation
- static QR
- dynamic QR
- dynamic redirects
- image export
- bulk generation
- developer tools
- OpenAPI
- WebMCP
- browser agents
- payments (QR)
- agent readiness
- llms.txt
- capability tokens
---
