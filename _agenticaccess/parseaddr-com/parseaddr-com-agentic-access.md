---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
api_specs:
- filename: parseaddr-com-checkout-api-openapi.yml
  format: yaml
  label: parseaddr-com Checkout API
  slug: parseaddr-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-checkout-api-openapi.yml
- filename: parseaddr-com-credits-api-openapi.yml
  format: yaml
  label: parseaddr-com Credits API
  slug: parseaddr-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-credits-api-openapi.yml
- filename: parseaddr-com-expand-api-openapi.yml
  format: yaml
  label: parseaddr-com Expand API
  slug: parseaddr-com-expand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-expand-api-openapi.yml
- filename: parseaddr-com-health-api-openapi.yml
  format: yaml
  label: parseaddr-com Health API
  slug: parseaddr-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-health-api-openapi.yml
- filename: parseaddr-com-parse-api-openapi.yml
  format: yaml
  label: parseaddr-com Parse API
  slug: parseaddr-com-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-parse-api-openapi.yml
- filename: parseaddr-com-signup-api-openapi.yml
  format: yaml
  label: parseaddr-com Signup API
  slug: parseaddr-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-signup-api-openapi.yml
- filename: parseaddr-com-usage-api-openapi.yml
  format: yaml
  label: parseaddr-com Usage API
  slug: parseaddr-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-usage-api-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parseaddr Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 16
overview: 'parseaddr-com exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: parseaddr-com
provider_slug: parseaddr-com
slug: parseaddr-com-agentic-access
source_filename: parseaddr-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/api-parseaddr-com-openapi.json, openapi/parseaddr-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 6\n    acting: 10\n  by_consequence:\n    read: 6\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parse\n  method: post\n  operationId: parse_v1_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expand\n  method: post\n  operationId: expand_v1_expand_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signup\n  method: post\n  operationId: signup_v1_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout\n  method: post\n  operationId: create_checkout_v1_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/topup\n  method: post\n  operationId: credits_topup_v1_credits_topup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/key\n  method: get\n  operationId: checkout_key_v1_checkout_key_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parse\n  method: post\n  operationId: parse_v1_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expand\n  method: post\n  operationId: expand_v1_expand_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/signup\n  method: post\n  operationId: signup_v1_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout\n  method: post\n  operationId: create_checkout_v1_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/topup\n\
  \  method: post\n  operationId: credits_topup_v1_credits_topup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/key\n  method: get\n  operationId: checkout_key_v1_checkout_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/parseaddr-com/agentic-access/parseaddr-com-agentic-access.yml
summary_line: 16 operations · 10 acting
tags:
- Company
- Address
- Parsing
- libpostal
---
