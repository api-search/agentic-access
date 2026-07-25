---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 1
api_specs:
- filename: cooperators-duuo-platform-openapi.yml
  format: yaml
  label: Duuo Platform API
  slug: duuo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/openapi/cooperators-duuo-platform-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cooperators Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/event/quote/{quoteId}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/tenant/quote/{quoteSubmissionId}/payment
operation_count: 10
overview: 'The Co-operators exposes 10 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Co-operators
provider_slug: cooperators
slug: cooperators-agentic-access
source_filename: cooperators-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/cooperators-duuo-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 9\n    connected: 1\n  by_consequence:\n    write: 7\n    read: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/event/entity\n  method: post\n  operationId: createEventEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/event/quote\n  method: post\n  operationId: createEventQuote\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/event/quote/{quoteId}\n  method: get\n  operationId: getEventQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/event/quote/{quoteId}/payment\n  method: post\n  operationId: createEventQuotePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/event/policy\n  method: post\n  operationId: createEventPolicy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/event/policy/{policyId}/email\n  method: put\n  operationId: emailEventPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tenant/eligibility\n  method: post\n  operationId: checkTenantEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/v1/tenant/quote/{quoteSubmissionId}\n  method: put\n  operationId: updateTenantQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tenant/quote/{quoteSubmissionId}/addinsured\n  method: put\n  operationId: addTenantQuoteInsured\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tenant/quote/{quoteSubmissionId}/payment\n  method: put\n  operationId: createTenantQuotePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/agentic-access/cooperators-agentic-access.yml
summary_line: 10 operations · 9 acting
tags:
- Insurance
- Canada
- Property and Casualty
- Life Insurance
- Group Benefits
- Embedded Insurance
- Co-operative
- Wealth Management
- Partner API
---
