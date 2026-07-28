---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Dispatches API
  slug: voltus-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Sites API
  slug: voltus-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Telemetry API
  slug: voltus-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Webhooks API
  slug: voltus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Voltus Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2022-04-15/dispatches
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2022-04-15/telemetry/controllable-load
operation_count: 10
overview: 'Voltus exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Voltus
provider_slug: voltus
slug: voltus-agentic-access
source_filename: voltus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/voltus-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 5\n    connected: 5\n  by_consequence:\n    safety-critical: 2\n    read: 5\n    write: 3\n  human_in_the_loop_required: 2\noperations:\n- path: /2022-04-15/dispatches\n  method: post\n  operationId: voltus#post-dispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2022-04-15/dispatches\n  method: get\n  operationId:\
  \ voltus#get-dispatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-04-15/dispatches/{id}\n  method: get\n  operationId: voltus#get-dispatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-04-15/sites\n  method: get\n  operationId: voltus#get-sites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-04-15/telemetry\n  method: post\n  operationId: voltus#post-telemetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2022-04-15/telemetry/controllable-load\n\
  \  method: post\n  operationId: voltus#post-controllable-load\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2022-04-15/telemetry/kw\n  method: get\n  operationId: voltus#get-telemetry-kw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-04-15/webhooks\n  method: get\n  operationId: voltus#get-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-04-15/webhooks\n  method: post\n  operationId: voltus#post-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2022-04-15/webhooks/{id}\n  method: delete\n  operationId: voltus#delete-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/agentic-access/voltus-agentic-access.yml
summary_line: 10 operations · 5 acting · 2 human-in-the-loop
tags:
- Energy
- United States
- Electricity
- Demand Response
- Virtual Power Plant
- DER
- Grid
- Energy Markets
- Flexibility
- Energy Storage
- OpenADR
- Telemetry
---
