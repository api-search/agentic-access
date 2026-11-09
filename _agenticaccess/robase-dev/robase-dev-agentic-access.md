---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: robase-dev-dashboard-api-openapi.yml
  format: yaml
  label: robase-dev Dashboard API
  slug: robase-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-dashboard-api-openapi.yml
- filename: robase-dev-otp-api-openapi.yml
  format: yaml
  label: robase-dev OTP API
  slug: robase-dev-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-otp-api-openapi.yml
- filename: robase-dev-sms-api-openapi.yml
  format: yaml
  label: robase-dev SMS API
  slug: robase-dev-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-sms-api-openapi.yml
- filename: robase-dev-system-api-openapi.yml
  format: yaml
  label: robase-dev System API
  slug: robase-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-system-api-openapi.yml
consequence_counts:
  physical: 3
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Robase Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /internal/auth/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/otp/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sms/send
operation_count: 9
overview: 'robase-dev exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: robase-dev
provider_slug: robase-dev
slug: robase-dev-agentic-access
source_filename: robase-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/robase-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    physical: 3\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/otp/send\n  method: post\n  operationId: sendOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/otp/verify\n  method: post\n  operationId: verifyOTP\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/otp/{id}\n  method: get\n  operationId: getOTP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/send\n  method: post\n  operationId: sendSMS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/{id}\n  method: get\n  operationId: getSMS\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/auth/signup\n  method: post\n  operationId: signupAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internal/auth/resend-verification\n  method: post\n  operationId: resendEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/robase-dev/agentic-access/robase-dev-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- SMS
- OTP
- Africa
- Messaging
- Communications
---
