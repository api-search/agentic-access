---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: liferay-openapi.yml
  format: yaml
  label: Liferay Roles API
  slug: liferay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/openapi/liferay-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liferay Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Liferay exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Liferay
provider_slug: liferay
slug: liferay-agentic-access
source_filename: liferay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/liferay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 2\n    acting: 6\n  by_consequence:\n    read: 2\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /roles\n  method: get\n  operationId: getRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/{roleId}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/{roleId}/association/user-account/{userId}\n  method:\
  \ post\n  operationId: associateRoleToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}/association/user-account/{userId}\n  method: delete\n  operationId: dissociateRoleFromUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}/association/user-account/{userId}/site/{siteId}\n  method: post\n  operationId: associateSiteRoleToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}/association/user-account/{userId}/site/{siteId}\n  method: delete\n  operationId: dissociateSiteRoleFromUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}/association/user-account/{userId}/organization/{orgId}\n  method: post\n  operationId: associateOrgRoleToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}/association/user-account/{userId}/organization/{orgId}\n\
  \  method: delete\n  operationId: dissociateOrgRoleFromUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/agentic-access/liferay-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Open Source
- Digital Experience
- DXP
- Roles
- Users
- Permissions
- Headless
---
