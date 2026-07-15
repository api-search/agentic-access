---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 18
api_specs:
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Access Tokens API
  slug: atomic-fi-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Transact SDK
  slug: atomic-fi-transact-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Tasks API
  slug: atomic-fi-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Deposit API
  slug: atomic-fi-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Verify API
  slug: atomic-fi-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic PayLink API
  slug: atomic-fi-paylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Data & Transactions API
  slug: atomic-fi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
- filename: atomic-fi-openapi.yml
  format: yaml
  label: Atomic Webhooks API
  slug: atomic-fi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/openapi/atomic-fi-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Atomic Fi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /access-token/{publicToken}/revoke
operation_count: 30
overview: 'Atomic exposes 30 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 11 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atomic
provider_slug: atomic-fi
slug: atomic-fi-agentic-access
source_filename: atomic-fi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atomic-fi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 12\n    connected: 18\n  by_consequence:\n    write: 11\n    safety-critical: 1\n    read: 18\n  human_in_the_loop_required: 1\noperations:\n- path: /access-token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-token/{publicToken}/revoke\n  method: put\n  operationId: revokeAccessToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /company/search\n  method: post\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/list\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{companyId}/details\n  method: get\n  operationId: getCompanyDetails\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{taskId}/details\n  method: get\n  operationId: getTaskDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{taskId}/status\n  method: get\n  operationId: getTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{taskId}/file/{fileId}/generate-url\n  method: get\n  operationId: generateTaskFileUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/prescreen\n  method: post\n  operationId: prescreenTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /task-workflow/from-linked-account\n  method: post\n  operationId: createTaskWorkflowFromLinkedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposit-accounts/{identifier}\n  method: get\n  operationId: getDepositAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employment/{identifier}\n  method: get\n  operationId: getEmployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /identity/{identifier}\n  method: get\n  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /income/{identifier}\n  method: get\n  operationId: getIncome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/{identifier}\n  method: get\n  operationId: getStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timesheets/{identifier}\n  method: get\n  operationId: getTimesheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxes/{identifier}\n  method: get\n  operationId: getTaxes\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linked-account/list/{identifier}\n  method: get\n  operationId: listLinkedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay-link/actions-for-company/{companyId}\n  method: get\n  operationId: getPayLinkActionsForCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay-link/accounts\n  method: get\n  operationId: getPayLinkAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{identifier}/tasks\n  method: get\n  operationId: getUserTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{identifier}/end-monitoring\n  method: put\n  operationId: endUserMonitoring\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints\n\
  \  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{id}\n  method: put\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /secrets\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets\n  method: post\n  operationId: createSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secrets/{id}\n  method: delete\n  operationId: deleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-fi/refs/heads/main/agentic-access/atomic-fi-agentic-access.yml
summary_line: 30 operations · 12 acting · 1 human-in-the-loop
tags:
- Fintech
- Payroll
- Direct Deposit
- Income Verification
- Employment Verification
- Financial Connectivity
- Embedded Finance
---
