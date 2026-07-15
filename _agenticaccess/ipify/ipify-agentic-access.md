---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: ipify-ip-api.yml
  format: yaml
  label: ipify Public IP Address API
  slug: ipify-public-ip-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-ip-api.yml
- filename: ipify-geolocation-api.yml
  format: yaml
  label: ipify IP Geolocation API
  slug: ipify-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-geolocation-api.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ipify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'ipify exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ipify
provider_slug: ipify
slug: ipify-agentic-access
source_filename: ipify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ipify-geolocation-api.yml, openapi/ipify-ip-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /country\n  method: get\n  operationId: getCountryLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country,city\n  method: get\n  operationId: getCountryCityLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country,city,vpn\n  method:\
  \ get\n  operationId: getCountryCityVpnLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service/account-balance\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getPublicIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/agentic-access/ipify-agentic-access.yml
summary_line: 5 operations
tags:
- Development
- IP Address
- Geolocation
- IP Intelligence
- Public APIs
---
