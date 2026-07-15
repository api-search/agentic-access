---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: IP Reputation & Proxy/VPN Detection API
  slug: ip-reputation-proxy-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Email Validation API
  slug: email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Phone Number Validation API
  slug: phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Malicious URL Scanner API
  slug: malicious-url-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Device Fingerprint API
  slug: device-fingerprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Transaction Scoring API
  slug: transaction-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Leaked Data (Dark Web) API
  slug: leaked-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ipqualityscore Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'IPQualityScore exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IPQualityScore
provider_slug: ipqualityscore
slug: ipqualityscore-agentic-access
source_filename: ipqualityscore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ipqualityscore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ip/{api_key}/{ip}\n  method: get\n  operationId: proxyDetection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/{api_key}/{email}\n  method: get\n  operationId: emailValidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone/{api_key}/{phone}\n\
  \  method: get\n  operationId: phoneValidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /url/{api_key}/{url}\n  method: get\n  operationId: maliciousUrlScanner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fingerprint/{api_key}\n  method: post\n  operationId: deviceFingerprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leaked/{type}/{api_key}\n  method: get\n  operationId: leakedData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/agentic-access/ipqualityscore-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Fraud Prevention
- IP Reputation
- Proxy Detection
- Email Validation
- Threat Intelligence
---
