---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: urbanfox-customer-api-openapi.yml
  format: yaml
  label: UrbanFox Customer API
  slug: urbanfox-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/openapi/urbanfox-customer-api-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Urbanfox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'UrbanFox exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UrbanFox
provider_slug: urbanfox
slug: urbanfox-agentic-access
source_filename: urbanfox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/urbanfox-customer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/{tenant_slug}/tenants\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:tenant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/tenants/auth-secret\n  method: get\n  operationId: getTenantAuthSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - read:tenant_auth_secret\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/tenants/rotate-auth-secret\n  method: post\n  operationId: postRotateTenantAuthSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:tenant_auth_secret\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{tenant_slug}/cases/{case_id}\n  method: get\n  operationId: getCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:case\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/cases/{case_id}\n  method: put\n  operationId: putCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:case\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{tenant_slug}/cases\n  method: get\n  operationId: getAllCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:cases\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/enduseraccounts/{website_account_id}\n  method: get\n  operationId: getEndUserAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:enduseraccount\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/enduseraccounts/{website_account_id}\n  method: put\n  operationId: putEndUserAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:enduseraccount\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{tenant_slug}/enduseraccounts/{website_account_id}\n  method: delete\n  operationId: deleteEndUserAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:enduseraccount\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{tenant_slug}/enduseraccounts\n  method: get\n  operationId: getEndUserAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:enduseraccounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/enduseraccounts\n  method: post\n  operationId: postEndUserAccount\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - create:enduseraccount\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{tenant_slug}/metrics\n  method: get\n  operationId: getMetricsAggregate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:metrics\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{tenant_slug}/snippet\n  method: get\n  operationId: getSnippet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:snippet\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth/token\n  method: post\n  operationId: postOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/agentic-access/urbanfox-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Fraud Detection
- Payment Fraud
- Account Takeover
- Bot Detection
- Risk Management
- Security
- Artificial Intelligence
- eCommerce
---
