---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: avasis-ai-admin-api-openapi.yml
  format: yaml
  label: Avasis Admin API
  slug: avasis-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-admin-api-openapi.yml
- filename: avasis-ai-authors-api-openapi.yml
  format: yaml
  label: Avasis Authors API
  slug: avasis-ai-authors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-authors-api-openapi.yml
- filename: avasis-ai-avasis-exchange-api-api-openapi.yml
  format: yaml
  label: Avasis Avasis Exchange API
  slug: avasis-ai-avasis-exchange-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-avasis-exchange-api-api-openapi.yml
- filename: avasis-ai-connect-api-openapi.yml
  format: yaml
  label: Avasis Connect API
  slug: avasis-ai-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-connect-api-openapi.yml
- filename: avasis-ai-fixes-api-openapi.yml
  format: yaml
  label: Avasis Fixes API
  slug: avasis-ai-fixes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-fixes-api-openapi.yml
- filename: avasis-ai-leaderboard-api-openapi.yml
  format: yaml
  label: Avasis Leaderboard API
  slug: avasis-ai-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-leaderboard-api-openapi.yml
- filename: avasis-ai-problems-api-openapi.yml
  format: yaml
  label: Avasis Problems API
  slug: avasis-ai-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-problems-api-openapi.yml
- filename: avasis-ai-report-api-openapi.yml
  format: yaml
  label: Avasis Report API
  slug: avasis-ai-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-report-api-openapi.yml
- filename: avasis-ai-stats-api-openapi.yml
  format: yaml
  label: Avasis Stats API
  slug: avasis-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avasis-ai/openapi/avasis-ai-stats-api-openapi.yml
consequence_counts:
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Avasis Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Avasis exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Avasis
provider_slug: avasis-ai
slug: avasis-ai-agentic-access
source_filename: avasis-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/avasis-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  operationId: v1_stats_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/problems\n  method: get\n  operationId:\
  \ v1_problems_v1_problems_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/problems/sitemap\n  method: get\n  operationId: v1_sitemap_v1_problems_sitemap_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect\n  method: get\n  operationId: v1_connect_v1_connect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leaderboard\n  method: get\n  operationId: v1_leaderboard_v1_leaderboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/authors/{slug}\n  method: get\n  operationId: v1_author_profile_v1_authors__slug__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/report/{sid}\n  method: post\n  operationId: v1_report_public_v1_report__sid__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fixes\n  method: post\n  operationId: v1_fix_publish_v1_fixes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/queue\n  method: get\n  operationId: v1_admin_queue_v1_admin_queue_get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/problems/{pid}/status\n  method: post\n  operationId: v1_admin_problem_status_v1_admin_problems__pid__status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/moderation\n  method: get\n  operationId: v1_admin_moderation_v1_admin_moderation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/moderation/stats\n  method: get\n  operationId: v1_admin_moderation_stats_v1_admin_moderation_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/avasis-ai/agentic-access/avasis-ai-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- Artificial Intelligence
- Edge Computing
- Privacy
- Research Lab
- Device AI
---
