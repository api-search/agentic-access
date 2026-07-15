---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Authentication API
  slug: terra-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra User Management API
  slug: terra-api-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Activity API
  slug: terra-api-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Body API
  slug: terra-api-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Daily API
  slug: terra-api-daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Sleep API
  slug: terra-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Nutrition API
  slug: terra-api-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Menstruation API
  slug: terra-api-menstruation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Athlete API
  slug: terra-api-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Integrations API
  slug: terra-api-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
consequence_counts:
  read: 11
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Terra Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Terra exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Terra
provider_slug: terra-api
slug: terra-api-agentic-access
source_filename: terra-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/terra-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 5\n    connected: 11\n  by_consequence:\n    write: 5\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/authenticateUser\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/generateWidgetSession\n  method: post\n  operationId: generateWidgetSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/generateAuthToken\n  method: post\n  operationId: generateAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/deauthenticateUser\n  method: delete\n  operationId: deauthenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userInfo\n\
  \  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulkUserInfo\n  method: post\n  operationId: bulkUserInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activity\n  method: get\n  operationId: getActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /body\n  method: get\n  operationId:\
  \ getBody\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /daily\n  method: get\n  operationId: getDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sleep\n  method: get\n  operationId: getSleep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nutrition\n  method: get\n  operationId: getNutrition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menstruation\n  method: get\n  operationId: getMenstruation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /athlete\n\
  \  method: get\n  operationId: getAthlete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/detailed\n  method: get\n  operationId: listDetailedIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/agentic-access/terra-api-agentic-access.yml
summary_line: 16 operations · 5 acting
tags:
- Wearables
- Health Data
- Fitness
- Aggregator
- Webhooks
- Digital Health
---
