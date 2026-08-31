---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 3
api_specs:
- filename: mparticle-data-plan-api-openapi.yml
  format: yaml
  label: mParticle Data Plan API
  slug: mparticle-data-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-api-openapi.yml
- filename: mparticle-data-plan-version-api-openapi.yml
  format: yaml
  label: mParticle Data Plan Version API
  slug: mparticle-data-plan-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-version-api-openapi.yml
- filename: mparticle-events-api-openapi.yml
  format: yaml
  label: mParticle Events API
  slug: mparticle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-events-api-openapi.yml
- filename: mparticle-identify-api-openapi.yml
  format: yaml
  label: mParticle Identify API
  slug: mparticle-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-identify-api-openapi.yml
- filename: mparticle-login-api-openapi.yml
  format: yaml
  label: mParticle Login API
  slug: mparticle-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-login-api-openapi.yml
- filename: mparticle-logout-api-openapi.yml
  format: yaml
  label: mParticle Logout API
  slug: mparticle-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-logout-api-openapi.yml
- filename: mparticle-modify-api-openapi.yml
  format: yaml
  label: mParticle Modify API
  slug: mparticle-modify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-modify-api-openapi.yml
consequence_counts:
  physical: 2
  read: 3
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mparticle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulkevents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events
operation_count: 16
overview: 'mParticle exposes 16 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 11 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: mParticle
provider_slug: mparticle
slug: mparticle-agentic-access
source_filename: mparticle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/mparticle-dataplanning-openapi-original.yml, openapi/mparticle-events-openapi-original.yml,\n  openapi/mparticle-identity-swagger-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 3\n    acting: 13\n  by_consequence:\n    read: 3\n    write: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: create-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{plan_id}\n  method: get\n  operationId: get-plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{plan_id}\n  method: delete\n  operationId: delete-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{plan_id}\n  method: patch\n  operationId: update-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{plan_id}/versions/{plan_version}\n  method: get\n  operationId: get-plan-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{plan_id}/versions/{plan_version}\n  method: patch\n  operationId: update-plan-version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{plan_id}/versions/{plan_version}\n  method: delete\n  operationId: delete-plan-version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{plan_id}/versions\n  method: post\n  operationId: create-plan-version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate\n  method: post\n  operationId: validate-plan-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: uploadEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulkevents\n  method: post\n  operationId: bulkUploadEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identify\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{mpid}/modify\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/agentic-access/mparticle-agentic-access.yml
summary_line: 16 operations · 13 acting
tags:
- Customer Data Platform
- CDP
- Analytics
- Identity Resolution
- Audience
- Data Pipeline
- Marketing Data
- Event Streaming
- Data Governance
---
