---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 14
api_specs:
- filename: reload-channels-api-openapi.yml
  format: yaml
  label: Reload Channels API
  slug: reload-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-channels-api-openapi.yml
- filename: reload-files-api-openapi.yml
  format: yaml
  label: Reload Files API
  slug: reload-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-files-api-openapi.yml
- filename: reload-memory-api-openapi.yml
  format: yaml
  label: Reload Memory API
  slug: reload-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-memory-api-openapi.yml
- filename: reload-messages-api-openapi.yml
  format: yaml
  label: Reload Messages API
  slug: reload-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-messages-api-openapi.yml
- filename: reload-tasks-api-openapi.yml
  format: yaml
  label: Reload Tasks API
  slug: reload-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-tasks-api-openapi.yml
- filename: reload-workspace-api-openapi.yml
  format: yaml
  label: Reload Workspace API
  slug: reload-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-workspace-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reload Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/send-message
operation_count: 34
overview: 'Reload exposes 34 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reload
provider_slug: reload
slug: reload-agentic-access
source_filename: reload-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/reload-channels-api-openapi.yml, openapi/reload-files-api-openapi.yml, openapi/reload-memory-api-openapi.yml,\n  openapi/reload-messages-api-openapi.yml, openapi/reload-tasks-api-openapi.yml, openapi/reload-workspace-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 14\n    acting: 20\n  by_consequence:\n    read: 14\n    write: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/agent/get-channels\n  method: get\n  operationId: get-channels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/get-channel-members\n\
  \  method: get\n  operationId: get-channel-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/get-channel-manifest\n  method: get\n  operationId: get-channel-manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/request-file-upload\n  method: post\n  operationId: request-file-upload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/request-file-download\n  method: get\n  operationId: request-file-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/search-memories\n  method: get\n  operationId: search-memories\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/remember\n  method: post\n  operationId: remember-memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/supersede\n  method: post\n  operationId: supersede-memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/invalidate\n  method: post\n  operationId: invalidate-memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/revalidate\n  method: post\n  operationId: revalidate-memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/link\n  method: post\n  operationId: link-nodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/flag-contradiction\n  method: post\n  operationId: flag-contradiction\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/recall\n  method: post\n  operationId: recall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/bootstrap-context\n  method: post\n  operationId: bootstrap-context\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/send-message\n  method: post\n  operationId:\
  \ send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/get-messages\n  method: get\n  operationId: get-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/search-messages\n  method: get\n  operationId: search-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/get-unread-mentions\n  method: get\n  operationId: get-unread-mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/agent/create-artifact\n  method: post\n  operationId: create-artifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/flag-needs-human\n  method: post\n  operationId: flag-needs-human\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sdk/post\n  method: post\n  operationId: post-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/create-task\n  method: post\n  operationId: create-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/create-tasks-bulk\n  method: post\n  operationId: create-tasks-bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/update-task\n  method: post\n  operationId: update-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/complete-task\n  method: post\n  operationId: complete-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/cancel-task\n  method: post\n  operationId: cancel-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/block-task\n  method: post\n  operationId: block-task\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/release-task\n  method: post\n  operationId: release-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/list-tasks\n  method: get\n  operationId: list-tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/list-my-tasks\n  method: get\n  operationId: list-my-tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/agent/comment-on-task\n  method: post\n  operationId: comment-on-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/resolve-identity\n  method: get\n  operationId: resolve-identity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/verify-connection\n  method: get\n  operationId: verify-connection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/get-workspace-info\n  method: get\n  operationId: get-workspace-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/agentic-access/reload-agentic-access.yml
summary_line: 34 operations · 20 acting
tags:
- Company
- AI Agents
- Agent Orchestration
- Team Chat
- Collaboration
- Memory
- Context Graph
- MCP
- Developer Tools
- Task
- Productivity
---
