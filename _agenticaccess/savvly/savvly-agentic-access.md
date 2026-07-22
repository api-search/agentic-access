---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: savvly-openapi-original.json
  format: json
  label: Savvly Public API
  slug: savvly-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvly/refs/heads/main/openapi/savvly-openapi-original.json
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Savvly Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Savvly exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Savvly
provider_slug: savvly
slug: savvly-agentic-access
source_filename: savvly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/savvly-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/product\n  method: get\n  operationId: getSavvlyProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product/summary\n  method: get\n  operationId: getSavvlyProductSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product/schema\n  method: get\n  operationId:\
  \ getSavvlyProductSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comparisons\n  method: get\n  operationId: getSavvlyComparisons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comparisons/{type}\n  method: get\n  operationId: compareSavvlyVsProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projections/lumpsum\n  method: get\n  operationId: projectLumpsumReturns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projections/monthly\n  method: get\n  operationId: projectMonthlyReturns\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projections/retirement\n  method: get\n  operationId: projectRetirementWithSavvly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projections/growth-chart\n  method: get\n  operationId: projectGrowthChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eligibility\n  method: get\n  operationId: getSavvlyEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/faq\n  method: get\n  operationId: getSavvlyFAQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels\n\
  \  method: get\n  operationId: getSavvlyChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savvly/refs/heads/main/agentic-access/savvly-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Fintech
- Retirement
- Longevity
- Investing
- Financial Services
- Projections
- Annuity Alternative
---
