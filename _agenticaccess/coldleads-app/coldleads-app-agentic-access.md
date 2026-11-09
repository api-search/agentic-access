---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: coldleads-app-activity-api-openapi.yml
  format: yaml
  label: Cold Leads Activity API
  slug: coldleads-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-activity-api-openapi.yml
- filename: coldleads-app-credits-api-openapi.yml
  format: yaml
  label: Cold Leads Credits API
  slug: coldleads-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-credits-api-openapi.yml
- filename: coldleads-app-find-api-openapi.yml
  format: yaml
  label: Cold Leads Find API
  slug: coldleads-app-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-find-api-openapi.yml
- filename: coldleads-app-follow-ups-api-openapi.yml
  format: yaml
  label: Cold Leads Follow Ups API
  slug: coldleads-app-follow-ups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-follow-ups-api-openapi.yml
- filename: coldleads-app-leads-api-openapi.yml
  format: yaml
  label: Cold Leads Leads API
  slug: coldleads-app-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-leads-api-openapi.yml
- filename: coldleads-app-next-actions-api-openapi.yml
  format: yaml
  label: Cold Leads Next Actions API
  slug: coldleads-app-next-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-next-actions-api-openapi.yml
- filename: coldleads-app-social-api-openapi.yml
  format: yaml
  label: Cold Leads Social API
  slug: coldleads-app-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-social-api-openapi.yml
- filename: coldleads-app-verify-api-openapi.yml
  format: yaml
  label: Cold Leads Verify API
  slug: coldleads-app-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-verify-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coldleads App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /follow-ups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /social/messages/reply
operation_count: 15
overview: 'Cold Leads exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cold Leads
provider_slug: coldleads-app
slug: coldleads-app-agentic-access
source_filename: coldleads-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coldleads-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 5\n    connected: 10\n  by_consequence:\n    write: 3\n    read: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /verify\n  method: post\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/bulk\n  method: post\n  operationId: verifyBulk\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/jobs/{id}\n  method: get\n  operationId: getVerifyJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find\n  method: post\n  operationId: findEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: get\n  operationId: searchLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/context\n  method: get\n  operationId: getLeadContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /next-actions\n  method: get\n  operationId: getSalesNextActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follow-ups\n  method: post\n  operationId: scheduleFollowUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activity\n  method: get\n  operationId: getAgentActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social\n  method: get\n  operationId: getSocialOverview\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/autoposts\n  method: get\n  operationId: listAutoposts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/posts\n  method: post\n  operationId: scheduleSocialPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /social/messages\n  method: get\n  operationId: getSocialInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/messages/reply\n  method: post\n  operationId: replySocialMessage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/coldleads-app/agentic-access/coldleads-app-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- CRM
- Software-as-a-Service
- Small Business
- Lead Management
- Cold Leads
---
