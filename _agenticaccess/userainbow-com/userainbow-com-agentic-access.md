---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: userainbow-com-agency-api-openapi.yml
  format: yaml
  label: Rainbow Agency API
  slug: userainbow-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-agency-api-openapi.yml
- filename: userainbow-com-appetite-api-openapi.yml
  format: yaml
  label: Rainbow Appetite API
  slug: userainbow-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-appetite-api-openapi.yml
- filename: userainbow-com-indication-api-openapi.yml
  format: yaml
  label: Rainbow Indication API
  slug: userainbow-com-indication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-indication-api-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Userainbow Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Rainbow exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rainbow
provider_slug: userainbow-com
slug: userainbow-com-agentic-access
source_filename: userainbow-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/userainbow-com-rainbow-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /appetite\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indication\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /indication/id/{IndicationID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-agency\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sub-agency/id/{SubAgencyID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-agency/id/{SubAgencyID}/agent\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sub-agency/id/{SubAgencyID}/agent/id/{AgentID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-agency/id/{SubAgencyID}/agents\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-agency/npn/{NPN}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/userainbow-com/agentic-access/userainbow-com-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Insurance
- Restaurant
- Commercial Real Estate
- Beauty and Wellness
- Agents
- MGA
---
