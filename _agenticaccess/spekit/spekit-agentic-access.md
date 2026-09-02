---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: spekit-searches-api-openapi.yml
  format: yaml
  label: Spekit Searches API
  slug: spekit-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-searches-api-openapi.yml
- filename: spekit-spek-reactions-api-openapi.yml
  format: yaml
  label: Spekit Spek Reactions API
  slug: spekit-spek-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-spek-reactions-api-openapi.yml
- filename: spekit-spek-views-api-openapi.yml
  format: yaml
  label: Spekit Spek Views API
  slug: spekit-spek-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-spek-views-api-openapi.yml
- filename: spekit-user-activities-api-openapi.yml
  format: yaml
  label: Spekit User Activities API
  slug: spekit-user-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-user-activities-api-openapi.yml
- filename: spekit-users-api-openapi.yml
  format: yaml
  label: Spekit Users API
  slug: spekit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-users-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spekit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Spekit exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spekit
provider_slug: spekit
slug: spekit-agentic-access
source_filename: spekit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/spekit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/analytics/searches/\n  method: get\n  operationId: v1_analytics_searches_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/speks/reactions/\n  method: get\n  operationId: v1_analytics_speks_reactions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/speks/views/\n\
  \  method: get\n  operationId: v1_analytics_speks_views_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/user-activities/\n  method: get\n  operationId: v1_analytics_user_activities_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/\n  method: get\n  operationId: v1_users_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/agentic-access/spekit-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Software-as-a-Service
- Sales Enablement
- Revenue Enablement
- Digital Adoption
- Knowledge-Management
- MCP
- Artificial Intelligence
- Analytics
- Sales
- Content Management
- Agents
- Authentication
---
