---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 2
api_specs:
- filename: qbe-anzo-digital-brokers-openapi.yml
  format: yaml
  label: QBE Australia ANZO Digital Brokers Experience API
  slug: qbe-anzo-digital-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-anzo-digital-brokers-openapi.yml
- filename: qbe-ctp-switch-service-openapi.yml
  format: yaml
  label: QBE Australia CTP Switch Service
  slug: qbe-ctp-switch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-ctp-switch-service-openapi.yml
consequence_counts:
  read: 2
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qbe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'QBE Insurance exposes 17 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: QBE Insurance
provider_slug: qbe
slug: qbe-agentic-access
source_filename: qbe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/qbe-anzo-digital-brokers-openapi.yml, openapi/qbe-ctp-switch-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 2\n    acting: 15\n  by_consequence:\n    read: 2\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /__health\n  method: get\n  operationId: get-__health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-model\n  method: post\n  operationId: post-data-model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/abandon\n  method: post\n  operationId: To-Abandon-a-policy-before-it-has-been-bound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes/{quoteId}/abandon\n  method: post\n  operationId: To-Abandon-an-existing-quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/endorse\n  method: post\n  operationId: Amend-an-existing-policy-endorsement\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/bind\n  method: post\n  operationId: Bind-a-policy-to-save-change-after-endoresement-cancellation-or-renewal-has\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/cancel\n  method: post\n  operationId: Cancel-an-existing-policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes/{quoteId}/bind\n  method: post\n  operationId: Convert-a-Quote-to-Policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes\n  method: post\n  operationId: Create-a-new-Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/renew\n  method: post\n  operationId: Generate-a-quote-request-for-a-policy-that-has-been-invited-for-renewal\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes/{quoteId}\n  method: put\n  operationId: Modify-an-existing-Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/documents\n  method: post\n  operationId: Policy-Document-Upload-API\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes/{quoteId}/documents\n\
  \  method: post\n  operationId: Quote-Document-Upload-API\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/quotes/{quoteId}/refer\n  method: post\n  operationId: Refer-a-quote-to-QBE-Underwriter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/policies/{policyId}/refer\n  method: post\n  operationId: Refer-an-existing-Policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ctp-documents/appenddata\n  method: post\n  operationId: append-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ctp-documents/saveddata\n  method: get\n  operationId: get-saved-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/agentic-access/qbe-agentic-access.yml
summary_line: 17 operations · 15 acting
tags:
- Insurance
- Australia
- Property and Casualty
- Commercial Insurance
- Underwriting
- Policy Administration
- Quotes
- Brokers
- Reinsurance
- Carrier
- Partner API
---
