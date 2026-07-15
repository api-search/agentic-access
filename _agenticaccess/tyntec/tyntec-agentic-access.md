---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Verification API
  slug: tyntec-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Information API
  slug: tyntec-number-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
consequence_counts:
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tyntec Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'tyntec exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tyntec
provider_slug: tyntec
slug: tyntec-agentic-access
source_filename: tyntec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tyntec-number-verification-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /verify/v1/phone/{number}\n  method: get\n  operationId: verifyPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/v1/templates\n  method: get\n  operationId: listVerifyTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /verify/v1/templates\n  method: post\n  operationId: createVerifyTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/v1/templates/{criteriaTemplateName}\n  method: get\n  operationId: getVerifyTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/v1/templates/{criteriaTemplateName}\n  method: put\n  operationId: updateVerifyTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/v1/templates/{criteriaTemplateName}\n\
  \  method: delete\n  operationId: deleteVerifyTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nis/v1/gnv\n  method: get\n  operationId: hlrLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nis/v1/gnp\n  method: get\n  operationId: numberPortabilityLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/v1/health\n  method: get\n  operationId: verifyHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/v1/version\n\
  \  method: get\n  operationId: verifyVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/agentic-access/tyntec-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Number Verification
- CPaaS
- SMS
- WhatsApp
- Phone Number Intelligence
- HLR Lookup
- Two-Factor Authentication
- OTP
- Messaging
- Number Portability
---
