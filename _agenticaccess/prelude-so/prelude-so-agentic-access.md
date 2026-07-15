---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Verification API
  slug: prelude-so-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Lookup API
  slug: prelude-so-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Watch Anti-Fraud API
  slug: prelude-so-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
- filename: prelude-so-openapi.yml
  format: yaml
  label: Prelude Transactional Messaging API
  slug: prelude-so-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/openapi/prelude-so-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Prelude So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /watch/dispatch-events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watch/feedback
operation_count: 7
overview: 'Prelude exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 3 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prelude
provider_slug: prelude-so
slug: prelude-so-agentic-access
source_filename: prelude-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/prelude-so-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 3\n    read: 1\n    physical: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /verification\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/check\n  method: post\n  operationId: checkVerification\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup/{phone_number}\n  method: get\n  operationId: lookupPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watch/predict\n  method: post\n  operationId: predictWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/feedback\n  method: post\n  operationId: sendWatchFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/dispatch-events\n  method: post\n  operationId: dispatchWatchEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /notify\n  method: post\n  operationId: sendTransactionalMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prelude-so/refs/heads/main/agentic-access/prelude-so-agentic-access.yml
summary_line: 7 operations · 6 acting · 1 human-in-the-loop
tags:
- Number Verification
- Phone Verification
- OTP
- Authentication
- Anti-Fraud
- Two-Factor Authentication
- SMS
- Phone Number Lookup
---
