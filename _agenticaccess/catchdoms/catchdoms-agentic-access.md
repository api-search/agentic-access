---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: catchdoms-domains-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Domains API
  slug: catchdoms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-domains-api-openapi.yml
- filename: catchdoms-free-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Free API
  slug: catchdoms-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-free-api-openapi.yml
- filename: catchdoms-pending-delete-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Pending Delete API
  slug: catchdoms-pending-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-pending-delete-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Catchdoms Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'CatchDoms Expired Domains API exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CatchDoms Expired Domains API
provider_slug: catchdoms
slug: catchdoms-agentic-access
source_filename: catchdoms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: generated\nsource: openapi/catchdoms-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /free/domains\n  method: get\n  operationId: freeDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pending-delete\n  method: get\n  operationId: listPendingDeleteDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pending-delete/{domain}\n  method: get\n  operationId: getPendingDeleteDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/agentic-access/catchdoms-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Domains
- SEO
- Expired
---
