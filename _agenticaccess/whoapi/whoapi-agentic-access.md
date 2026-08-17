---
acting_count: 0
action_class_counts:
  connected: 1
api_specs:
- filename: whoapi-domain-intelligence-api-openapi.yml
  format: yaml
  label: WhoAPI Domain Intelligence API
  slug: whoapi-domain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/openapi/whoapi-domain-intelligence-api-openapi.yml
consequence_counts:
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Whoapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'WhoAPI exposes 1 API operation that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WhoAPI
provider_slug: whoapi
slug: whoapi-agentic-access
source_filename: whoapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/whoapi-domain-intelligence-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    connected: 1\n  by_consequence:\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: queryWhoAPI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/agentic-access/whoapi-agentic-access.yml
summary_line: 1 operation
tags:
- Company
- Domains
- WHOIS
- Domain Availability
- SSL
- Email Verification
- Blacklist
- Cybersecurity
- Domain Intelligence
- Screenshots
- Reputation
---
