---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: liberty-global-appstore-metadata-service-openapi.yml
  format: yaml
  label: AppStore Metadata Service API
  slug: appstore-metadata-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-metadata-service-openapi.yml
- filename: liberty-global-appstore-bundle-service-openapi.yml
  format: yaml
  label: AppStore Bundle Service API
  slug: appstore-bundle-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-bundle-service-openapi.yml
- filename: liberty-global-appstore-caching-service-openapi.yml
  format: yaml
  label: AppStore Caching Service API
  slug: appstore-caching-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-caching-service-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liberty Global Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Liberty Global exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Liberty Global
provider_slug: liberty-global
slug: liberty-global-agentic-access
source_filename: liberty-global-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/liberty-global-appstore-bundle-service-openapi.yml, openapi/liberty-global-appstore-caching-service-openapi.yml,\n  openapi/liberty-global-appstore-metadata-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /applications/{appId}/{appVersion}/{platformName}/{firmwareVersion}/{appBundleName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{appId}/{appVersion}/{platformName}/{firmwareVersion}/{appBundleName}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{applicationId}\n  method: get\n  operationId: getApplicationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintainers\n  method: get\n  operationId: getMaintainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintainers\n  method: post\n  operationId: createMaintainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maintainers/{maintainerCode}\n  method: get\n  operationId: getMaintainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintainers/{maintainerCode}\n  method: put\n  operationId: replaceMaintainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maintainers/{maintainerCode}\n  method: delete\n  operationId: deleteMaintainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maintainers/{maintainerCode}/apps\n  method: get\n  operationId: listMaintainerApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintainers/{maintainerCode}/apps\n  method: post\n  operationId: createMaintainerApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maintainers/{maintainerCode}/apps/{applicationId}\n  method: put\n  operationId: replaceMaintainerApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maintainers/{maintainerCode}/apps/{applicationId}\n  method: get\n  operationId: getMaintainerApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintainers/{maintainerCode}/apps/{applicationId}\n  method: delete\n  operationId: deleteMaintainerApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/agentic-access/liberty-global-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Telecommunications
- United Kingdom
- Broadband
- Fixed Broadband
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Europe
- Set-Top Box
- RDK
---
