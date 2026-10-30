---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 16
api_specs:
- filename: appmixer-accounts-api-openapi.yml
  format: yaml
  label: Appmixer Accounts API
  slug: appmixer-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-accounts-api-openapi.yml
- filename: appmixer-apps-api-openapi.yml
  format: yaml
  label: Appmixer Apps API
  slug: appmixer-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-apps-api-openapi.yml
- filename: appmixer-authentication-api-openapi.yml
  format: yaml
  label: Appmixer Authentication API
  slug: appmixer-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-authentication-api-openapi.yml
- filename: appmixer-files-api-openapi.yml
  format: yaml
  label: Appmixer Files API
  slug: appmixer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-files-api-openapi.yml
- filename: appmixer-flows-api-openapi.yml
  format: yaml
  label: Appmixer Flows API
  slug: appmixer-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-flows-api-openapi.yml
- filename: appmixer-insights-api-openapi.yml
  format: yaml
  label: Appmixer Insights API
  slug: appmixer-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-insights-api-openapi.yml
- filename: appmixer-acl-api-openapi.yml
  format: yaml
  label: Appmixer ACL API
  slug: appmixer-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-acl-api-openapi.yml
- filename: appmixer-audit-logs-api-openapi.yml
  format: yaml
  label: Appmixer Audit Logs API
  slug: appmixer-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-audit-logs-api-openapi.yml
- filename: appmixer-automation-hub-api-openapi.yml
  format: yaml
  label: Appmixer Automation Hub API
  slug: appmixer-automation-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-automation-hub-api-openapi.yml
- filename: appmixer-config-api-openapi.yml
  format: yaml
  label: Appmixer Config API
  slug: appmixer-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-config-api-openapi.yml
- filename: appmixer-connector-configuration-api-openapi.yml
  format: yaml
  label: Appmixer Connector Configuration API
  slug: appmixer-connector-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-connector-configuration-api-openapi.yml
- filename: appmixer-integration-categories-api-openapi.yml
  format: yaml
  label: Appmixer Integration Categories API
  slug: appmixer-integration-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-integration-categories-api-openapi.yml
- filename: appmixer-modifiers-api-openapi.yml
  format: yaml
  label: Appmixer Modifiers API
  slug: appmixer-modifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-modifiers-api-openapi.yml
- filename: appmixer-public-files-api-openapi.yml
  format: yaml
  label: Appmixer Public Files API
  slug: appmixer-public-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-public-files-api-openapi.yml
- filename: appmixer-unprocessed-messages-api-openapi.yml
  format: yaml
  label: Appmixer Unprocessed Messages API
  slug: appmixer-unprocessed-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-unprocessed-messages-api-openapi.yml
- filename: appmixer-user-api-openapi.yml
  format: yaml
  label: Appmixer User API
  slug: appmixer-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-user-api-openapi.yml
- filename: appmixer-user-groups-api-openapi.yml
  format: yaml
  label: Appmixer User Groups API
  slug: appmixer-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-user-groups-api-openapi.yml
- filename: appmixer-variables-api-openapi.yml
  format: yaml
  label: Appmixer Variables API
  slug: appmixer-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-variables-api-openapi.yml
- filename: appmixer-datastores-api-openapi.yml
  format: yaml
  label: Appmixer Datastores API
  slug: appmixer-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-datastores-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Appmixer Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /flows/{flowId}/stop
operation_count: 33
overview: 'Appmixer exposes 33 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Appmixer
provider_slug: appmixer
slug: appmixer-agentic-access
source_filename: appmixer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/appmixer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 16\n    acting: 17\n  by_consequence:\n    read: 16\n    write: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: get\n  operationId: getApiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/auth\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n\
  \  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flows\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows/{flowId}\n  method: get\n  operationId: getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flows/{flowId}\n  method: put\n  operationId: updateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows/{flowId}\n  method: delete\n  operationId: deleteFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows/{flowId}/start\n  method: put\n  operationId: startFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows/{flowId}/stop\n  method: put\n  operationId: stopFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components\n  method: get\n  operationId: listComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components\n  method: post\n  operationId: publishComponent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /components/{componentId}\n  method: delete\n  operationId: deleteComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}\n  method: get\n  operationId: getFile\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-stores\n  method: get\n  operationId: listDataStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{storeId}\n  method: get\n  operationId: getDataStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{storeId}\n  method: delete\n  operationId: deleteDataStore\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights\n  method: get\n  operationId: listInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people-task/tasks\n  method: get\n  operationId: listPeopleTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs\n  method: get\n  operationId: getLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unprocessed-messages\n  method: get\n  operationId: listUnprocessedMessages\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unprocessed-messages/{messageId}\n  method: post\n  operationId: reprocessMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unprocessed-messages/{messageId}\n  method: delete\n  operationId: deleteUnprocessedMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/agentic-access/appmixer-agentic-access.yml
summary_line: 33 operations · 17 acting · 1 human-in-the-loop
tags:
- AI Agents
- Automation
- Embedded iPaaS
- Integration
- Low-Code
- Workflows
---
