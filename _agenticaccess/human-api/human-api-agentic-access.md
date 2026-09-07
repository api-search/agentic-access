---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: human-api-admin-api-openapi.yml
  format: yaml
  label: Human API Admin API
  slug: human-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-admin-api-openapi.yml
- filename: human-api-connect-api-openapi.yml
  format: yaml
  label: Human API Connect API
  slug: human-api-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-connect-api-openapi.yml
- filename: human-api-orders-api-openapi.yml
  format: yaml
  label: Human API Orders API
  slug: human-api-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-orders-api-openapi.yml
- filename: human-api-reports-api-openapi.yml
  format: yaml
  label: Human API Reports API
  slug: human-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-reports-api-openapi.yml
- filename: human-api-resources-api-openapi.yml
  format: yaml
  label: Human API Resources API
  slug: human-api-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-resources-api-openapi.yml
- filename: human-api-subscriptions-api-openapi.yml
  format: yaml
  label: Human API Subscriptions API
  slug: human-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-subscriptions-api-openapi.yml
- filename: human-api-users-api-openapi.yml
  format: yaml
  label: Human API Users API
  slug: human-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-users-api-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Human Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Human API exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Human API
provider_slug: human-api
slug: human-api-agentic-access
source_filename: human-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/humanapi-admin-openapi.yml, openapi/humanapi-auth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/order-types\n  method: get\n  operationId: getOrderTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users\n  method: get\n  operationId: getUsersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/actions\n  method: post\n  operationId: performActionForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{humanId}\n  method: get\n  operationId: getUserDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/providers\n  method: get\n  operationId: userProviders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscriptions\n  method: get\n  operationId: getUsersSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscriptions/{subscriptionId}\n  method: get\n  operationId: getSubscriptionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscriptions/{subscriptionId}\n\
  \  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/reports\n  method: get\n  operationId: getUserReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/reports/{reportId}\n  method: get\n  operationId: getReportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resources/consumer-link\n  method: post\n  operationId: getTasksLiistLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/agentic-access/human-api-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Healthcare
- United States
- Health Data
- EHR
- Interoperability
- Remote Monitoring
- Wearables
- Life Insurance
- Clinical Data
- Health API
---
