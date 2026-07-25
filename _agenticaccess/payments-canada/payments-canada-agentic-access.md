---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: rtr-inbound-participant-payment-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Participant Payment API
  slug: rtr-inbound-participant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-participant-payment-api-openapi.yml
- filename: rtr-inbound-csp-heartbeat-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Exchange Heartbeat API
  slug: rtr-inbound-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
- filename: rtr-interest-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Interest Report API
  slug: rtr-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-interest-report-api-openapi.yml
- filename: rtr-balance-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Payment Capacity Balance Report API
  slug: rtr-balance-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-balance-report-api-openapi.yml
- filename: fif-extracts-api-openapi.yml
  format: yaml
  label: FIF Extracts API
  slug: fif-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-extracts-api-openapi.yml
- filename: fif-branch-api-openapi.yml
  format: yaml
  label: FIF Branch API
  slug: fif-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-branch-api-openapi.yml
- filename: ccin-extracts-api-openapi.yml
  format: yaml
  label: CCIN Extracts API
  slug: ccin-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-extracts-api-openapi.yml
- filename: ccin-lookup-api-openapi.yml
  format: yaml
  label: CCIN Lookup API
  slug: ccin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-lookup-api-openapi.yml
consequence_counts:
  physical: 3
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Payments Canada Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-capacity-balance-report
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/status
operation_count: 11
overview: 'Payments Canada exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Payments Canada
provider_slug: payments-canada
slug: payments-canada-agentic-access
source_filename: payments-canada-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/ccin-extracts-api-openapi.yml, openapi/ccin-lookup-api-openapi.yml, openapi/fif-branch-api-openapi.yml,\n  openapi/fif-extracts-api-openapi.yml, openapi/rtr-balance-report-api-openapi.yml, openapi/rtr-inbound-csp-heartbeat-api-openapi.yml,\n  openapi/rtr-inbound-participant-payment-api-openapi.yml, openapi/rtr-interest-report-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 6\n    acting: 5\n  by_consequence:\n    read: 6\n    physical: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/extracts/master\n  method: get\n  operationId: getMasterExtractUsingGET\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extracts/updated\n  method: get\n  operationId: getUpdateExtractUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ccins/{ccin}\n  method: get\n  operationId: getCcinByIdUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches/{dprn}\n  method: get\n  operationId: getBranchById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extracts/master\n  method: get\n  operationId: getMaster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extracts/updated\n\
  \  method: get\n  operationId: getUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-capacity-balance-report\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound-heartbeat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/status\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interest-report\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/agentic-access/payments-canada-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Financial Services
- Payments
- Canada
- Payment Infrastructure
- Clearing and Settlement
- Real-Time Rail
- ISO 20022
- Lynx
- Crown Corporation
- Faster Payments
---
