---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Scrape API
  slug: zenscrape-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Account API
  slug: zenscrape-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zenscrape Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Zenscrape exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zenscrape
provider_slug: zenscrape
slug: zenscrape-agentic-access
source_filename: zenscrape-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zenscrape-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /get\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/agentic-access/zenscrape-agentic-access.yml
summary_line: 2 operations
tags:
- Web Scraping
- Proxy
- HTML
- Data Extraction
- JavaScript Rendering
---
