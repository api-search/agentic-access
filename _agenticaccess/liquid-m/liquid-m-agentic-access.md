---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: liquid-m-ads-api-openapi.yml
  format: yaml
  label: Liquid M Ads API
  slug: liquid-m-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-ads-api-openapi.yml
- filename: liquid-m-authentication-api-openapi.yml
  format: yaml
  label: Liquid M Authentication API
  slug: liquid-m-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-authentication-api-openapi.yml
- filename: liquid-m-budgets-api-openapi.yml
  format: yaml
  label: Liquid M Budgets API
  slug: liquid-m-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-budgets-api-openapi.yml
- filename: liquid-m-campaigns-api-openapi.yml
  format: yaml
  label: Liquid M Campaigns API
  slug: liquid-m-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-campaigns-api-openapi.yml
- filename: liquid-m-reporting-api-openapi.yml
  format: yaml
  label: Liquid M Reporting API
  slug: liquid-m-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-reporting-api-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liquid M Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Liquid M exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Liquid M
provider_slug: liquid-m
slug: liquid-m-agentic-access
source_filename: liquid-m-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/liquid-m-ads-api-openapi.yml, openapi/liquid-m-authentication-api-openapi.yml,\n  openapi/liquid-m-budgets-api-openapi.yml, openapi/liquid-m-campaigns-api-openapi.yml, openapi/liquid-m-reporting-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /ads\n  method: get\n  operationId: listAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ads\n  method: post\n  operationId: createAd\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth\n  method: get\n  operationId: createAuthToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /budgets\n  method: post\n  operationId: createBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visual_reports.json\n  method: get\n  operationId: getVisualReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/agentic-access/liquid-m-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Company
- Advertising
- AdTech
- Demand-Side Platform
- Programmatic Advertising
- Mobile Advertising
- Reporting
- Analytics
- Campaign Management
- OpenRTB
---
