---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: cloudwalk-checkout-links-api-openapi.yml
  format: yaml
  label: CloudWalk Checkout Links API
  slug: cloudwalk-checkout-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-checkout-links-api-openapi.yml
- filename: cloudwalk-infinitepay-checkout-api-api-openapi.yml
  format: yaml
  label: CloudWalk InfinitePay Checkout API
  slug: cloudwalk-infinitepay-checkout-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-infinitepay-checkout-api-api-openapi.yml
- filename: cloudwalk-payments-api-openapi.yml
  format: yaml
  label: CloudWalk Payments API
  slug: cloudwalk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-payments-api-openapi.yml
consequence_counts:
  physical: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudwalk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_check
operation_count: 2
overview: 'CloudWalk exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CloudWalk
provider_slug: cloudwalk
slug: cloudwalk-agentic-access
source_filename: cloudwalk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/cloudwalk-infinitepay-checkout-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /links\n  method: post\n  operationId: createCheckoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_check\n  method: post\n  operationId: checkPaymentStatus\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/agentic-access/cloudwalk-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Company
- Payments
- Financial-Services
- Fintech
- Checkout
- Point-of-Sale
- Acquiring
- Pix
- Brazil
- Banking
- Webhook
- Tap to Pay
---
