---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: productiv-app-details-api-openapi.yml
  format: yaml
  label: Productiv App Details API
  slug: productiv-app-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-app-details-api-openapi.yml
- filename: productiv-app-summaries-api-openapi.yml
  format: yaml
  label: Productiv App Summaries API
  slug: productiv-app-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-app-summaries-api-openapi.yml
- filename: productiv-applications-api-openapi.yml
  format: yaml
  label: Productiv Applications API
  slug: productiv-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-applications-api-openapi.yml
- filename: productiv-audit-events-api-openapi.yml
  format: yaml
  label: Productiv Audit Events API
  slug: productiv-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-audit-events-api-openapi.yml
- filename: productiv-authentication-api-openapi.yml
  format: yaml
  label: Productiv Authentication API
  slug: productiv-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-authentication-api-openapi.yml
- filename: productiv-batch-upload-api-openapi.yml
  format: yaml
  label: Productiv Batch Upload API
  slug: productiv-batch-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-batch-upload-api-openapi.yml
- filename: productiv-org-chart-api-openapi.yml
  format: yaml
  label: Productiv Org Chart API
  slug: productiv-org-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-org-chart-api-openapi.yml
- filename: productiv-provisioned-users-api-openapi.yml
  format: yaml
  label: Productiv Provisioned Users API
  slug: productiv-provisioned-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-provisioned-users-api-openapi.yml
- filename: productiv-provisioning-workflows-api-openapi.yml
  format: yaml
  label: Productiv Provisioning Workflows API
  slug: productiv-provisioning-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-provisioning-workflows-api-openapi.yml
- filename: productiv-spend-data-api-openapi.yml
  format: yaml
  label: Productiv Spend Data API
  slug: productiv-spend-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-spend-data-api-openapi.yml
- filename: productiv-usage-events-api-openapi.yml
  format: yaml
  label: Productiv Usage Events API
  slug: productiv-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-usage-events-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Productiv Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/push/v1/customer/apps/{appId}/users
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /services/push/v1/customer/apps/{appId}/users
operation_count: 15
overview: 'Productiv exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Productiv
provider_slug: productiv
slug: productiv-agentic-access
source_filename: productiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/productiv-developer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 5\n    physical: 2\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/apps\n  method: post\n  operationId: setupApplication\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/apps/{appId}/usage-events\n  method: post\n  operationId: publishUsageEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/apps/{appId}/spend\n  method: post\n  operationId: publishSpendData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /services/push/v1/customer/apps/{appId}/users\n  method: post\n  operationId: publishProvisionedUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/apps/{appId}/users\n  method: get\n  operationId: getProvisionedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/push/v1/customer/apps/{appId}/users\n  method: delete\n  operationId: deleteProvisionedUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/org-chart\n  method: put\n  operationId: publishOrgChart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/push/v1/customer/apps/{appId}/upload\n  method: get\n  operationId: getBatchUploadUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/export/v1/customer/app-summaries\n  method: get\n  operationId: getAppSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /services/export/v1/customer/app-details/{applicationId}\n  method: get\n  operationId: getAppDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/export/v1/customer/provisioning-workflows\n  method: get\n  operationId: listProvisioningWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/export/v1/customer/provisioning-workflows/{workflowId}/executions\n  method: get\n  operationId: listProvisioningExecutionSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/export/v1/customer/provisioning-workflows/{workflowId}/executions/{executionId}\n  method: get\n  operationId: getProvisioningWorkflowExecution\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/export/v1/customer/audit-events\n  method: get\n  operationId: getAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/agentic-access/productiv-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
---
