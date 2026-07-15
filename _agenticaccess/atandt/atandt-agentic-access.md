---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 4
api_specs:
- filename: atandt-wireless-apis.yaml
  format: yaml
  label: AT&T Wireless APIs
  slug: att-wireless-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-wireless-apis.yaml
- filename: atandt-network-apis.yaml
  format: yaml
  label: AT&T 5G Network APIs
  slug: att-network-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-network-apis.yaml
- filename: atandt-enterprise-connectivity-apis.yaml
  format: yaml
  label: AT&T Enterprise Connectivity APIs
  slug: att-enterprise-connectivity-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-enterprise-connectivity-apis.yaml
consequence_counts:
  physical: 1
  read: 4
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atandt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /alliance/productOrder/v1
operation_count: 15
overview: 'AT&T exposes 15 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AT&T
provider_slug: atandt
slug: atandt-agentic-access
source_filename: atandt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atandt-enterprise-connectivity-apis.yaml, openapi/atandt-network-apis.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 11\n    connected: 4\n  by_consequence:\n    write: 10\n    physical: 1\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /alliance/serviceQualification/v1/check\n  method: post\n  operationId: checkServiceQualification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alliance/productOrder/v1\n\
  \  method: post\n  operationId: createProductOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alliance/productOrder/v1\n  method: get\n  operationId: listProductOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alliance/productOrder/v1/{orderId}\n  method: get\n  operationId: getProductOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sim-swap/v1/check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sim-swap/v1/retrieve-date\n  method: post\n  operationId: retrieveSimSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device-status/v1/connectivity\n  method: post\n  operationId: getDeviceConnectivityStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device-status/v1/roaming\n  method: post\n  operationId:\
  \ getDeviceRoamingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number-verification/v1/verify\n  method: post\n  operationId: verifyPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qod/v1/sessions\n  method: post\n  operationId: createQodSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /qod/v1/sessions\n  method: get\n  operationId: listQodSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qod/v1/sessions/{sessionId}\n  method: get\n  operationId: getQodSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qod/v1/sessions/{sessionId}\n  method: delete\n  operationId: deleteQodSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/insights/v1/metrics\n  method: post\n  operationId: getNetworkMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/threat-detection/v1/threats\n  method: post\n  operationId: getThreatAssessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/agentic-access/atandt-agentic-access.yml
summary_line: 15 operations · 11 acting
tags:
- Fortune 100
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
---
