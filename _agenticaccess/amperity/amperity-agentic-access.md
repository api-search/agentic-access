---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 15
api_specs:
- filename: amperity-control-plane-2024-04-01-openapi.json
  format: json
  label: Amperity API
  slug: amperity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-control-plane-2024-04-01-openapi.json
- filename: amperity-control-plane-unstable-openapi.json
  format: json
  label: Amperity API (Unstable)
  slug: amperity-api-unstable
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-control-plane-unstable-openapi.json
consequence_counts:
  read: 15
  safety-critical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Amperity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workflow/runs/{workflow-id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workflow/runs/{workflow-id}/stop
operation_count: 19
overview: 'Amperity exposes 19 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 2 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amperity
provider_slug: amperity
slug: amperity-agentic-access
source_filename: amperity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/amperity-control-plane-2024-04-01-openapi.json, openapi/amperity-control-plane-unstable-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 15\n    acting: 4\n  by_consequence:\n    read: 15\n    write: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /audit-events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: get\n  operationId: list-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments\n  method: get\n  operationId: list-segment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/jobs\n  method: get\n  operationId: list-ingest-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/jobs/{job-id}\n  method: get\n  operationId: get-ingest-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs\n  method: get\n  operationId: list-workflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs\n  method: post\n  operationId: run-workflow\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflow/runs/{workflow-id}\n  method: get\n  operationId: get-workflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs/{workflow-id}/stop\n  method: post\n  operationId: stop-workflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /audit-events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign-drafts\n  method: get\n  operationId: list-campaign-draft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: get\n  operationId: list-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments\n  method: get\n  operationId: list-segment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/jobs\n  method: get\n  operationId: list-ingest-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/jobs/{job-id}\n  method: get\n\
  \  operationId: get-ingest-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs\n  method: get\n  operationId: list-workflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs\n  method: post\n  operationId: run-workflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflow/runs/{workflow-id}\n  method: get\n  operationId: get-workflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/runs/{workflow-id}/stop\n\
  \  method: post\n  operationId: stop-workflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/agentic-access/amperity-agentic-access.yml
summary_line: 19 operations · 4 acting · 2 human-in-the-loop
tags:
- Company
- Enterprise
- Customer Data Platform
- CDP
- Identity Resolution
- Customer 360
- Marketing
- Data
- Profiles
- Analytics
- MCP
- Agents
- Retail
- Identity
---
