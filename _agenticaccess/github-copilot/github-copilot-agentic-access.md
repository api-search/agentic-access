---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 14
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Copilot API
  slug: github-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot for Business API
  slug: github-copilot-for-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot User Management API
  slug: github-copilot-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Metrics API
  slug: github-copilot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Usage Metrics API
  slug: github-copilot-usage-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Content Exclusion API
  slug: github-copilot-content-exclusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
consequence_counts:
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Github Copilot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'GitHub Copilot exposes 19 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitHub Copilot
provider_slug: github-copilot
slug: github-copilot-agentic-access
source_filename: github-copilot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/github-copilot-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 14\n    acting: 5\n  by_consequence:\n    read: 14\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /orgs/{org}/copilot/billing\n  method: get\n  operationId: getCopilotBillingForOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/billing/seats\n  method: get\n  operationId: listCopilotSeats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /orgs/{org}/copilot/billing/selected_teams\n  method: post\n  operationId: addTeamsToCopilotSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/copilot/billing/selected_teams\n  method: delete\n  operationId: removeTeamsFromCopilotSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/copilot/billing/selected_users\n  method: post\n  operationId: addUsersToCopilotSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/copilot/billing/selected_users\n  method: delete\n  operationId: removeUsersFromCopilotSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/members/{username}/copilot\n  method: get\n  operationId: getCopilotSeatForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/metrics\n  method: get\n  operationId: getCopilotMetricsForOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/team/{team_slug}/copilot/metrics\n  method: get\n  operationId: getCopilotMetricsForTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprises/{enterprise}/copilot/metrics/reports/enterprise-1-day\n  method: get\n  operationId: getEnterpriseCopilotUsageDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprises/{enterprise}/copilot/metrics/reports/enterprise-28-day/latest\n  method: get\n  operationId: getEnterpriseCopilotUsage28Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprises/{enterprise}/copilot/metrics/reports/users-1-day\n  method: get\n\
  \  operationId: getEnterpriseUsersCopilotUsageDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprises/{enterprise}/copilot/metrics/reports/users-28-day/latest\n  method: get\n  operationId: getEnterpriseUsersCopilotUsage28Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/metrics/reports/organization-1-day\n  method: get\n  operationId: getOrganizationCopilotUsageDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/metrics/reports/organization-28-day/latest\n  method: get\n  operationId: getOrganizationCopilotUsage28Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/metrics/reports/users-1-day\n  method: get\n  operationId: getOrganizationUsersCopilotUsageDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/metrics/reports/users-28-day/latest\n  method: get\n  operationId: getOrganizationUsersCopilotUsage28Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/content_exclusion\n  method: get\n  operationId: getCopilotContentExclusionRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/copilot/content_exclusion\n  method: put\n  operationId: setCopilotContentExclusionRules\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/agentic-access/github-copilot-agentic-access.yml
summary_line: 19 operations · 5 acting
tags:
- Agents
- AI
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine Learning
- MCP
- Metrics
- Model Context Protocol
- Productivity
---
