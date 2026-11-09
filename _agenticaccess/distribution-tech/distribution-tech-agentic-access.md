---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: distribution-tech-audience-api-openapi.yml
  format: yaml
  label: distribution-tech Audience API
  slug: distribution-tech-audience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-audience-api-openapi.yml
- filename: distribution-tech-brain-api-openapi.yml
  format: yaml
  label: distribution-tech Brain API
  slug: distribution-tech-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-brain-api-openapi.yml
- filename: distribution-tech-campaigns-api-openapi.yml
  format: yaml
  label: distribution-tech Campaigns API
  slug: distribution-tech-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-campaigns-api-openapi.yml
- filename: distribution-tech-creators-api-openapi.yml
  format: yaml
  label: distribution-tech Creators API
  slug: distribution-tech-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-creators-api-openapi.yml
- filename: distribution-tech-evidence-api-openapi.yml
  format: yaml
  label: distribution-tech Evidence API
  slug: distribution-tech-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-evidence-api-openapi.yml
- filename: distribution-tech-feedback-api-openapi.yml
  format: yaml
  label: distribution-tech Feedback API
  slug: distribution-tech-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-feedback-api-openapi.yml
- filename: distribution-tech-inventory-api-openapi.yml
  format: yaml
  label: distribution-tech Inventory API
  slug: distribution-tech-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-inventory-api-openapi.yml
- filename: distribution-tech-plans-api-openapi.yml
  format: yaml
  label: distribution-tech Plans API
  slug: distribution-tech-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-plans-api-openapi.yml
- filename: distribution-tech-results-api-openapi.yml
  format: yaml
  label: distribution-tech Results API
  slug: distribution-tech-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-results-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Distribution Tech Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /feedback
operation_count: 23
overview: 'distribution-tech exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: distribution-tech
provider_slug: distribution-tech
slug: distribution-tech-agentic-access
source_filename: distribution-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/distribution-tech-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /inventory\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inventory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audience\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}/quote\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{id}/lines\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}/lines/{line_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}/lines/{line_id}/swap\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}/dates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}/approve\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - plans:approve\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/creator-guidelines\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/archive\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - campaigns:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evidence\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - evidence:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - results:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creators:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creators/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creators:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /creators/{id}/price-request\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creators:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brain\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - brain:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/distribution-tech/agentic-access/distribution-tech-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Company
- Distribution
- Marketing
- Software-as-a-Service
- Creator Economy
---
