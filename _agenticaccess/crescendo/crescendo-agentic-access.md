---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: crescendo-platform-openapi-original.json
  format: json
  label: Crescendo Platform API
  slug: crescendo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/openapi/crescendo-platform-openapi-original.json
consequence_counts:
  physical: 6
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crescendo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/provisioning/tenants/{tenantId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/provisioning/tenants/{tenantId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}/versions/current
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}/versions/current
operation_count: 17
overview: 'Crescendo exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 2 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crescendo
provider_slug: crescendo
slug: crescendo-agentic-access
source_filename: crescendo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/crescendo-platform-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    physical: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provisioning/tenants/{tenantId}\n  method: get\n  operationId: getProvisioningTenant\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provisioning/tenants/{tenantId}\n  method: post\n  operationId: postProvisioningTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/provisioning/tenants/{tenantId}\n  method: put\n  operationId: putProvisioningTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}\n  method: get\n  operationId: listProvisioningCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}\n  method: get\n  operationId: getProvisioningDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}\n  method: post\n  operationId: postProvisioningDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}\n  method: put\n  operationId: putProvisioningDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}/versions/current\n  method: get\n  operationId: getProvisioningVersionCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}/versions/current\n  method: post\n  operationId: postProvisioningVersionCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/provisioning/tenants/{tenantId}/{collection}/{docId}/versions/current\n  method: put\n  operationId: putProvisioningVersionCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reporting/tenants/{tenantId}/assistant/conversations\n  method: get\n  operationId: listReportingBotConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/reporting/tenants/{tenantId}/voc/conversations\n  method: get\n  operationId: listReportingVocConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/voc/tenants/{tenantId}/recording\n  method: post\n  operationId: uploadVocRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/voc/tenants/{tenantId}/recording/{jobId}/status\n  method: get\n  operationId: getVocJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mcp/tenants/{tenantId}/bots\n  method: post\n  operationId: mcpBots\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/agentic-access/crescendo-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Company
- Customer Experience
- Customer Support
- Artificial Intelligence
- AI Agents
- Contact Center
- Conversational AI
- Voice of Customer
- MCP
---
