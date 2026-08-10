---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: antimetal-artifacts-api-openapi.yml
  format: yaml
  label: Antimetal Artifacts API
  slug: antimetal-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-artifacts-api-openapi.yml
- filename: antimetal-issues-api-openapi.yml
  format: yaml
  label: Antimetal Issues API
  slug: antimetal-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-issues-api-openapi.yml
- filename: antimetal-query-api-openapi.yml
  format: yaml
  label: Antimetal Query API
  slug: antimetal-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-query-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Antimetal Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Antimetal exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Antimetal
provider_slug: antimetal
slug: antimetal-agentic-access
source_filename: antimetal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/antimetal-external-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 4\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/by_number/{number}\n  method: get\n  operationId: getIssueByNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/{id}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/{id}\n  method: patch\n  operationId: updateIssueStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/{id}\n  method: delete\n  operationId: deleteIssue\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/{id}/results\n  method: get\n  operationId: getIssueResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artifacts\n  method: get\n  operationId: batchGetArtifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: post\n  operationId: query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/agentic-access/antimetal-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- Observability
- Incident Management
- Site Reliability Engineering
- Artificial Intelligence
- Agents
- DevOps
- Cloud Infrastructure
- Kubernetes
- Root Cause Analysis
- MCP
---
