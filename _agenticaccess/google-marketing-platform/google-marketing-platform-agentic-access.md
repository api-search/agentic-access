---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Marketing Platform Admin API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Marketing Platform Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Google Marketing Platform Admin exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
slug: google-marketing-platform-agentic-access
source_filename: google-marketing-platform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 2\n    acting: 3\n  by_consequence:\n    read: 2\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1alpha/organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n- path: /v1alpha/{parent}/analyticsAccountLinks\n  method: get\n  operationId: listAnalyticsAccountLinks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n- path: /v1alpha/{parent}/analyticsAccountLinks\n  method: post\n  operationId: createAnalyticsAccountLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n- path: /v1alpha/{name}\n  method: delete\n  operationId: deleteAnalyticsAccountLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n- path: /v1alpha/{analyticsAccountLink}:setPropertyServiceLevel\n  method: post\n  operationId: setPropertyServiceLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/agentic-access/google-marketing-platform-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
---
