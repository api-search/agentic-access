---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Team Members
  slug: team-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave / Absences
  slug: leave-absences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave Allowances
  slug: leave-allowances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Company
  slug: company
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Charliehr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'CharlieHR exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CharlieHR
provider_slug: charliehr
slug: charliehr-agentic-access
source_filename: charliehr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/charliehr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /team_members\n  method: get\n  operationId: listTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team_members/{id}\n  method: get\n  operationId: getTeamMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team_members/{id}/notes\n  method: get\n  operationId:\
  \ listTeamMemberNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team_members/{id}/leave_requests\n  method: get\n  operationId: listTeamMemberLeaveRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team_members/{id}/leave_allowance\n  method: get\n  operationId: getTeamMemberLeaveAllowance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave_requests\n  method: get\n  operationId: listLeaveRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave_requests/{id}\n  method: get\n  operationId: getLeaveRequest\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave_allowances\n  method: get\n  operationId: listLeaveAllowances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offices\n  method: get\n  operationId: listOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offices/{id}\n  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId:\
  \ listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{id}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/agentic-access/charliehr-agentic-access.yml
summary_line: 13 operations
tags:
- HR
- HRIS
- People
- Leave
- Time Off
---
