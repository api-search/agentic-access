---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 3
api_specs:
- filename: intelligems-external-api-openapi.yml
  format: yaml
  label: Intelligems External API
  slug: intelligems-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-external-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intelligems Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v25-10-beta/analytics/sitewide/order-distribution
operation_count: 15
overview: 'Intelligems exposes 15 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Intelligems
provider_slug: intelligems
slug: intelligems-agentic-access
source_filename: intelligems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/intelligems-external-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 3\n    acting: 12\n  by_consequence:\n    read: 3\n    write: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v25-10-beta/experiences-list\n  method: get\n  operationId: listExperiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v25-10-beta/experiences/{experienceId}\n  method: get\n  operationId: getExperience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v25-10-beta/experiences/{experienceId}\n  method: put\n  operationId: updateExperience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/experiences\n  method: post\n  operationId: createExperience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/experiences/{experienceId}/actions/{action}\n  method: post\n  operationId: performExperienceAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/resource/{experienceId}\n  method: get\n  operationId: getExperienceAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v25-10-beta/analytics/resource/{experienceId}\n  method: post\n  operationId: queryExperienceAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/experience/{experienceId}/timeseries\n  method: post\n  operationId: getExperienceTimeseries\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/experience/{experienceId}/export\n  method: post\n  operationId: exportExperienceAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/sitewide/snapshot\n  method: post\n  operationId: getSitewideSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v25-10-beta/analytics/sitewide/timeseries\n  method: post\n  operationId: getSitewideTimeseries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/sitewide/order-distribution\n  method: post\n  operationId: getSitewideOrderDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/sitewide/conversion-funnel\n  method: post\n  operationId: getSitewideConversionFunnel\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/event/snapshot\n  method: post\n  operationId: getHolidayBenchmarkSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v25-10-beta/analytics/event/timeseries\n  method: post\n  operationId: getHolidayBenchmarkTimeseries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/agentic-access/intelligems-agentic-access.yml
summary_line: 15 operations · 12 acting
tags:
- Company
- A/B Testing
- Ecommerce
- Pricing
- Personalization
- Conversion Rate Optimization
- Shopify
- Analytics
- Experimentation
---
