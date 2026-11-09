---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 14
api_specs:
- filename: irmu-com-booking-api-openapi.yml
  format: yaml
  label: Irmu Booking API
  slug: irmu-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-booking-api-openapi.yml
- filename: irmu-com-crawl-api-openapi.yml
  format: yaml
  label: Irmu Crawl API
  slug: irmu-com-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-crawl-api-openapi.yml
- filename: irmu-com-google-api-openapi.yml
  format: yaml
  label: Irmu Google API
  slug: irmu-com-google-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-google-api-openapi.yml
- filename: irmu-com-screenshot-api-openapi.yml
  format: yaml
  label: Irmu Screenshot API
  slug: irmu-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-screenshot-api-openapi.yml
- filename: irmu-com-chat-gpt-api-openapi.yml
  format: yaml
  label: Irmu Chat GPT API
  slug: irmu-com-chat-gpt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-chat-gpt-api-openapi.yml
consequence_counts:
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Irmu Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Irmu exposes 16 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Irmu
provider_slug: irmu-com
slug: irmu-com-agentic-access
source_filename: irmu-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/app.irmu.com.yaml, openapi/irmu-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 14\n    acting: 2\n  by_consequence:\n    read: 14\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /crawl\n  method: get\n  operationId: crawl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crawl\n  method: post\n  operationId: crawlRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crawl/{job}\n  method: get\n  operationId: crawlPoll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatgpt\n  method: get\n  operationId: chatgpt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screenshot\n  method: get\n  operationId: screenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/search\n  method: get\n  operationId: bookingSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/hotel\n  method: get\n  operationId: bookingHotel\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-ai-overview\n  method: get\n  operationId: googleAiOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crawl\n  method: get\n  operationId: crawl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crawl\n  method: post\n  operationId: crawlRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crawl/{job}\n  method: get\n  operationId: crawlPoll\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatgpt\n  method: get\n  operationId: chatgpt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screenshot\n  method: get\n  operationId: screenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/search\n  method: get\n  operationId: bookingSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/hotel\n  method: get\n  operationId: bookingHotel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-ai-overview\n  method: get\n  operationId: googleAiOverview\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/irmu-com/agentic-access/irmu-com-agentic-access.yml
summary_line: 16 operations · 2 acting
tags:
- Web Scraping
- Developer Tools
- Automation
- Data Extraction
- Company
---
