---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
- filename: simon-data-contact-openapi.yml
  format: yaml
  label: Simon Data Contact API
  slug: simon-data-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-contact-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simon Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Simon Data exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simon Data
provider_slug: simon-data
slug: simon-data-agentic-access
source_filename: simon-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/simon-data-contact-openapi.yml, openapi/simon-data-event-ingestion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 1\n    acting: 1\n  by_consequence:\n    read: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collect\n  method: post\n  operationId: collectEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/agentic-access/simon-data-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
---
