---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 12
api_specs:
- filename: bytebase-auth-api-openapi.yml
  format: yaml
  label: Bytebase Auth API
  slug: bytebase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-auth-api-openapi.yml
- filename: bytebase-databases-api-openapi.yml
  format: yaml
  label: Bytebase Databases API
  slug: bytebase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-databases-api-openapi.yml
- filename: bytebase-groups-api-openapi.yml
  format: yaml
  label: Bytebase Groups API
  slug: bytebase-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-groups-api-openapi.yml
- filename: bytebase-instances-api-openapi.yml
  format: yaml
  label: Bytebase Instances API
  slug: bytebase-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-instances-api-openapi.yml
- filename: bytebase-issues-api-openapi.yml
  format: yaml
  label: Bytebase Issues API
  slug: bytebase-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-issues-api-openapi.yml
- filename: bytebase-plans-api-openapi.yml
  format: yaml
  label: Bytebase Plans API
  slug: bytebase-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-plans-api-openapi.yml
- filename: bytebase-projects-api-openapi.yml
  format: yaml
  label: Bytebase Projects API
  slug: bytebase-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-projects-api-openapi.yml
- filename: bytebase-roles-api-openapi.yml
  format: yaml
  label: Bytebase Roles API
  slug: bytebase-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-roles-api-openapi.yml
- filename: bytebase-rollouts-api-openapi.yml
  format: yaml
  label: Bytebase Rollouts API
  slug: bytebase-rollouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-rollouts-api-openapi.yml
- filename: bytebase-sheets-api-openapi.yml
  format: yaml
  label: Bytebase Sheets API
  slug: bytebase-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-sheets-api-openapi.yml
- filename: bytebase-users-api-openapi.yml
  format: yaml
  label: Bytebase Users API
  slug: bytebase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-users-api-openapi.yml
- filename: bytebase-webhooks-api-openapi.yml
  format: yaml
  label: Bytebase Webhooks API
  slug: bytebase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-webhooks-api-openapi.yml
consequence_counts:
  read: 12
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bytebase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Bytebase exposes 24 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bytebase
provider_slug: bytebase
slug: bytebase-agentic-access
source_filename: bytebase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bytebase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 12\n    connected: 12\n  by_consequence:\n    write: 12\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance}\n  method: patch\n  operationId: updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /instances/{instance}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance}/databases\n  method: get\n  operationId: listInstanceDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance}/databases/{database}\n  method: get\n  operationId: getDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/issues/{issue}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/issues/{issue}:approve\n  method: post\n  operationId: approveIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/rollouts\n  method: post\n  operationId: createRollout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/rollouts/{rollout}\n  method: get\n  operationId: getRollout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/sheets\n  method: post\n  operationId: createSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/webhooks\n  method: post\n  operationId: addWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n\
  \  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/agentic-access/bytebase-agentic-access.yml
summary_line: 24 operations · 12 acting
tags:
- Database
- DevOps
- Schema Migration
- CI/CD
- DevSecOps
---
