---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: webscraping-ai-account-api-openapi.yml
  format: yaml
  label: WebScraping.AI Account API
  slug: webscraping-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-account-api-openapi.yml
- filename: webscraping-ai-ai-api-openapi.yml
  format: yaml
  label: WebScraping.AI AI API
  slug: webscraping-ai-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-ai-api-openapi.yml
- filename: webscraping-ai-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI HTML API
  slug: webscraping-ai-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-html-api-openapi.yml
- filename: webscraping-ai-selected-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI Selected HTML API
  slug: webscraping-ai-selected-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-selected-html-api-openapi.yml
- filename: webscraping-ai-text-api-openapi.yml
  format: yaml
  label: WebScraping.AI Text API
  slug: webscraping-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-text-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Webscraping Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'WebScraping.AI exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WebScraping.AI
provider_slug: webscraping-ai
slug: webscraping-ai-agentic-access
source_filename: webscraping-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/webscraping-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ai/question\n  method: get\n  operationId: getQuestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/fields\n  method: get\n  operationId: getFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /html\n  method: get\n  operationId: getHTML\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /text\n  method: get\n  operationId: getText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /selected\n  method: get\n  operationId: getSelected\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /selected-multiple\n  method: get\n  operationId: getSelectedMultiple\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/agentic-access/webscraping-ai-agentic-access.yml
summary_line: 7 operations
tags:
- Web Scraping
- Data Extraction
- Proxies
- Artificial Intelligence
- Browser Automation
- Model Context Protocol
- Development
- Public APIs
- ai
- html
- mcp
- llm-tools
- structured-data
- headless-browser
- captcha
---
