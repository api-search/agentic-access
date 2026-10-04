---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 8
api_specs:
- filename: cursor-audit-logs-api-openapi.yml
  format: yaml
  label: Cursor Audit Logs API
  slug: cursor-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-audit-logs-api-openapi.yml
- filename: cursor-groups-api-openapi.yml
  format: yaml
  label: Cursor Groups API
  slug: cursor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-groups-api-openapi.yml
- filename: cursor-members-api-openapi.yml
  format: yaml
  label: Cursor Members API
  slug: cursor-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-members-api-openapi.yml
- filename: cursor-repo-blocklists-api-openapi.yml
  format: yaml
  label: Cursor Repo Blocklists API
  slug: cursor-repo-blocklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-repo-blocklists-api-openapi.yml
- filename: cursor-spend-api-openapi.yml
  format: yaml
  label: Cursor Spend API
  slug: cursor-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-spend-api-openapi.yml
- filename: cursor-usage-api-openapi.yml
  format: yaml
  label: Cursor Usage API
  slug: cursor-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-usage-api-openapi.yml
consequence_counts:
  read: 8
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cursor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Cursor exposes 17 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cursor
provider_slug: cursor
slug: cursor-agentic-access
source_filename: cursor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cursor-audit-logs-api-openapi.yml, openapi/cursor-groups-api-openapi.yml, openapi/cursor-members-api-openapi.yml,\n  openapi/cursor-repo-blocklists-api-openapi.yml, openapi/cursor-spend-api-openapi.yml, openapi/cursor-usage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 8\n    acting: 9\n  by_consequence:\n    read: 8\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /teams/audit-logs\n  method: get\n  operationId: getAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/groups\n  method: get\n\
  \  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/groups/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/groups/{groupId}\n  method: patch\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/groups/{groupId}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/groups/{groupId}/members\n  method: post\n  operationId: addGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/groups/{groupId}/members\n  method: delete\n  operationId: removeGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/members\n  method: get\n  operationId: getTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/remove-member\n  method: post\n  operationId: removeTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/repo-blocklists/repos\n  method: get\n  operationId: getRepoBlocklists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /settings/repo-blocklists/repos/upsert\n  method: post\n  operationId: upsertRepoBlocklists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/repo-blocklists/repos/{repoId}\n  method: delete\n  operationId: deleteRepoBlocklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/user-spend-limit\n  method: post\n  operationId: setUserSpendLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/spend\n  method: post\n  operationId: getSpend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/daily-usage-data\n  method: post\n  operationId: getDailyUsageData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/filtered-usage-events\n  method: post\n  operationId: getFilteredUsageEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/agentic-access/cursor-agentic-access.yml
summary_line: 17 operations · 9 acting
tags:
- Artificial Intelligence
- Developer Tools
- Code Editor
- Agents
- IDE
- Cloud Agents
---
