---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: seon-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Phone API
  slug: phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON IP API
  slug: ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON AML API
  slug: aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Scoring / Labels API
  slug: transaction-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
- filename: seon-openapi.yml
  format: yaml
  label: SEON Device Fingerprint
  slug: device-fingerprint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/openapi/seon-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Seon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'SEON exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SEON
provider_slug: seon
slug: seon-agentic-access
source_filename: seon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/seon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /SeonRestService/fraud-api/v2.0\n  method: post\n  operationId: scoreFraud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/email-api/v3\n  method: post\n  operationId: analyzeEmail\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/phone-api/v2\n  method: post\n  operationId: analyzePhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/ip-api/v1/{ip}\n  method: get\n  operationId: analyzeIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SeonRestService/aml-api/v1\n  method: post\n  operationId: screenAml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/fraud-api/transaction-label/v2\n  method: put\n  operationId: labelTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon/refs/heads/main/agentic-access/seon-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Fraud Prevention
- Risk Scoring
- Digital Footprint
- AML
- Identity
---
