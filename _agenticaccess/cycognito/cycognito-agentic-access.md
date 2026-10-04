---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 20
api_specs:
- filename: cycognito-assets-api-openapi.yml
  format: yaml
  label: CyCognito Assets API
  slug: cycognito-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-assets-api-openapi.yml
- filename: cycognito-audit-logs-api-openapi.yml
  format: yaml
  label: CyCognito Audit Logs API
  slug: cycognito-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-audit-logs-api-openapi.yml
- filename: cycognito-cloud-connectors-api-openapi.yml
  format: yaml
  label: CyCognito Cloud Connectors API
  slug: cycognito-cloud-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-cloud-connectors-api-openapi.yml
- filename: cycognito-export-data-api-openapi.yml
  format: yaml
  label: CyCognito Export Data API
  slug: cycognito-export-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-export-data-api-openapi.yml
- filename: cycognito-issues-api-openapi.yml
  format: yaml
  label: CyCognito Issues API
  slug: cycognito-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-issues-api-openapi.yml
- filename: cycognito-organizations-api-openapi.yml
  format: yaml
  label: CyCognito Organizations API
  slug: cycognito-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-organizations-api-openapi.yml
- filename: cycognito-realm-api-openapi.yml
  format: yaml
  label: CyCognito Realm API
  slug: cycognito-realm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-realm-api-openapi.yml
- filename: cycognito-reports-api-openapi.yml
  format: yaml
  label: CyCognito Reports API
  slug: cycognito-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-reports-api-openapi.yml
- filename: cycognito-revalidation-api-openapi.yml
  format: yaml
  label: CyCognito Revalidation API
  slug: cycognito-revalidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-revalidation-api-openapi.yml
- filename: cycognito-scope-management-api-openapi.yml
  format: yaml
  label: CyCognito Scope Management API
  slug: cycognito-scope-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-scope-management-api-openapi.yml
- filename: cycognito-users-api-openapi.yml
  format: yaml
  label: CyCognito Users API
  slug: cycognito-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-users-api-openapi.yml
- filename: cycognito-verify-ips-api-openapi.yml
  format: yaml
  label: CyCognito Verify IPs API
  slug: cycognito-verify-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-verify-ips-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Cycognito Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/export/assets-to-pdf/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/is-scanner-ips
operation_count: 43
overview: 'CyCognito exposes 43 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 21 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CyCognito
provider_slug: cycognito
slug: cycognito-agentic-access
source_filename: cycognito-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cycognito-assets-api-openapi.yml, openapi/cycognito-audit-logs-api-openapi.yml,\n  openapi/cycognito-cloud-connectors-api-openapi.yml, openapi/cycognito-export-data-api-openapi.yml,\n  openapi/cycognito-issues-api-openapi.yml, openapi/cycognito-organizations-api-openapi.yml,\n  openapi/cycognito-realm-api-openapi.yml, openapi/cycognito-reports-api-openapi.yml, openapi/cycognito-revalidation-api-openapi.yml,\n  openapi/cycognito-scope-management-api-openapi.yml, openapi/cycognito-users-api-openapi.yml,\n  openapi/cycognito-verify-ips-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 20\n    acting: 23\n  by_consequence:\n    read:\
  \ 20\n    write: 21\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/assets\n  method: post\n  operationId: postV1Assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets\n  method: delete\n  operationId: deleteV1Assets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/{asset_type}\n  method: post\n  operationId: postV1AssetsByAssetType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{asset_type}/{asset_id}\n  method: get\n  operationId: getV1AssetsByAssetTypeByAssetId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{asset_type}/{asset_id}\n  method: delete\n  operationId: deleteV1AssetsByAssetTypeByAssetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/{asset_type}/{asset_id}/investigation-status\n  method: put\n  operationId: putV1AssetsByAssetTypeByAssetIdInvestigationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/actions/add/comment\n\
  \  method: put\n  operationId: putV1AssetsActionsAddComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/actions/{action}/tags\n  method: put\n  operationId: putV1AssetsActionsByActionTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audit-log\n  method: post\n  operationId: postV1AuditLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cloud-environments\n  method: get\n  operationId: getV1CloudEnvironments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cloud-environments\n  method: post\n  operationId: postV1CloudEnvironments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cloud-environments/script\n  method: post\n  operationId: postV1CloudEnvironmentsScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cloud-environments/{cloud-env-id}\n  method: get\n  operationId: getV1CloudEnvironmentsByCloudEnvId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/cloud-environments/{cloud-env-id}/test-connector\n  method: put\n  operationId: putV1CloudEnvironmentsByCloudEnvIdTestConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export/request/{type}\n  method: post\n  operationId: postV1ExportRequestByType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export/get/{report_id}\n  method: get\n  operationId: getV1ExportGetByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/export/issue-to-pdf/request\n  method: post\n  operationId: postV1ExportIssueToPdfRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export/issue-to-pdf/get/{report_id}\n  method: get\n  operationId: getV1ExportIssueToPdfGetByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/export/assets-to-pdf/request\n  method: post\n  operationId: postV1ExportAssetsToPdfRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/export/assets-to-pdf/get/{report_id}\n  method: get\n  operationId: getV1ExportAssetsToPdfGetByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues\n  method: post\n  operationId: postV1Issues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/issue/{issue_instance_id}\n  method: get\n  operationId: getV1IssuesIssueByIssueInstanceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/issue/{issue_instance_id}/investigation-status\n  method: put\n  operationId: putV1IssuesIssueByIssueInstanceIdInvestigationStatus\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/issues/actions/add/comment\n  method: put\n  operationId: putV1IssuesActionsAddComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/issues/actions/{action}/tags\n  method: put\n  operationId: putV1IssuesActionsByActionTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/issues/actions/archive\n  method: put\n  operationId: putV1IssuesActionsArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/issues/actions/snooze\n  method: put\n  operationId: putV1IssuesActionsSnooze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/archived-issues\n  method: post\n  operationId: postV1ArchivedIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolved-issues\n  method:\
  \ post\n  operationId: postV1ResolvedIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs\n  method: post\n  operationId: postV1Orgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/org-mgmt\n  method: post\n  operationId: postV1OrgsOrgMgmt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realm\n  method: get\n  operationId: getV1Realm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realm/asset-summary\n  method:\
  \ get\n  operationId: getV1RealmAssetSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/executive-report/request\n  method: post\n  operationId: postV1ReportsExecutiveReportRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/executive-report/get/{report_id}\n  method: get\n  operationId: getV1ReportsExecutiveReportGetByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/revalidate\n  method: post\n  operationId: postV1Revalidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/include-assets\n  method: post\n  operationId: postV1IncludeAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users\n  method: get\n  operationId: getV1Users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: postV1Users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{email}\n  method: get\n  operationId: getV1UsersByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{email}\n  method: put\n  operationId: putV1UsersByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{email}\n  method: delete\n  operationId: deleteV1UsersByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/is-scanner-ips\n  method: post\n  operationId: postV1IsScannerIps\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/agentic-access/cycognito-agentic-access.yml
summary_line: 43 operations · 23 acting · 1 human-in-the-loop
tags:
- Company
- Cybersecurity
- Attack Surface Management
- Exposure Management
- Security
- Vulnerability Management
- Cloud Security
- API Security
---
