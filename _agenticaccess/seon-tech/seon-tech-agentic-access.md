---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON Phone API
  slug: phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON IP API
  slug: ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON BIN API
  slug: bin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
- filename: seon-tech-openapi.yml
  format: yaml
  label: SEON AML API
  slug: aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/openapi/seon-tech-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Seon Tech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'SEON exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SEON
provider_slug: seon-tech
slug: seon-tech-agentic-access
source_filename: seon-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/seon-tech-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /SeonRestService/fraud-api/v2/\n  method: post\n  operationId: submitFraudCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/email-api/v3\n  method: post\n  operationId: enrichEmail\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/phone-api/v2\n  method: post\n  operationId: enrichPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SeonRestService/ip-api/v1/{ip}\n  method: get\n  operationId: lookupIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SeonRestService/bin-api/v1/{bin}\n  method: get\n  operationId: lookupBin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SeonRestService/aml-api/v1\n  method: post\n  operationId: submitAmlCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon-tech/refs/heads/main/agentic-access/seon-tech-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- AML Compliance
- Device Intelligence
- Digital Footprint
- Fraud Prevention
- Identity Verification
- Risk Scoring
---
