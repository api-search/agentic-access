---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: networkcalc-binary-converter-api-openapi.yml
  format: yaml
  label: NetworkCalc Binary Converter API
  slug: networkcalc-binary-converter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-binary-converter-api-openapi.yml
- filename: networkcalc-dns-api-openapi.yml
  format: yaml
  label: NetworkCalc DNS API
  slug: networkcalc-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-dns-api-openapi.yml
- filename: networkcalc-encoder-api-openapi.yml
  format: yaml
  label: NetworkCalc Encoder API
  slug: networkcalc-encoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-encoder-api-openapi.yml
- filename: networkcalc-security-api-openapi.yml
  format: yaml
  label: NetworkCalc Security API
  slug: networkcalc-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-security-api-openapi.yml
- filename: networkcalc-subnet-calculator-api-openapi.yml
  format: yaml
  label: NetworkCalc Subnet Calculator API
  slug: networkcalc-subnet-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-subnet-calculator-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Networkcalc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'NetworkCalc exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NetworkCalc
provider_slug: networkcalc
slug: networkcalc-agentic-access
source_filename: networkcalc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/networkcalc-openapi-original.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /ip/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ipv6/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/lookup/{domain}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/scan/{host}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encoder/{type}/{value}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /binary/{value}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/agentic-access/networkcalc-agentic-access.yml
summary_line: 6 operations
tags:
- Networking
- DNS
- Security
- Subnetting
- Domains
- Calculator
---
