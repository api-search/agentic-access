---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 12
api_specs:
- filename: gbg-as-api-openapi.yml
  format: yaml
  label: GBG As API
  slug: gbg-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-as-api-openapi.yml
- filename: gbg-authentication-api-openapi.yml
  format: yaml
  label: GBG Authentication API
  slug: gbg-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-authentication-api-openapi.yml
- filename: gbg-customer-apis-api-openapi.yml
  format: yaml
  label: GBG Customer APIs API
  slug: gbg-customer-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-customer-apis-api-openapi.yml
- filename: gbg-device-api-openapi.yml
  format: yaml
  label: GBG Device API
  slug: gbg-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-device-api-openapi.yml
- filename: gbg-end-user-apis-api-openapi.yml
  format: yaml
  label: GBG End User APIs API
  slug: gbg-end-user-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-end-user-apis-api-openapi.yml
- filename: gbg-health-api-openapi.yml
  format: yaml
  label: GBG Health API
  slug: gbg-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-health-api-openapi.yml
- filename: gbg-interaction-api-openapi.yml
  format: yaml
  label: GBG Interaction API
  slug: gbg-interaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-api-openapi.yml
- filename: gbg-interaction-service-api-openapi.yml
  format: yaml
  label: GBG Interaction Service API
  slug: gbg-interaction-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-service-api-openapi.yml
- filename: gbg-journey-api-openapi.yml
  format: yaml
  label: GBG Journey API
  slug: gbg-journey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-api-openapi.yml
- filename: gbg-journey-execution-api-openapi.yml
  format: yaml
  label: GBG Journey execution API
  slug: gbg-journey-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-execution-api-openapi.yml
- filename: gbg-sandbox-api-openapi.yml
  format: yaml
  label: GBG Sandbox API
  slug: gbg-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-sandbox-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Gbg Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /journey/terminate
operation_count: 29
overview: 'GBG exposes 29 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GBG
provider_slug: gbg
slug: gbg-agentic-access
source_filename: gbg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/gbg-go-v1-openapi.yml, openapi/gbg-go-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 17\n    connected: 12\n  by_consequence:\n    write: 16\n    read: 12\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /as/token.oauth2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/start\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/task/list\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/task/list/schema\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/task/schema\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/task/update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/state/fetch\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/start\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/interaction/fetch\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/interaction/submit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/interaction/asset/upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/instance/{instanceId}/handoff-token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/loqate/search\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /journey/loqate/retrieve\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/state/fetch\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/schema/fetch\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/task/schema\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/terminate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n \
  \     exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /journey/state/delete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/device/start\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/device/connect\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/device/refresh\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journey/device/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/journeys/{journeyId}/scenarios\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/journeys/{journeyId}/scenarios\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/journeys/{journeyId}/scenarios/{name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/journeys/{journeyId}/scenarios/{name}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/journeys/{journeyId}/scenarios/{name}\n  method: delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/token.oauth2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/gbg/agentic-access/gbg-agentic-access.yml
summary_line: 29 operations · 17 acting · 1 human-in-the-loop
tags:
- Company
- Identity Verification
- Fraud Prevention
- KYC
- Location Intelligence
- Compliance
- Digital Identity
---
