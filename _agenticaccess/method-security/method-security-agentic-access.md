---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 8
api_specs:
- filename: method-security-openapi-original.yml
  format: yaml
  label: Method Platform API
  slug: method-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-openapi-original.yml
consequence_counts:
  read: 8
  safety-critical: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Method Security Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /method-api-gateway/api/v1/skills/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /method-api-gateway/api/v1/skills/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /method-api-gateway/api/v1/skills/{skillId}
operation_count: 18
overview: 'Method Security exposes 18 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 7 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Method Security
provider_slug: method-security
slug: method-security-agentic-access
source_filename: method-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/method-security-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 10\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /method-api-gateway/api/auth/getToken\n  method: post\n  operationId: getTokenWithClientCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/audit/getAuditEvents\n\
  \  method: post\n  operationId: getAuditEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/blueprints/\n  method: get\n  operationId: listBlueprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/blueprints/{blueprintId}/run\n  method: post\n  operationId: runBlueprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/environments/\n\
  \  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/environments/{environmentId}/intel\n  method: post\n  operationId: uploadEnvironmentIntel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/issues/{id}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/issues/{id}/update\n\
  \  method: post\n  operationId: updateIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/reports/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/signals/{signalId}/content\n  method: get\n  operationId: getSignalContentServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/skills/search\n  method: post\n  operationId: searchSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /method-api-gateway/api/v1/skills/{skillId}\n  method: get\n  operationId: getSkill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/skills/{skillId}\n  method: put\n  operationId: updateSkill\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /method-api-gateway/api/v1/skills/\n  method: post\n  operationId: createSkill\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /method-api-gateway/api/v1/system/externalIp\n  method: get\n  operationId: getExternalIPAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/targets/search\n  method: post\n  operationId: searchTargets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /method-api-gateway/api/v1/targets/{targetId}\n  method: get\n  operationId: getTarget\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /method-api-gateway/api/v1/targets/{targetId}/reports\n  method: get\n  operationId: getTargetReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/agentic-access/method-security-agentic-access.yml
summary_line: 18 operations · 10 acting · 3 human-in-the-loop
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Exposure Management
- Attack Surface Management
- Vulnerability Management
- Red Team
- AI Agents
- Government
---
