---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: clevertap-campaigns-api-openapi.yml
  format: yaml
  label: CleverTap Campaigns API
  slug: clevertap-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-campaigns-api-openapi.yml
- filename: clevertap-events-api-openapi.yml
  format: yaml
  label: CleverTap Events API
  slug: clevertap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-events-api-openapi.yml
- filename: clevertap-profiles-api-openapi.yml
  format: yaml
  label: CleverTap Profiles API
  slug: clevertap-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-profiles-api-openapi.yml
- filename: clevertap-reports-api-openapi.yml
  format: yaml
  label: CleverTap Reports API
  slug: clevertap-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-reports-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Clevertap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /1/targets/stop.json
operation_count: 11
overview: 'CleverTap exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CleverTap
provider_slug: clevertap
slug: clevertap-agentic-access
source_filename: clevertap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/clevertap-campaigns-api-openapi.yml, openapi/clevertap-events-api-openapi.yml,\n  openapi/clevertap-profiles-api-openapi.yml, openapi/clevertap-reports-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 4\n    safety-critical: 1\n    read: 6\n  human_in_the_loop_required: 1\noperations:\n- path: /1/targets/create.json\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /1/targets/stop.json\n  method: post\n  operationId: stopCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /1/targets/result.json\n  method: get\n  operationId: getCampaignResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/upload\n  method: post\n  operationId: upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /1/events.json\n  method: post\n  operationId: queryEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/upload\n  method: post\n  operationId: upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/profile.json\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/profiles.json\n  method: post\n  operationId: queryProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/disassociate\n\
  \  method: post\n  operationId: disassociateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/counts/event.json\n  method: post\n  operationId: getEventCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/counts/profile.json\n  method: post\n  operationId: getProfileCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/agentic-access/clevertap-agentic-access.yml
summary_line: 11 operations · 5 acting · 1 human-in-the-loop
tags:
- Audiences
- Customer Engagement
- Customer Retention
- Marketing Automation
- Mobile Engagement
- Push Notifications
- User Behavior
---
